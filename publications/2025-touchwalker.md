---
layout: publication_post
title: 'TouchWalker: Real-Time Avatar Locomotion from Touchscreen Finger Walking'
nav-menu: false
show_tile: false
---

<div class="venue">
    ISMAR 2025
</div>

<div class="authors">
	<a href="../people/geuntae-park.html">Geuntae Park<sup>1</sup></a>
	<a href="../people/jiwon-yi.html">Jiwon Yi<sup>1</sup></a>
	<a href="https://findanexpert.unimelb.edu.au/profile/1084098-taehyun-rhee">Taehyun Rhee<sup>2</sup></a>
	<a href="http://hcilab.dothome.co.kr/professor/166">Kwanguk Kim<sup>1</sup></a>
	<a href="../people/yoonsang-lee.html">Yoonsang Lee<sup>1</sup></a>
</div>

<div class="affiliations"> 
    <div><sup>1</sup> Hanyang University</div>
    <div><sup>2</sup> University of Melbourne</div>
</div>

<div class="link-buttons">
  <a href="https://www.computer.org/csdl/proceedings-article/ismar/2025/876100a582/2byAkM9tRiE" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-doi"></span>
    <span>Publisher</span>
  </a>

  <a href="https://arxiv.org/abs/2511.07860" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-arxiv"></span>
    <span>arXiv</span>
  </a>

  <a href="https://gitcgr.hanyang.ac.kr/publications/2025-touchwalker/touchwalker-ismar-presentation.pdf" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-file-pdf-o"></span>
    <span>Slides (PDF)</span>
  </a>

  <a href="https://gitcgr.hanyang.ac.kr/publications/2025-touchwalker/touchwalker-ismar-presentation.pptx" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="fa fa-file-powerpoint-o"></span>
    <span>Slides (PPTX)</span>
  </a>

</div>

<!--[Geuntae Park](../people/geuntae-park.html), [Jiwon Yi](../people/jiwon-yi.html), [Taehyun Rhee](https://findanexpert.unimelb.edu.au/profile/1084098-taehyun-rhee), [Kwanguk Kim](http://hcilab.dothome.co.kr/professor/166), [Yoonsang Lee](../people/yoonsang-lee.html)  -->
<!--To appear in 2025 IEEE International Symposium on Mixed and Augmented Reality (ISMAR 2025)-->

![teaser](../assets/publications/2025-touchwalker/teaser-touchwalker.png)  
*TouchWalker enables real-time control of full-body avatar locomotion using finger walking on a touchscreen. Users specify foot contacts within a touch region overlaid on the screen (bottom), and the system generates responsive full-body locomotion (top).*

## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="640" height="360" src="https://www.youtube.com/embed/RO8SRQUstoI" title="TouchWalker: Real-Time Avatar Locomotion from Touchscreen Finger Walking" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div></div>  
<br/>

## Abstract
 We present TouchWalker, a real-time system for controlling full-body avatar locomotion using finger-walking gestures on a touchscreen. The system comprises two main components: TouchWalker-MotionNet, a neural motion generator that synthesizes full-body avatar motion on a per-frame basis from temporally sparse two-finger input, and TouchWalker-UI, a compact touch interface that interprets user touch input to avatar-relative foot positions. Unlike prior systems that rely on symbolic gesture triggers or predefined motion sequences, TouchWalker uses its neural component to generate continuous, context-aware full-body motion on a per-frame basis—including airborne phases such as running, even without input during mid-air steps—enabling more expressive and immediate interaction. To ensure accurate alignment between finger contacts and avatar motion, it employs a MoE-GRU architecture with a dedicated foot-alignment loss. We evaluate TouchWalker in a user study comparing it to a virtual joystick baseline with predefined motion across diverse locomotion tasks. Results show that TouchWalker improves users’ sense of embodiment, enjoyment, and immersion.

## Paper
Publisher: [page](https://doi.ieeecomputersociety.org/10.1109/ISMAR67309.2025.00068)
\
arXiv: [page](https://arxiv.org/abs/2511.07860), [paper](https://arxiv.org/pdf/2511.07860)


## Presentation
ISMAR 2025 Presentation Slides: [pdf](https://gitcgr.hanyang.ac.kr/publications/2025-touchwalker/touchwalker-ismar-presentation.pdf) (2MB), [pptx](https://gitcgr.hanyang.ac.kr/publications/2025-touchwalker/touchwalker-ismar-presentation.pptx) (268.8MB)

