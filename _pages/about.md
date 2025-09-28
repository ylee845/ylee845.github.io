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
/* 로컬/임포트 폰트 (구글폰트) */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap');

:root{
  --brand:#3b5bdb;
  --line:#e9e9ee;
}

/* 페이지 전용 래퍼 */
.about-inline .page__content {
  max-width:1200px;   /* 더 넓게 쓰되 너무 길지 않게 */
  margin: 0 auto;
  padding: 0 1.25rem;
  font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, Arial, sans-serif;
  color: #333;
  font-weight: 300;
  line-height: 1.65;
}

/* 사이드바 완전 제거 (보험용) */
.sidebar, .page__sidebar { display:none !important; }
.page__content { float:none !important; width:100% !important; }

/* 히어로 레이아웃 */
.intro {
  display:flex;
  align-items:flex-start;   /* 텍스트 상단 정렬 */
  gap: 2.25rem;
  margin: 1.5rem 0 2.25rem;
}

/* 이미지: 작게, 둥글고 그림자 */
.intro__img {
  width: 240px;            /* 부담 덜한 크기 (조정: 220/240/260) */
  height: auto;
  border-radius: 14px;
  border: 1px solid var(--line);
  box-shadow: 0 6px 22px rgba(30,30,30,0.06);
  flex-shrink: 0;
}

/* 텍스트 영역 */
.intro__body {
  flex: 1;
  font-size: 1.02rem;
  color: #2f2f2f;
}
.intro__title {
  font-size: 2.0rem;
  margin: 0 0 .4rem;
  font-weight: 700;
  color: #111;
}
.intro__lead { margin: 0 0 1rem; }

/* 리스트 스타일 정리 */
.aboutme ul { padding-left: 1.25rem; margin-top: .75rem; }
.aboutme li { margin: .6rem 0; }

/* 링크 색상 */
a { color: var(--brand); text-decoration: none; }
a:hover { text-decoration: underline; }

/* 반응형: 모바일에서 이미지 위로 */
@media (max-width: 880px) {
  .intro { flex-direction: column; gap:1rem; }
  .intro__img { width: 100%; max-width: 420px; align-self: center; }
  .about-inline .page__content { padding: 0 1rem; }
}
</style>

<div class="intro">
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Portrait">
  <div class="intro__body">
    <h1 class="intro__title">Yeonju Lee</h1>
    <div class="intro__lead">
      I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at
      <strong>Georgia Tech</strong>, advised by <a href="mailto:jing.li@gatech.edu">Prof. Jing Li</a>.
    </div>

    <div class="aboutme">
      <p>
        My research focuses on <strong style="color:var(--brand)">knowledge-informed machine learning</strong>—developing methods that incorporate domain expertise to make models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>.
      </p>

      <ul>
        <li><strong>Representation level</strong> – encoding qualitative knowledge into quantitative representations.</li>
        <li><strong>Architecture level</strong> – embedding knowledge into network design or loss function.</li>
        <li><strong>Inference level</strong> – guiding model reasoning with explicit rules during inference.</li>
      </ul>

      <p>
        These strategies are particularly relevant under <em>real-world data challenges</em> such as <strong>scarcity</strong>, <strong>heterogeneity</strong>, and <strong>high dimensionality</strong>. My work applies these ideas to domains like <strong style="color:#4169E1;">healthcare</strong>, <strong style="color:#4169E1;">precision agriculture</strong>, and <strong style="color:#4169E1;">manufacturing</strong>.
      </p>

      <p>
        Outside research, I enjoy playing racquetball 🎾, knitting 🧶, and running 🏃‍♀️. If you'd like to connect: <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>.
      </p>
    </div>
  </div>
</div>
