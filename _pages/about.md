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
  /*text-align: justify;*/
  margin: 0 auto;
  width: 100% !important;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color:#333; font-weight:300; line-height:1.45;
}

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
  margin: 1.2rem 0 0.5rem;
  align-items:start;
}

.intro__img{
  grid-area: photo;
  width: 100%;
  border-radius: 0;
  object-fit: cover;
}

.intro__body {
  font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
  font-size: 1rem;          /* 살짝 작게 (기존 1rem → 0.98rem) */
  line-height: 1.65;           /* 줄 간격 약간 촘촘하게 */
  letter-spacing: -0.1px;      /* 살짝 좁혀서 정돈된 느낌 */
  color: var(--text);
  max-width: 600px;
  /*text-align: justify;*/
}

.intro__body,
.about-sections p,
.about-sections li {
  font-family: "Inter", "Helvetica Neue", Arial, sans-serif;
  font-size: 1rem;
  line-height: 1.65;
  letter-spacing: -0.1px;
  color: var(--text);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}
  
.intro__title{ grid-area:title; margin:0 0 .4rem; font-size:2rem; font-weight:700; color:#111; }
.intro__lead { grid-area:lead;  margin:0 0 .6rem; font-size:1rem; color:#2f2f2f; }
.aboutme     { grid-area:about; font-size:1rem; margin-top:.1rem; }
.about-sections{ grid-area:full; margin-top:.15rem; font-size:1rem; }

.intro__title,
.intro__lead,
.aboutme,
.about-sections {
  /*text-align: justify;*/     /* 기본 정렬로 되돌림 (보통 왼쪽) */
}

/* 반응형: 1열 스택 */

@media (max-width:1024px){  /* 기존 880px → 1024px 로 확장 */
  .intro{
    grid-template-columns:1fr;
    grid-template-areas:
      "photo"
      "title"
      "lead"
      "about"
      "full";
    text-align: unset !important;
  }
  .intro__img{
    width:95%;
    justify-self:center;
  }
  .intro,
  .intro__lead,
  .aboutme,
  .about-sections{
    text-align: unset !important;
    font-weight: 500; /* 기본 700일 경우 중간 정도로 낮춰줌 */
    -webkit-font-smoothing: antialiased; /* 크롬, 사파리에서 부드럽게 */
    -moz-osx-font-smoothing: grayscale;  /* 파이어폭스용 */
    text-rendering: optimizeLegibility;  /* 렌더링 품질 개선 */
  }
}

.about-sections h3 {
  margin-top: 0.1rem;   /* 위쪽 간격 줄이기 */
  margin-bottom: 0.2rem; /* 아래쪽 간격 줄이기 */
  font-weight: 700;
  font-size: 1.05rem;
}

h4 {
  color: #3A5F91;        /* 진회색 555 */
  font-weight: 650;     /* 볼드 강조 500 */
  font-size: 1rem;    /* 약간 크게 */
  letter-spacing: 0.2px;
  margin-top: 1.2rem;
  margin-bottom: 0.4rem;
  line-height: 1.3;
}

.about-sections p {
  margin-top: 0;
  margin-bottom: 0;
  line-height: 1.65;           /* 줄 간격 약간 촘촘하게 */
  letter-spacing: -0.1px;
  font-size: 1rem; 
}

.about-sections ul {
  margin-top: 0.3rem;
  margin-bottom: 0.8rem; /* 리스트와 다음 섹션 간격 살짝만 */
  font-size: 1rem; 
}

.about-sections li {
  margin-bottom: 0.2rem; /* 리스트 내부 항목 간 간격 */
}
  
</style>

<div class="intro">
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Yeonju Lee Portrait">

  <div class="intro__body">
    <h2 class="intro__title">Yeonju Lee</h2>

    <p>
      Hello! I’m a Ph.D. student in the 
      <span style="font-weight:600; letter-spacing:0.2px;"> H. Milton Stewart School of Industrial & Systems Engineering</span> at 
      <span style="font-weight:600; letter-spacing:0.2px;">Georgia Tech</span>, advised by 
      <a href="https://isye.gatech.edu/users/jing-li" target="_blank">Dr. Jing Li</a>.
    </p>

    <p>
      My research focuses on 
    <span style="color:#3A5F91; font-weight:600; letter-spacing:0.2px;">
      knowledge-informed machine learning (ML)
    </span>,
    developing models that integrate domain knowledge to build more 
    data-efficient, robust, and interpretable systems. 
    Please feel free to contact me at 
    <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>. 
    <br>
    <a href="/files/Yeonju_Lee_CV.pdf" style="color:#3A5F91;">CV</a> (Updated Oct 2025)
     &nbsp;|&nbsp;
    <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" 
     target="_blank" 
     style="color:#3A5F91;">
     Google Scholar
    </a> 
    </p>
  </div>
</div>

<hr>
<section class="about-sections">
  <h3>Knowledge-Informed ML: <span class="accent">Why, Where, and How</span></h3>
  <hr class="section-divider" style="margin-top:0.8rem; margin-bottom:0.8rem;">

<h4>Why Knowledge-Informed ML?</h4>
<p>
Real-world data often suffers from <span style="font-weight:550; letter-spacing:0.2px;">scarcity</span>, <span style="font-weight:550; letter-spacing:0.2px;">heterogeneity</span>, 
and <span style="font-weight:550; letter-spacing:0.2px;">high dimensionality</span>, making it difficult for purely data-driven models to generalize. 
Knowledge-informed ML integrates domain understanding to enhance robustness and interpretability.
</p>

<h4>Where to Inform?</h4>
<p>
At the <span style="font-weight:550; letter-spacing:0.2px;">input</span>, <span style="font-weight:550; letter-spacing:0.2px;">architecture</span>, and <span style="font-weight:550; letter-spacing:0.2px;">inference</span> levels — 
where domain knowledge can guide representation, structure, and decision-making.
</p>

<h4>How to Inform?</h4>
<p>
Through <span style="font-weight:550; letter-spacing:0.2px;">representations</span>, <span style="font-weight:550; letter-spacing:0.2px;">constraints</span>, and <span style="font-weight:550; letter-spacing:0.2px;">rules</span> — 
translating expert understanding into model priors and learning objectives.
</p>

<h4>Applications</h4>
<ul>
  <li><span style="font-weight:550; letter-spacing:0.2px;">Healthcare</span> – dental lesion detection and medical image translation</li>
  <li><span style="font-weight:550; letter-spacing:0.2px;">Precision Agriculture</span> – yield forecasting, anomaly detection, and change-point detection</li>
  <li><span style="font-weight:550; letter-spacing:0.2px;">Manufacturing</span> – root cause analysis and process optimization</li>
</ul>

  <p>
    For more details, please refer to the <a href="/publications">Publications</a> section.
  </p>
</section>
