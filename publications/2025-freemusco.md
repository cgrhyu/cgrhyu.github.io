---
layout: publication_post
title: 'FreeMusco: Motion-Free Learning of Latent Control for Morphology-Adaptive Locomotion in Musculoskeletal Characters'
nav-menu: false
show_tile: false
---

<style>
:root {
  /* ===== 기본 배경 / 텍스트 ===== */
  --white: #ffffff;
  --black: #000000;
  --gray-bg: #f0f0f0;
  --gray-light: #e6e6e6;
  --gray-mid: #bfbfbf;
  --gray-dark: #666666;
  --text-primary: #222222;
  --text-secondary: #555555;

  /* ===== 주요 포인트 색상 ===== */
  --blue-accent: #1f77b4;   /* 주요 포인트 (ex: 제목, 링크) */
  --orange-accent: #ff7f0e; /* 보조 포인트 (ex: 강조 텍스트) */
  --green-accent: #2ca02c;  /* 긍정 / 성공 / OK */
  --red-accent: #d62728;    /* 경고 / 실패 */
  --purple-accent: #9467bd; /* 특별 강조 / 연구분류 구분 */
  --yellow-accent: #ffc107; /* 밝은 포인트 / 하이라이트 */

  /* ===== UI 요소 ===== */
  --border-color: #dddddd;
  --shadow-light: rgba(0, 0, 0, 0.08);
  --shadow-dark: rgba(0, 0, 0, 0.25);

  /* ===== 링크 / hover ===== */
  --link-color: var(--blue-accent);
  --link-hover: #004b87;
}

.fullwidth-section {
  background-color: var(--gray-bg);
  padding: 40px 20px;
  text-align: center;
  width: 100vw;
  margin-left: calc(50% - 50vw);
}

.fullwidth-section2 {
  background-color: var(--white);
  padding: 40px 20px;
  text-align: center;
  width: 100vw;
  margin-left: calc(50% - 50vw);
}

@media (max-width: 768px) {
  .fullwidth-section div[style*="grid-template-columns"] {
    grid-template-columns: 1fr !important;
  }
}

@media (max-width: 768px) {
  .fullwidth-section2 div[style*="grid-template-columns"] {
    grid-template-columns: 1fr !important;
  }
}

</style>

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

  <a href="https://arxiv.org/abs/2511.14205" rel="noopener noreferrer" target="_blank" class="button icon">
    <span class="ai ai-arxiv"></span>
    <span>arXiv </span> 
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
  <!--<a href="https://gitcgr.hanyang.ac.kr/publications/2025-b2f/18_B2F_End-to-End Body-to-Face Motion Generation with Style Reference.pdf" rel="noopener noreferrer" target="_blank" class="button icon">-->
    <span class="fa fa-file-pdf-o"></span>
    <span>Slides (PDF) (coming soon)</span>
  </a>

  <a href="" rel="noopener noreferrer" target="_blank" class="button icon">
  <!--<a href="https://gitcgr.hanyang.ac.kr/publications/2025-b2f/18_B2F_End-to-End Body-to-Face Motion Generation with Style Reference.pptx" rel="noopener noreferrer" target="_blank" class="button icon">-->
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

<!--
## Abstract
We propose FreeMusco, a motion-free framework that jointly learns latent representations and control policies for musculoskeletal characters. By leveraging the musculoskeletal model as a strong prior, our method enables energy-aware and morphology-adaptive locomotion to emerge without motion data. The framework generalizes across human, non-human, and synthetic morphologies, where distinct energy-efficient strategies naturally appear—for example, quadrupedal gaits in Chimanoid versus bipedal gaits in Humanoid. The latent space and corresponding control policy are constructed from scratch, without demonstration, and enable downstream tasks such as goal navigation and path following—representing, to our knowledge, the first motion-free method to provide such capabilities. FreeMusco learns diverse and physically plausible locomotion behaviors through model-based reinforcement learning, guided by the locomotion objective that combines control, balancing, and biomechanical terms. To better capture the periodic structure of natural gait, we introduce a temporally averaged loss formulation, which compares simulated and target states over a time window rather than on a per-frame basis. We further encourage behavioral diversity by randomizing target poses and energy levels during training, enabling locomotion to be flexibly modulated in both form and intensity at runtime. Together, these results demonstrate that versatile and adaptive locomotion control can emerge without motion capture, offering a new direction for simulating movement in characters where data collection is impractical or impossible.

