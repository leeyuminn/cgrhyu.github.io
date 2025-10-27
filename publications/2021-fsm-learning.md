---
layout: publication_post
title: Finite State Machine-Based Motion-Free Learning of Biped Walking
nav-menu: false
show_tile: false
---

<div class="venue">
	IEEE Access (2021)
</div>

<div class="authors">
	<span>Gyoo-Chul Kang<sup>1,2</sup></span>
  <a href="../people/yoonsang-lee.html">Yoonsang Lee<sup>2</sup></a>
</div>

<div class="affiliations"> 
    <div><sup>1</sup> CLO Virtual Fashion LLC.</div>
    <div><sup>2</sup> Hanyang University, Department of Computer Science</div>
</div>

<div class="link-buttons">
  <a href="https://ieeexplore.ieee.org/document/9337805" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-doi"></span>
    <span>Publisher</span>
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-arxiv"></span>
    <span>arXiv (coming soon)</span>
  </a>
</div>

<!--Gyoo-Chul Kang, [Yoonsang Lee](../people/yoonsang-lee.html)  -->
<!--IEEE Access, Volume 9, 20662-20672, January 2021-->

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="1047" height="589" src="https://www.youtube.com/embed/jqgf-sHqCz0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div></div>  
<br/>
<!--[Download mp4 (48.4MB)](https://gitcgr.hanyang.ac.kr/publications/2021-fsm-learning/final-video.mp4)-->

## Abstract
Recently, deep reinforcement learning (DRL) is commonly used to create controllers for physically simulated characters. Among DRL-based approaches, imitation learning for character control using motion capture clips as tracking references has shown successful results in controlling various motor skills with natural movement. However, the output motion tends to be constrained close to the reference motion, and thus the learning of various styles of motion requires many motion clips. In this paper, we present a DRL method for learning a finite state machine (FSM) based policy in a motion-free manner (without the use of any motion data), which controls a simulated character to produce a gait as specified by the desired gait parameters. The control policy learns to output the target pose for each FSM state and transition timing between states, based on the character state at the beginning of each step and the user-specified gait parameters, such as the desired step length or maximum swing foot height. The combination of FSM-based policy learning and simple linear balance feedback embedded in the base controller has a positive synergistic effect on the performance of the learned policy. The learned policy allows the simulated character to walk as instructed by the continuously changing the gait parameters while responding to external perturbations. We demonstrate the effectiveness of our approach through interactive control, external push, comparison, and ablation studies.

## Paper
Publisher: [page](https://ieeexplore.ieee.org/document/9337805), [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9337805)

