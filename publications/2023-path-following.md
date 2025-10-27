---
layout: publication_post
title: Interactive Character Path-Following Using Long-Horizon Motion Matching With Revised Future Queries
nav-menu: false
show_tile: false
---

<div class="venue">
	IEEE Access (2023)
</div>

<div class="authors">
  <a href="../people/jeongmin-lee.html">Jeongmin Lee<sup>1,2</sup></a>
  <a href="http://calab.hanyang.ac.kr/cgi-bin/home.cgi?node=Taesoo">Taesoo Kwon<sup>2</sup></a>
  <a href="../people/yoonsang-lee.html">Yoonsang Lee<sup>2</sup></a>
</div>

<div class="affiliations"> 
    <div><sup>1</sup> Samsung Electronics Co., Seoul R&D Campus</div>
    <div><sup>2</sup> Hanyang University, Department of Computer Science</div>
</div>

<div class="link-buttons">
  <a href="https://ieeexplore.ieee.org/document/10029373" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-doi"></span>
    <span>Publisher</span>
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-arxiv"></span>
    <span>arXiv (coming soon)</span>
  </a>

  <a href="https://github.com/jmmhappy/InteractiveCharacterPathFollowing" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-github"></span>
    <span>Code</span>
  </a>
</div>

<!--[Jeongmin Lee](../people/jeongmin-lee.html), [Taesoo Kwon](http://calab.hanyang.ac.kr/cgi-bin/home.cgi?node=Taesoo), [Yoonsang Lee](../people/yoonsang-lee.html)  -->
<!--IEEE Access, Volume 11, 9942-9956, January 2023-->

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="1536" height="864" src="https://www.youtube.com/embed/N357UBDALpw" title="Interactive Character Path-Following using Long-Horizon Motion Matching with Revised Future Queries" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div></div>  
<br/>

## Abstract
We propose a method for interactively generating a character motion that follows a user-specified path based on motion matching. Unlike basic motion matching that finds the best frame considering only the current state and current control input, our long-horizon motion matching algorithm is performed recursively over multiple levels and finds the matching path that minimizes the total distance, to find the best frame for a longer future interval. The matching query is carefully revised from the raw query directly extracted from the user path to address the following aspects: inherent differences between an actual moving path of a human and a user-drawn path, and possible user errors such as a path drawn with excessive speed or with abrupt changes in direction. Also, two interactive control modes for path-following characters are proposed. The combination of our long-horizon motion matching and carefully revised queries enables smooth and reliable interactive path tracking for a variety of paths. We show the effectiveness of our method using various experiments such as path-following with different shaped paths, game-like interactive control demos, and ablation studies.

## Paper
Publisher: [page](https://ieeexplore.ieee.org/document/10029373), [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10029373)

## Code
[Github repository](https://github.com/jmmhappy/InteractiveCharacterPathFollowing)
