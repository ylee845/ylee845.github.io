---
permalink: /
layout: single
author_profile: false
classes: about-inline
redirect_from: 
  - /about/
  - /about.html
---
<!-- About hero: 사진 왼쪽, 텍스트 오른쪽 (깔끔·세련) -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap');

:root{
  --brand:#3b5bdb;
  --line:#e9e9ee;
}

/* 페이지 폭 정상화 (가로 스크롤/튐 방지) */
.about-inline .page__content {
  max-width: 1200px !important;      /* 필요시 1100~1320 조절 */
  margin: 0 auto;
  width: 100% !important;            /* ← 180% 제거 */
  #padding: 0 .75rem !important;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color: #333;
  font-weight: 300;
  line-height: 1.45;                 /* 줄간격 적당히 타이트 */
}

.sidebar, .page__sidebar { display:none !important; }
.page__content { float:none !important; width:100% !important; }

/* ✅ 사진 왼쪽 / 텍스트 오른쪽: grid 레이아웃 */
/* ===== Layout: photo + intro copy side-by-side, then full-width sections ===== */

/* container width */
.about-inline .page__content{
  max-width: 1400px;
  margin: 0 auto;
  padding: 0 1.25rem;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color:#333; font-weight:300; line-height:1.65;
}

/* intro grid */
.intro{
  display: grid !important;
  grid-template-columns: 260px minmax(0,1fr); /* photo | text */
  column-gap: 1.75rem;
  row-gap: 0.9rem;
  align-items: start;
  margin: 1.2rem 0 1.8rem;
}

/* photo */
.intro__img{
  grid-column: 1;
  width: 260px; height:auto;
  border-radius: 14px;
  border: 1px solid var(--line);
  box-shadow: 0 6px 22px rgba(30,30,30,.06);
}

/* let children of .intro__body become grid items of .intro */
.intro__body{ display: contents; }

/* items that should sit to the RIGHT of the photo */
.intro__title,
.intro__lead,
.aboutme{
  grid-column: 2;
}

/* items that should span FULL WIDTH below the photo */
.about-sections{
  grid-column: 1 / -1;     /* <-- full width */
  margin-top: .25rem;
}

/* typography */
.intro__title{ font-size:2rem; margin:0 0 .4rem; font-weight:700; color:#111 }
.intro__lead{ margin:0 0 1rem; font-size:1.02rem; color:#2f2f2f }
.aboutme ul{ padding-left:1.25rem; margin-top:.75rem }
.aboutme li{ margin:.6rem 0 }

/* mobile: single column */
@media (max-width: 880px){
  .intro{
    grid-template-columns: 1fr;
  }
  .intro__img{
    grid-column: 1; justify-self: center;
    width: min(75%, 360px);
  }
  .intro__title,
  .intro__lead,
  .aboutme,
  .about-sections{
    grid-column: 1;
  }
}

</style>

<div class="intro">
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Portrait">
  <div class="intro__body">
    <h1 class="intro__title">Yeonju Lee</h1>
    <div class="intro__lead">
      I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at
      <strong>Georgia Tech</strong>, advised by <a href="https://sites.gatech.edu/jing-li/">Prof. Jing Li</a>.
    </div>

    <div class="aboutme">
      <p>
        My research focuses on <strong style="color:var(--brand)">knowledge-informed machine learning</strong>—developing methods that incorporate domain expertise to make models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>.
      </p>

  <section class="about-sections">
  <h3>Why</h3>
  <p>
    Real-world data often suffers from <strong>scarcity</strong>, <strong>heterogeneity</strong>,
    and <strong>high dimensionality</strong>, making it difficult for purely data-driven models to generalize…
  </p>

  <h3>Where</h3>
  <ul>
    <li><strong>Representation level</strong> – encoding qualitative knowledge into quantitative representations.</li>
    <li><strong>Architecture level</strong> – embedding knowledge into network design or loss function.</li>
    <li><strong>Inference level</strong> – guiding model reasoning with explicit rules during inference.</li>
  </ul>

  <h3>How</h3>
  <ul>
    <li><strong>Representations</strong> – transforming expert concepts into measurable features.</li>
    <li><strong>Constraints</strong> – enforcing biologically or physically valid conditions.</li>
    <li><strong>Rules</strong> – applying domain heuristics to refine inference.</li>
  </ul>

  <p>
    My work applies these ideas to domains like <strong style="color:#4169E1;">healthcare</strong>,
    <strong style="color:#4169E1;">precision agriculture</strong>, and <strong style="color:#4169E1;">manufacturing</strong>.
  </p>

  <p>
    Outside research, I enjoy playing racquetball 🎾, knitting 🧶, and running 🏃‍♀️.
    If you'd like to connect: <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>.
  </p>
</section>