## System Overview
![teaser](https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/fig_overview-v6.jpg)  
-->

<!--
<section class="fullwidth-section2">
  <h2>System Overview</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 16px; border-radius: 8px; background-color: #f9f9f9; text-align: left;">
      <h3 style="color: var(--black); margin-bottom: 12px; text-align: center;">Abstract</h3>
      <p style="font-size: 16px; line-height: 1.6;">
        We propose FreeMusco, a motion-free framework that jointly learns latent representations and control policies for musculoskeletal characters. By leveraging the musculoskeletal model as a strong prior, our method enables energy-aware and morphology-adaptive locomotion to emerge without motion data. The framework generalizes across human, non-human, and synthetic morphologies, where distinct energy-efficient strategies naturally appear—for example, quadrupedal gaits in Chimanoid versus bipedal gaits in Humanoid. The latent space and corresponding control policy are constructed from scratch, without demonstration, and enable downstream tasks such as goal navigation and path following—representing, to our knowledge, the first motion-free method to provide such capabilities. FreeMusco learns diverse and physically plausible locomotion behaviors through model-based reinforcement learning, guided by the locomotion objective that combines control, balancing, and biomechanical terms. To better capture the periodic structure of natural gait, we introduce a temporally averaged loss formulation, which compares simulated and target states over a time window rather than on a per-frame basis. We further encourage behavioral diversity by randomizing target poses and energy levels during training, enabling locomotion to be flexibly modulated in both form and intensity at runtime. Together, these results demonstrate that versatile and adaptive locomotion control can emerge without motion capture, offering a new direction for simulating movement in characters where data collection is impractical or impossible.
      </p>
    </div>
    <div style="display: flex; flex-direction: column; gap: 16px;">
      <div style="padding: 8px; border-radius: 8px; background-color: #f9f9f9;">
        <img src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/fig_overview-v6.jpg" 
             alt="System Overview" 
             style="width: 100%; border-radius: 8px;">
      </div>
      <div style="padding: 8px; border-radius: 8px; background-color: #f9f9f9;">
        <img src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/fig_loss-v1.jpg" 
             alt="Loss Formulation" 
             style="width: 100%; border-radius: 8px;">
      </div>
    </div>
  </div>
</section>
-->

<!-- test gif
<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 8px; text-align: center;">
  <div>
    <img src="../assets/publications/2025-freemusco/prediction.gif" width="100%" alt="Human"> 
    <p><small>Human</small></p> 
  </div>
  <div>
    <img src="../assets/publications/2025-freemusco/prediction.gif" width="100%" alt="Ostrich">
    <p><small>Ostrich</small></p>
  </div>
  <div>
    <img src="../assets/publications/2025-freemusco/prediction.gif" width="100%" alt="Chimanoid">
    <p><small>Chimanoid</small></p>
  </div>
</div>
-->
<!-- memo
<source src="../assets/publications/2025-freemusco/rev_ablation_ours_front_compressed.mp4" type="video/mp4">
<source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/ablation_updir_ours.mp4" type="video/mp4">
#1f77b4 light-blue #ff7f0e orange
-->

<!--
## Results
### Muscularskeletal Humanoid Locomotion

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 8px; text-align: center;">
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p><small>Velocity Only</small></p>
  </div>
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p><small>Velocity + Direction</small></p>
  </div>
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p><small>Velocity + Pose + Energy</small></p>
  </div>
</div>


### Morphology-Adaptive Locomotion

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 8px; text-align: center;">
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="color: #ff7f0e; font-weight: bold; font-size: 20px; margin-top: 4px;"> Velocity & Direction </p>
  </div>
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="color: #ff7f0e; font-weight: bold; font-size: 20px; margin-top: 4px;"> Velocity & Direction </p>
  </div>
  <div>
    <video width="100%" controls loop muted autoplay>
      <source src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="color: #ff7f0e; font-weight: bold; font-size: 20px; margin-top: 4px;"> Velocity & Direction </p>
  </div>
