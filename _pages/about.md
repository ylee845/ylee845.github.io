---
permalink: /
layout: single
author_profile: false
#classes: about-inline
sidebar: false      # ← 사이드바 완전 비활성
toc: false
classes: wide       # ← 본문을 넓게(가로폭 회수)
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
  max-width: none; !important;      /* 필요시 1100~1320 조절 */
  margin: 0 auto;
  width: 100% !important;            /* ← 180% 제거 */
  #padding: 0 .75rem !important;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color: #333;
  font-weight: 300;
  line-height: 1.45;                 /* 줄간격 적당히 타이트 */
}

.sidebar, .page__sidebar {display:none !important;}
.page__content {float:none !important; width:100% !important;}
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap');

:root{
  --brand:#3b5bdb;
  --line:#e9e9ee;
  --sidebar-w: 280px;
}

/* 사이드바 끄고 본문을 100%로 */
.sidebar, .page__sidebar { display:none !important; }
.page__content { float:none !important; width:100% !important; }

/* 페이지 기본 타이포 */
.page__content {
  max-width: none !important;
  margin: 0 auto;
  width: 100% !important;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color:#333; font-weight:300; line-height:1.45;
}

/* Intro: 사진 | 텍스트 2열 */
.intro{
  display:grid !important;
  grid-template-columns: 280px 1fr;           /* ← 2열 */
  grid-template-areas:
    "photo title"
    "photo lead"
    "photo about"
    "full  full";
  column-gap: 1.25rem;
  row-gap: .6rem;
  margin: 1.2rem 0 1.8rem;
  align-items:start;
}

.intro__img{
  grid-area: photo;
  width: 100%;
  border-radius: 0;
  object-fit: cover;
}

.intro__body{ display: contents; }
.intro__title{ grid-area:title; margin:0 0 .4rem; font-size:2rem; font-weight:700; color:#111; }
.intro__lead { grid-area:lead;  margin:0 0 .6rem; font-size:1rem; color:#2f2f2f; }
.aboutme     { grid-area:about; font-size:1rem; margin-top:.1rem; }
.about-sections{ grid-area:full; margin-top:.15rem; font-size:1rem; }

/* 반응형: 1열 스택 */
@media (max-width:880px){
  .intro{
    grid-template-columns:1fr;
    grid-template-areas:
      "photo" "title" "lead" "about" "full";
  }
  .intro__img{ width:90%; justify-self:center; }
}
.about-sections h3 {
  margin-top: 0.8rem;   /* 위쪽 간격 줄이기 */
  margin-bottom: 0.3rem; /* 아래쪽 간격 줄이기 */
}

.about-sections p {
  margin-top: 0;
  margin-bottom: 0.3rem;
}

.about-sections ul {
  margin-top: 0.3rem;
  margin-bottom: 0.8rem; /* 리스트와 다음 섹션 간격 살짝만 */
}

.about-sections li {
  margin-bottom: 0.2rem; /* 리스트 내부 항목 간 간격 */
}
  
</style>

<div class="intro">
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Portrait">

  <div class="intro__body">
    <h1 class="intro__title">Yeonju Lee</h1>
    <div class="intro__lead">
      Hello! Thank you for stopping by. <br>
      I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at
      Georgia Institute of Technology, advised by <a href="https://sites.gatech.edu/jing-li/">Prof. Jing Li</a>.
    </div>

<div class="aboutme">
  <p>
    My research focuses on <strong style="color:var(--brand)">knowledge-informed machine learning (ML)</strong>—developing methods that incorporate domain expertise to make ML models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>. 
    If you’d like to connect, feel free to reach out at <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>.
  </p>
</div>

<div class="about-sections" style="max-width:75ch; margin:auto; line-height:1.65; font-family:'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif; color:#333;">
  <hr style="border:none; border-top:1px solid #e5e5e5; margin:2.2rem 0 1.5rem; width:85%;">
  <h3 style="font-size:1.4rem; font-weight:650; color:#222; margin-bottom:1rem;">
    Knowledge-Informed ML: Why, Where, and How
  </h3>

  <h4 style="font-size:1.05rem; font-weight:550; margin-top:1.2rem;">Why</h4>
  <p style="margin-top:.4rem;">
    Real-world data often suffers from 
    <span style="font-weight:520;">scarcity</span>, 
    <span style="font-weight:520;">heterogeneity</span>, and 
    <span style="font-weight:520;">high dimensionality</span>, 
    making it difficult for purely data-driven models to generalize well.
  </p>

  <h4 style="font-size:1.05rem; font-weight:550; margin-top:1.4rem;">Where</h4>
  <ul style="margin-top:.3rem; margin-left:0.8rem;">
    <li><span style="font-weight:520;">Input level</span> – deliberately refine model inputs using domain knowledge.</li>
    <li><span style="font-weight:520;">Architecture level</span> – embed knowledge into network design or loss function.</li>
    <li><span style="font-weight:520;">Inference level</span> – guide model reasoning during inference.</li>
  </ul>

  <h4 style="font-size:1.05rem; font-weight:550; margin-top:1.4rem;">How</h4>
  <ul style="margin-top:.3rem; margin-left:0.8rem;">
    <li><span style="font-weight:520;">Representations</span> – encode qualitative knowledge into quantitative representations.</li>
    <li><span style="font-weight:520;">Constraints</span> – enforce biologically or physically valid conditions.</li>
    <li><span style="font-weight:520;">Rules</span> – formalize domain knowledge as rule-based guidance.</li>
  </ul>
</div>
