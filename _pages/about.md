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
  max-width: 100% !important;      /* 필요시 1100~1320 조절 */
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

/* --- Intro: photo | text(right-top-aligned) -> full-width sections --- */
.intro{
  display:grid !important;
  grid-template-columns: 260px minmax(0,1fr);
  grid-template-areas:
    "photo title"
    "photo lead"
    "photo about"
    "full  full";
  column-gap: 1.75rem;
  row-gap: .75rem;
  align-items:start;
  margin: 1.2rem 0 1.8rem;
}

.intro__img{
  grid-area: photo;
  width:260px; height:auto;
  border-radius:14px;
  border:1px solid var(--line);
  box-shadow:0 6px 22px rgba(30,30,30,.06);
}

.intro__body{ display: contents; }

.intro__title{ grid-area: title; margin:0 0 .4rem; font-size:2rem; font-weight:700; color:#111; }
.intro__lead { grid-area: lead;  margin:0 0 1rem; font-size:1.02rem; color:#2f2f2f; }
.aboutme      { grid-area: about; }
.about-sections{ grid-area: full; margin-top:.2rem; }

.page__content,
.page__inner-wrap,
.wrapper,
.container {
  max-width: 100% !important;
  width: 100% !important;
}

@media (max-width:880px){
  .intro{
    grid-template-columns:1fr;
    grid-template-areas:
      "photo"
      "title"
      "lead"
      "about"
      "full";
  }
  .intro__img{ width:90%; justify-self:center; }
}

.about-sections h3 {
  margin-top: 0.8rem;   /* 위쪽 간격 줄이기 */
  margin-bottom: 0.3rem; /* 아래쪽 간격 줄이기 */
}

.about-sections p {
  margin-top: 0;
  margin-bottom: 0.6rem;
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
      Hello! Thank you for stopping by.
      I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at
      <strong>Georgia Tech</strong>, advised by <a href="https://sites.gatech.edu/jing-li/">Prof. Jing Li</a>.
    </div>

    <div class="aboutme">
      <p>
        My research focuses on <strong style="color:var(--brand)">knowledge-informed machine learning</strong>—developing methods that incorporate domain expertise to make models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>. If you would like to connect, feel free to email via ylee845@gatech.edu.
      </p>
    </div>

    <div class="about-sections">
      <h3>Why</h3>
      <p> Real-world data often suffers from <strong>scarcity</strong>, <strong>heterogeneity</strong>, and <strong>high dimensionality</strong>, making it difficult for purely data-driven models to generalize. </p>
      <h3>Where</h3>
      <ul> 
      <li><strong>Input level</strong> – infuse knowledge into what the model sees.</li> 
      <li><strong>Architecture level</strong> – embed knowledge into network design or loss function.</li> 
      <li><strong>Inference level</strong> – guide model reasoning during inference.</li>
      </ul>
      <h3>How</h3>
      <ul> 
      <li><strong>Representations</strong> – encoding qualitative knowledge into quantitative representations.</li> 
      <li><strong>Constraints</strong> – enforcing biologically or physically valid conditions.</li>
      <li><strong>Rules</strong> – applying domain heuristics to refine inference.</li>
      </ul>
    </div>
  </div>
</div>