</div>
-->

<section class="fullwidth-section">
  <h2>Humanoid Locomotion</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/DtPPea1EODw?autoplay=1&mute=1&loop=1&playlist=DtPPea1EODw" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Goal Velocity-Only
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/H1zTPru_yPY?autoplay=1&mute=1&loop=1&playlist=H1zTPru_yPY" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Goal Velocity + Direction
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/jFX2WJysYac?autoplay=1&mute=1&loop=1&playlist=jFX2WJysYac"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Goal Velocity + Energy + Pose (symmetric)
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/-yUyC-40AHE?autoplay=1&mute=1&loop=1&playlist=-yUyC-40AHE"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Goal Velocity + Energy + Pose (asymmetirc)
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section2">
  <h2>Morphology-Adaptive Locomotion</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/vFqhSliXM24?autoplay=1&mute=1&loop=1&playlist=vFqhSliXM24" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Chimanoid: Goal Velocity-Only
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/3SS7apL1dWQ?autoplay=1&mute=1&loop=1&playlist=3SS7apL1dWQ" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media" 
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Ostrich: Goal Velocity-Only
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/lvtsGscn2Hc?autoplay=1&mute=1&loop=1&playlist=lvtsGscn2Hc"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Ostrich: Goal Velocity + Pose + Energy
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section">
  <h2>Emergent Gait Strategies Across Morphologies</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/0kecrXYtuWU?autoplay=1&mute=1&loop=1&playlist=0kecrXYtuWU" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Chimanoid: Goal Velocity + Energy
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/dUMsO8iHufA?autoplay=1&mute=1&loop=1&playlist=dUMsO8iHufA" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;"> 
        Humanoid: Goal Velocity + Energy
      </p>
    </div>
    <div style="
        grid-column: 1 / -1;
        background-color: #f9f9f9;
        padding: 16px 20px;
        border-radius: 12px;
        border: 1px solid #e0e0e0;
        margin-top: 8px;
        text-align: center;
      ">
      <p style="font-size: 16px; line-height: 1.6; margin: 0; text-align: left; ">
        If initialized in a bipedal pose, Chimanoid walks bipedally at high energy but shifts to a quadrupedal gait as energy decreases. 
        And when the energy is raised again, it does not return to bipedal walking but instead exhibits a stronger qudarupedal gait,
        indiciating quadrupedal motion is more efficient for its body. Humanoid, however, never adopts quadrupedal gaits—showing
        that energy-efficient strategies depend on morphology and can naturally emerge in our motion-free framework.
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section2">
  <h2>Unconditional Random Sampling in Latent Space</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/T9i6hZIwuRY?autoplay=1&mute=1&loop=1&playlist=T9i6hZIwuRY" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Humanoid Latent Space <br> Trained with Velocity-Only Goals
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/h4vRzwobSuk?autoplay=1&mute=1&loop=1&playlist=h4vRzwobSuk"   
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Humanoid Latent Space <br> Trained with Velocity + Pose + Energy Goals
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/t8F7GiGLYlo?autoplay=1&mute=1&loop=1&playlist=t8F7GiGLYlo"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Chimanoid Latent Space <br> Trained with Velocity-Only Goals
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/61gtTT5rC5A?autoplay=1&mute=1&loop=1&playlist=61gtTT5rC5A"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Ostrich Latent Space <br> Trained with Velocity + Pose + Energy Goals
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section">
  <h2>Downstream Tasks: Point-Goal Navigation</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/5TBRc0ojVas?autoplay=1&mute=1&loop=1&playlist=5TBRc0ojVas"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Humanoid
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/4-67VchDw1E?autoplay=1&mute=1&loop=1&playlist=4-67VchDw1E"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Chimanoid
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/dX-QdRzvEtY?autoplay=1&mute=1&loop=1&playlist=dX-QdRzvEtY" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Ostrich
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section2">
  <h2>Downstream Tasks: Path Following</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/QH8ilQQaTRw?autoplay=1&mute=1&loop=1&playlist=QH8ilQQaTRw" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Humanoid
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;"> 
        <iframe
          src="https://www.youtube.com/embed/uWwg47TXzjs?autoplay=1&mute=1&loop=1&playlist=uWwg47TXzjs" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Chimanoid
      </p>
    </div>
  </div>
