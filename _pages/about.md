---
permalink: /
layout: single
author_profile: false
classes: about-inline
redirect_from: 
  - /about/
  - /about.html
---
<style>
.about-inline .page__content{ max-width:1100px; margin:0 auto; padding:0 1rem; }

/* 사진+소개 나란히 */
.intro{ display:flex; align-items:center; gap:2rem; margin:1rem 0 2rem; }
.intro__img{
width:420px; max-width:45vw; height:auto;
border-radius:16px; border:1px solid #e9e9ee;
box-shadow:0 1px 2px rgba(0,0,0,.05), 0 10px 28px -18px rgba(0,0,0,.25);
}
@media (max-width:900px){
.intro{ flex-direction:column; align-items:flex-start; gap:1.25rem; }
.intro__img{ width:100%; max-width:640px; }
}
.aboutme {
  font-family: Arial, Helvetica, sans-serif;
  max-width: 75ch;
  line-height: 1.65;
  color: #444;
  font-size: 1rem;
}

.aboutme p {
  margin: 0 0 1.2rem;
}

.aboutme h2 {
  font-size: 1.6rem;
  font-weight: 700;
  margin-bottom: 1rem;
  color: #444;
}

.aboutme ul {
  list-style: none;
  padding: 0;
  margin: 0 0 1.2rem;
}

.aboutme li {
  margin: 0.7rem 0;
  padding-left: 1.2rem;
  position: relative;
}

.aboutme li::before {
  content: "•";
  position: absolute;
  left: 0;
  color: #4169E1; /* Royal Blue dot */
  font-weight: 700;
}

.aboutme strong {
  font-weight: 600;
  color: #222;
}

.aboutme em {
  font-style: italic;
  color: #555;
}
</style>

<div class="intro">
  <!-- ⬇️ 사진 경로만 바꿔주세요 -->
  <img class="intro__img" src="/images/prof_headshot7.jpg" alt="Yeonju Lee">

  <!-- 기존 소개 블록 그대로 -->
  <div class="aboutme">
    <p>
    I am a Ph.D. student in the H. Milton Stewart School of Industrial & Systems Engineering at 
    <strong>Georgia Tech</strong>, fortunate to be advised by <strong style="color:#4169E1;">Prof. Jing Li</strong>.
  </p>

  <p>
    My research focuses on <strong style="color:#4169E1;">knowledge-informed machine learning</strong>—developing methods that incorporate domain expertise to make models more <em>data-efficient</em>, <em>robust</em>, and <em>interpretable</em>. 
    I develop methods to systematically integrate domain knowledge at different stages of the learning pipeline, tailored to the challenges posed by real-world data:
  </p>

  <ul>
    <li><strong>Representation level</strong> – encoding qualitative knowledge into quantitative representations.</li>
    <li><strong>Architecture level</strong> – embedding knowledge into network design or loss function.</li>
    <li><strong>Inference level</strong> – guiding model reasoning with explicit rules during inference.</li>
  </ul>

  <p>
    These strategies are particularly relevant under <em>real-world data challenges</em> such as 
    <strong>scarcity</strong>, <strong>heterogeneity</strong>, and 
    <strong>high dimensionality</strong>. My work applies these ideas to domains like 
    <strong style="color:#4169E1;">healthcare</strong>, 
    <strong style="color:#4169E1;">precision agriculture</strong>, and 
    <strong style="color:#4169E1;">manufacturing</strong>.
  </p>

  <p>
  Outside research, I enjoy playing racquetball 🎾, knitting 🧶, and running 🏃‍♀️—activities that keep me balanced and often refresh my perspective.  
  </p>

  <p>
  If you would like to get in touch, please reach out via email: <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>. 
  </p>
</div>
 
