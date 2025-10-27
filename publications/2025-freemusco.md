---
layout: publication_post
title: 'FreeMusco: Motion-Free Learning of Latent Control for Morphology-Adaptive Locomotion in Musculoskeletal Characters'
nav-menu: false
show_tile: false
---

<div class="venue">
	SIGGRAPH Asia 2025
</div>

<div class="authors">
  <a href="../people/minkwan-kim.html">Minkwan Kim</a>
  <a href="../people/yoonsang-lee.html">Yoonsang Lee</a>
</div>

<div class="affiliations"> 
    Hanyang University
</div>

<div class="link-buttons">
  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-doi"></span>
    <span>Publisher (coming soon)</span>
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-arxiv"></span>
    <span>arXiv (coming soon)</span>
  </a>

  <a href="https://gitcgr.hanyang.ac.kr/publications/2025-b2f/18_B2F_End-to-End Body-to-Face Motion Generation with Style Reference.pdf" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-file-pdf-o"></span>
    <span>Slides (PDF) (coming soon)</span>
  </a>

  <a href="https://gitcgr.hanyang.ac.kr/publications/2025-b2f/18_B2F_End-to-End Body-to-Face Motion Generation with Style Reference.pptx" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-file-powerpoint-o"></span>
    <span>Slides (PPTX) (coming soon)</span>
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-github"></span>
    <span>Code (coming soon)</span>
  </a>
</div>

<!--[Minkwan Kim](../people/minkwan-kim.html), [Yoonsang Lee](../people/yoonsang-lee.html)  -->
<!--To appear in SIGGRAPH Asia 2025-->

![teaser](../assets/publications/2025-freemusco/FreeMusco-teaser-web.jpg)  
*FreeMusco is a motion-free framework that learns a latent representation of morphology-adaptive locomotion from musculoskeletal simulation, without motion data. The learned latent space enables high-level control for downstream tasks such as goal navigation and path following. The figure shows: (1) Humanoid locomotion control, (2) diverse motions sampled from the latent space, (3) goal navigation with Ostrich, and (4) path following with Chimanoid.*

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="1198" height="674" src="https://www.youtube.com/embed/YFNKLzUQ0zk" title="FreeMusco: Motion-Free Learning of Latent Control for Morphology-Adaptive Locomotion in Musculoske.." frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div></div>  
<br/>

## Abstract
We propose FreeMusco, a motion-free framework that jointly learns latent representations and control policies for musculoskeletal characters. By leveraging the musculoskeletal model as a strong prior, our method enables energy-aware and morphology-adaptive locomotion to emerge without motion data. The framework generalizes across human, non-human, and synthetic morphologies, where distinct energy-efficient strategies naturally appear—for example, quadrupedal gaits in Chimanoid versus bipedal gaits in Humanoid. The latent space and corresponding control policy are constructed from scratch, without demonstration, and enable downstream tasks such as goal navigation and path following—representing, to our knowledge, the first motion-free method to provide such capabilities. FreeMusco learns diverse and physically plausible locomotion behaviors through model-based reinforcement learning, guided by the locomotion objective that combines control, balancing, and biomechanical terms. To better capture the periodic structure of natural gait, we introduce a temporally averaged loss formulation, which compares simulated and target states over a time window rather than on a per-frame basis. We further encourage behavioral diversity by randomizing target poses and energy levels during training, enabling locomotion to be flexibly modulated in both form and intensity at runtime. Together, these results demonstrate that versatile and adaptive locomotion control can emerge without motion capture, offering a new direction for simulating movement in characters where data collection is impractical or impossible.

## Paper
Publisher: Coming soon  
arXiv: Coming soon
<!--Publisher: [page](https://dl.acm.org/doi/10.1145/3731425), [paper](https://dl.acm.org/doi/pdf/10.1145/3731425)\-->
<!--arXiv: [page](https://arxiv.org/abs/2504.21216), [paper](https://arxiv.org/pdf/2504.21216)-->


<!--## Presentation & Poster-->
<!--SIGGRAPH 2025 Technical Papers Presentation Slides: [pdf](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-siggraph-presentation.pdf) (3.5MB), [pptx](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-siggraph-presentation.pptx) (369.7MB)  -->
<!--SIGGRAPH 2025 Emerging Technologies & Interactive Discussion Poster: [pdf](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-etech-intdis-poster.pdf) (523KB)-->