</section>


<section class="fullwidth-section">
  <h2>Method </h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <img src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/fig_overview-v6.jpg"
           alt="Overview"
           style="width: 100%; border-radius: 8px;">
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        System Overview
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <img src="https://gitcgr.hanyang.ac.kr/publications/2025-freemusco/fig_loss-v1.jpg"
           alt="Loss"
           style="width: 100%; border-radius: 8px;">
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Locomotion Objective Loss
      </p>
    </div>
    <div style="
        grid-column: 1 / -1;
        background-color: #f9f9f9;
        padding: 16px 20px;
        border-radius: 12px;
        border: 1px solid #e0e0e0;
        margin-top: 8px; 
        text-align: center;
      ">
      <p style="font-size: 16px; line-height: 1.6; margin: 0; text-align: left; ">
        FreeMusco builds on conditional VAE and model-based RL, guided by the locomotion objective loss with temporally averaged terms, to learn
        energy-aware latent locomotion directly from muscle dynamics and goal signals without motion data.
      </p>
    </div>
  </div>
</section>



<section class="fullwidth-section2">
  <h2>Effect of Temporally Averaged Loss Formulation</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/miqnPb9hEEE?autoplay=1&mute=1&loop=1&playlist=miqnPb9hEEE" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Temporally-averaged L<sub>pose</sub> (Ours)
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/nQd02C6xftA?autoplay=1&mute=1&loop=1&playlist=nQd02C6xftA" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Per-step L<sub>pose</sub>
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/Mn6ZEFCjtZE?autoplay=1&mute=1&loop=1&playlist=Mn6ZEFCjtZE" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Temporally-averaged L<sub>up</sub> (Ours)
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/SoFYlazzQdM?autoplay=1&mute=1&loop=1&playlist=SoFYlazzQdM"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Per-step L<sub>up</sub>
      </p>
    </div>
    <div style="
        grid-column: 1 / -1;
        background-color: #f9f9f9;
        padding: 16px 20px;
        border-radius: 12px;
        border: 1px solid #e0e0e0;
        margin-top: 8px;
        text-align: center;
      ">
      <p style="font-size: 16px; line-height: 1.6; margin: 0; text-align: left; ">
        (1) Per-step enforces rigid frame-level pose matching, leading to slightly crouched, short-stepped gait with suppressed pelvic rotation.
        <br> (2) Per-step strongly constrains pelvic dynamics, so pelvic rotation appears nearly rigid without natural oscillatory components.
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section">
  <h2>Comparison with Torque-Actuated Humanoid</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/5MfxHva0FCg?autoplay=1&mute=1&loop=1&playlist=5MfxHva0FCg"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Muscle-Actuated (Ours)
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/XTT0r_96Xik?autoplay=1&mute=1&loop=1&playlist=XTT0r_96Xik" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Torque-Actuated 
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/A1iyknW-Y4s?autoplay=1&mute=1&loop=1&playlist=A1iyknW-Y4s"  
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Torque-Actuated <br>(with manually tuned torque limits)
      </p>
    </div>
    <div style="
        grid-column: 1 / -1;
        background-color: #f9f9f9;
        padding: 16px 20px;
        border-radius: 12px;
        border: 1px solid #e0e0e0;
        margin-top: 8px;
        text-align: center;
      ">
      <p style="font-size: 16px; line-height: 1.6; margin: 0; text-align: left; ">
        Torque-actuated humanoid failed to learn even basic balanced walking behavior. Even with
        manual tuning of joint torque limits, it only learned a very short-stepped, high-frequency locomotion.
      </p>
    </div>
  </div>
</section>

