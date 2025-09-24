---
layout: landing
title: Showcase
image: assets/home/showcase.jpg
nav-menu: true
banner_style: style4
---

<section id="one">
<div class="inner">

<div class="row">
<b><a href="5-showcase-seniorprojs.html">Showcase - Senior Projects</a></b>
<!--<b><a href="6-showcase-pblprojs.html">Showcase - PBL Projects</a></b>-->
</div>

<div class="row">
<p/>
</div>

<div class="row">

<div class="3u 12u$(small)">
Conference / Journal:
<select id="conf_select" onChange="onSelect()">
  <option value='all'>ALL</option>
  <option value='siggraph'>SIGGRAPH (Asia) / TOG</option>
</select>
</div>

<div class="2u 12u$(small)">
Year:
<select id="year_select" onChange="onSelect()">
  <option value='all'>ALL</option>
</select>
</div>

</div>

<p/>

<div id="contents">

<script>
// https://stackoverflow.com/questions/610406/javascript-equivalent-to-printf-string-format
// First, checks if it isn't implemented yet.
if (!String.prototype.format) {
  String.prototype.format = function() {
    var args = arguments;
    return this.replace(/{(\d+)}/g, function(match, number) { 
      return typeof args[number] != 'undefined'
        ? args[number]
        : match
      ;
    });
  };
}

function dynamicallyLoadScript(url) {
    var script = document.createElement("script");  // create a script DOM node
    script.src = url;  // set its src to the provided URL

    document.head.appendChild(script);  // add it to the end of the head section of the page (could change 'head' to 'body' to add it to the end of the body section instead)
}

dynamicallyLoadScript('publications-eng.js');

function onSelect() {
	var items = publications_eng;

	var year_select = document.getElementById("year_select");
	var year = year_select.options[year_select.selectedIndex].value;

	var conf_select = document.getElementById("conf_select");
	var conf = conf_select.options[conf_select.selectedIndex].value;

	var contents_code = '';
	var showCount = 0;

	for(var i = 0; i < items.length; i++) 
	{
		var item = items[i];
		var show = false;

		if(year=='all')
			show = true;
		else
			show = false;

		if(show)
		{
			if(conf=='siggraph'
				&& (item.conference_journal=='SIGGRAPH' || item.conference_journal=='SIGGRAPH Asia'
					|| item.conference_journal=='TOG'))
				show = true;
			else if(conf=='all')
				show = true;
			else
				show = false;
		}

		if(!('video_iframe' in item))
			show = false;

		if(show)
		{
			if(showCount % 2 == 0)
				contents_code += '<div class="row">';
/*
			if(item.type=='paper')
				typestr = 'Paper';
			else if(item.type=='poster')
				typestr = 'Poster';
			else if(item.type=='senior')
				typestr = 'Senior Project';
			else if(item.type=='pbl')
				typestr = 'PBL Project';
*/
			contents_code += '<div class="6u 12u$(small)">';
			if('id' in item)
				project_page = item.project_page + '#' + item.id;
			else
				project_page = item.project_page
			contents_code += '<b><a href={0} rel="noopener noreferrer" target="_blank">{1} ({2})</a></b><br/>'.format(project_page, item.title, item.year);
			contents_code += '<div id="iframe_container"> <div id="iframe">';
			contents_code += '{0}'.format(item.video_iframe);;
			contents_code += '</div></div>';
			contents_code += '<br/></div>';

			if(showCount % 2 == 1 || i == items.length-1)
				contents_code += '</div>';

			showCount += 1;
		}
	}

	var contents = document.getElementById("contents");
	contents.innerHTML = contents_code;
}

// set default value and trigger onchange event when window is loaded
window.onload = function () {
	var year_select = document.getElementById("year_select");
	year_select.value = 'all';

	var conf_select = document.getElementById("conf_select");
	conf_select.value = 'all';
	conf_select.onchange();

}

</script>

</div>
</div>
</section>

<!--<section id="one">-->
<!--<div class="inner">-->
<!--<div class="row">-->

<!--<div class="6u 12u$(small)">-->
<!--<b><a href="publications/2018-iguana-ctrl.html">Control of an Iguana Character Using Soft-Body Simulation</a></b><br/>-->
<!--<div id="iframe_container"> <div id="iframe">-->
<!--<iframe width="1280" height="720" src="https://www.youtube.com/embed/c37VEexDZaY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  -->
<!--</div></div>  -->
<!--</div>-->

<!--</div>-->
<!--</div>-->
<!--</section>-->
