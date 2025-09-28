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

.about-inline .page__content{
  max-width: 1400px;      /* 글을 더 넓게 펼치기 */
  margin: 0 auto;
  padding: 0 1.5rem;
  font-family:'Inter',system-ui,-apple-system,'Segoe UI',Roboto,Arial,sans-serif;
  color:#333; font-weight:300; line-height:1.65;
}

/* 2) 이미지가 글 속에 '짧게' 떠 있게 */
.intro__img{
  float: left;                 /* 핵심: 오른쪽→아래로 글이 흘러감 */
  width: 240px;                /* 필요시 220~280 조절 */
  height: auto;
  border-radius: 12px;
  border: 1px solid var(--line);
  box-shadow: 0 6px 22px rgba(30,30,30,.06);
  margin: .2rem 1.5rem 1rem 0; /* 오른쪽/아래 여백 */
  display: block;
}

/* 3) float 정리: 이미지 높이 끝난 뒤 다음 섹션 겹침 방지 */
.intro::after{
  content: "";
  display: block;
  clear: both;
}

/* 4) 모바일에서는 안전하게 단일 열로 */
@media (max-width: 880px){
  .intro__img{
    float:none;
    margin: 0 auto 1rem;
    width: min(75%, 360px);
  }
}
/* 리스트 */
.aboutme ul{padding-left:1.25rem;margin-top:.75rem}
.aboutme li{margin:.6rem 0}

/* 링크 */
a{color:var(--brand);text-decoration:none}
a:hover{text-decoration:underline}

/* 모바일: 이미지 위, 본문 아래(가독성) */
@media (max-width: 880px){
  .intro__img{
    float:none;
    margin:0 auto 1rem;
    width: min(70%, 360px);   /* 화면에 맞게 자동 축소 */
  }
}
</style>

<div class="intro">
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Portrait">

  <h1 class="intro__title">Yeonju Lee</h1>
  <div class="intro__lead">
    I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at
    <strong>Georgia Tech</strong>, advised by <a href="https://sites.gatech.edu/jing-li/">Prof. Jing Li</a>.
  </div>
    <div class="aboutme">
      <p>
        My research focuses on <strong style="color:var(--brand)">knowledge-informed machine learning</strong>—developing methods that incorporate domain expertise to make models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>.
      </p>

      <h3>Why</h3>
      <p>
        Real-world data often suffers from <strong>scarcity</strong>, <strong>heterogeneity</strong>, and <strong>high dimensionality</strong>, making it difficult for purely data-driven models to generalize. Incorporating domain knowledge helps overcome these challenges, yielding models that are not only accurate but also aligned with expert reasoning.
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
        My work applies these ideas to domains like <strong style="color:#4169E1;">healthcare</strong>, <strong style="color:#4169E1;">precision agriculture</strong>, and <strong style="color:#4169E1;">manufacturing</strong>.
      </p>

      <p>
        Outside research, I enjoy playing racquetball 🎾, knitting 🧶, and running 🏃‍♀️. If you'd like to connect: <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>.
      </p>
    </div>
  </div>
</div>