<section class="fullwidth-section2">
  <h2>Discussion</h2>
  <div style="display: grid; grid-template-columns: 1fr 1fr ; gap: 16px; max-width: 1200px; margin: auto;">
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/5MfxHva0FCg?autoplay=1&mute=1&loop=1&playlist=5MfxHva0FCg"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Target Pose: <br>Standing pose with straight arms 
      </p>
    </div>
    <div style="padding: 8px; border-radius: 8px;">
      <div style="position: relative; width: 100%; padding-top: 56.25%;">
        <iframe
          src="https://www.youtube.com/embed/PWkwiGMc0sw?autoplay=1&mute=1&loop=1&playlist=PWkwiGMc0sw"
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
          frameborder="0"
          allow="autoplay; encrypted-media"
          allowfullscreen>
        </iframe>
      </div>
      <p style="color: var(--black); font-weight: bold; font-size: 20px; margin-top: 4px;">
        Target Pose: <br>Standing pose with slightly bent elbows 
      </p>
    </div>
    <div style="
        grid-column: 1 / -1;
        background-color: #f9f9f9;
        padding: 16px 20px;
        border-radius: 12px;
        border: 1px solid #e0e0e0;
        margin-top: 8px;
        text-align: center;
      ">
      <p style="font-size: 16px; line-height: 1.6; margin: 0; text-align: left; ">
        Learning with target poses featuring slightly bent elbows mitigates the straight and stiff arm artifact, suggesting
        that searching for optimal target poses would be a valuable direction for future work.
      </p>
    </div>
  </div>
</section>
<div style="grid-column: 1 / -1;">
  <hr style="border: none; height: 2px; background-color: #333; width: 100%; display: block; margin: 32px 0;">
</div>

## Abstract
We propose FreeMusco, a motion-free framework that jointly learns latent representations and control policies for musculoskeletal characters. By leveraging the musculoskeletal model as a strong prior, our method enables energy-aware and morphology-adaptive locomotion to emerge without motion data. The framework generalizes across human, non-human, and synthetic morphologies, where distinct energy-efficient strategies naturally appear—for example, quadrupedal gaits in Chimanoid versus bipedal gaits in Humanoid. The latent space and corresponding control policy are constructed from scratch, without demonstration, and enable downstream tasks such as goal navigation and path following—representing, to our knowledge, the first motion-free method to provide such capabilities. FreeMusco learns diverse and physically plausible locomotion behaviors through model-based reinforcement learning, guided by the locomotion objective that combines control, balancing, and biomechanical terms. To better capture the periodic structure of natural gait, we introduce a temporally averaged loss formulation, which compares simulated and target states over a time window rather than on a per-frame basis. We further encourage behavioral diversity by randomizing target poses and energy levels during training, enabling locomotion to be flexibly modulated in both form and intensity at runtime. Together, these results demonstrate that versatile and adaptive locomotion control can emerge without motion capture, offering a new direction for simulating movement in characters where data collection is impractical or impossible.


## Video 
<div id="iframe_container"> <div id="iframe">
<iframe width="1198" height="674" src="https://www.youtube.com/embed/YFNKLzUQ0zk" title="FreeMusco: Motion-Free Learning of Latent Control for Morphology-Adaptive Locomotion in Musculoske.." frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div></div>  
<br/>

## Paper
Publisher: Coming soon  
<!--Publisher: [page](https://dl.acm.org/doi/10.1145/3731425), [paper](https://dl.acm.org/doi/pdf/10.1145/3731425)\-->
arXiv: [page](https://arxiv.org/abs/2511.14205), [paper](https://arxiv.org/pdf/2511.14205)
<!--arXiv: Coming soon-->



<!--## Presentation & Poster-->
<!--SIGGRAPH 2025 Technical Papers Presentation Slides: [pdf](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-siggraph-presentation.pdf) (3.5MB), [pptx](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-siggraph-presentation.pptx) (369.7MB)  -->
<!--SIGGRAPH 2025 Emerging Technologies & Interactive Discussion Poster: [pdf](https://gitcgr.hanyang.ac.kr/publications/2025-physicsfc/physicsfc-etech-intdis-poster.pdf) (523KB)-->

