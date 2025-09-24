---
layout: post
title: Performance-Based Biped Control using a Consumer Depth Camera
nav-menu: false
show_tile: false
---

[Yoonsang Lee](../people/yoonsang-lee.html), [Taesoo Kwon](http://calab.hanyang.ac.kr/cgi-bin/home.cgi?node=Taesoo)  
Computer Graphics Forum, Volume 36, Issue 2, 387-395, May 2017 (Presented at Eurographics 2017)

![teaser](../assets/publications/2017-perf-based/perf-biped-teaser.png)  
*A user controls a physically simulated character by moving his or her body parts. Top: The input depth data of user poses. Bottom: The simulated character imitating the user’s actions.*

## Abstract
We present a technique for controlling physically simulated characters using user inputs from an off-the-shelf depth camera. Our controller takes a real-time stream of user poses as input, and simulates a stream of target poses of a biped based on it. The simulated biped mimics the user's actions while moving forward at a modest speed and maintaining balance. The controller is parameterized over a set of modulated reference motions that aims to cover the range of possible user actions. For real-time simulation, the best set of control parameters for the current input pose is chosen from the parameterized sets of pre-computed control parameters via a regression method. By applying the chosen parameters at each moment, the simulated biped can imitate a range of user actions while walking in various interactive scenarios. 

## Paper
Publisher: [page](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.13134), [paper](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.13134)\
arXiv: [page](https://arxiv.org/abs/2401.15523), [paper](https://arxiv.org/pdf/2401.15523)\
Preprint: [paper](https://gitcgr.hanyang.ac.kr/publications/2017-perf-based/perf-biped-preprint.pdf)

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="1280" height="720" src="https://www.youtube.com/embed/WVDPXdlnhBM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div></div>  
[Download mp4 (67.3MB)](https://gitcgr.hanyang.ac.kr/publications/2017-perf-based/perf-biped-final.mp4)

## Slides
Eurographics 2017 presentation slides: [pdf](https://gitcgr.hanyang.ac.kr/publications/2017-perf-based/perf-biped-v2-public.pdf) (2.0MB), [pptx](https://gitcgr.hanyang.ac.kr/publications/2017-perf-based/perf-biped-v2-public.pptx) (193.9MB)
