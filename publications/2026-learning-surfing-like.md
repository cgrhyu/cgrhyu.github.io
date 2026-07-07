---
layout: publication_post
title: 'Learning Surfing-like Balance without Water Simulation'
nav-menu: false
show_tile: false
---

<div class="venue">
    SIGGRAPH 2026 Posters
</div>

<div class="authors">
	<a href="../people/hauk-nam.html">Hauk Nam<sup>*</sup></a>
	<a href="../people/changho-lee.html">Changho Lee<sup>*</sup></a>
	<a href="../people/yoonsang-lee.html">Yoonsang Lee</a>
</div>

<div class="affiliations"> 
    Hanyang University
</div>

<div class="additional"> 
	<sup>*</sup> Co-first authors
</div>

<div class="link-buttons">
  <a href="https://dl.acm.org/doi/abs/10.1145/3799825.3818707" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-doi"></span>
    <span>Publisher</span>
  </a>

  <a href="https://gitcgr.hanyang.ac.kr/publications/2026-learning-surfing-like/learning-surfing-like-poster.pdf" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-image"></span>
    <span>Poster</span>
  </a>
</div>


![teaser](../assets/publications/2026-learning-surfing-like/teaser-1080.png)  
*Our method learns surfing-like balance control without water simulation. The learned policy maintains stable balance on a moving board under wave conditions at runtime.*

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="730" height="411" src="https://www.youtube.com/embed/Vf1hafwHSmM" title="Learning Surfing-like Balance without Water Simulation" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div></div>  
<br/>

## Abstract
Controlling characters in fluid environments such as water remains challenging due to complex dynamics and high simulation cost. In particular, surfing requires maintaining balance on a continuously moving support, making stable control difficult without accurate physical modeling. In this work, we present a method for learning surfing-like balance control without relying on water simulation. Our approach combines a hierarchical control framework with a stage-based training scheme that progressively introduces dynamic board behavior. The low-level policy generates full-body motion from partial joint targets, while the high-level policy adapts these targets based on environmental conditions.
Despite being trained entirely in a non-fluid setting, the learned policy maintains stable balance on a moving board under wave conditions at runtime. These results suggest that surfing-like balance can be achieved without explicitly modeling fluid dynamics through appropriate control structures and training strategies.

<!--## Paper-->
<!--Publisher: [page](https://ieeexplore.ieee.org/document/11519541)-->
<!--\-->
<!--arXiv: [page](https://arxiv.org/abs/2511.07860), [paper](https://arxiv.org/pdf/2511.07860)-->
