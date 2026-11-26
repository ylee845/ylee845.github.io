---
permalink: /
layout: single
author_profile: false
sidebar: false
toc: false
classes: wide
redirect_from:
  - /about/
  - /about.html
---

<style>
/* Homepage-only styles. Shared layout lives in _sass/custom.scss. */

/* ===== Hero ===== */
.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 225px;
  gap: 3rem;
  align-items: center;
}
.hero-name { margin: 0 0 .25rem; color: var(--text); font-size: 2.1rem; font-weight: 600; line-height: 1.05; }
.hero-meta { margin: 0 0 1.3rem; color: var(--text-soft); font-size: 0.97rem; line-height: 1.55; }
.hero-meta a { text-decoration: underline; text-decoration-color: #9db0bf; text-underline-offset: 2px; }
.hero-title {
  max-width: 760px;
  margin: 0 0 .8rem;
  padding: 0 !important;
  border: 0 !important;
  color: var(--gt-navy);
  font-size: 1.45rem;
  font-weight: 600;
  line-height: 1.3;
}
.hero-description { max-width: 760px; margin: 0; color: #1f2429; font-size: 1.04rem !important; line-height: 1.65; }
.hero-links { margin: 1.2rem 0 0; color: var(--muted); font-size: 0.97rem; }
.hero-links a { font-weight: 600; text-decoration: underline !important; text-decoration-thickness: 1px; text-underline-offset: 3px; }
.hero-links .sep { margin: 0 .45rem; color: #c2c8ce; }
.hero-photo-wrap { width: 225px; height: 300px; overflow: hidden; border-radius: 3px; justify-self: end; }
.hero-photo { width: 100%; height: 100%; display: block; object-fit: contain; }

/* ===== Shared section rhythm ===== */
.home-section { border-top: 1px solid var(--line); padding-top: 2rem !important; }
.section-lede { max-width: 820px; margin: -.3rem 0 1.6rem; color: var(--text-soft); font-size: 1rem; line-height: 1.6; }

/* ===== Research thrusts ===== */
.thrusts { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 2.4rem; }
.thrust .num { display: block; margin-bottom: .35rem; color: var(--gt-gold); font-size: 0.97rem; font-weight: 600; }
.thrust h3 { margin: 0 0 .5rem; color: var(--text); font-size: 1.05rem; font-weight: 600; line-height: 1.3; }
.thrust p { margin: 0 0 .7rem; color: var(--text-soft); font-size: 0.97rem; line-height: 1.6; }
.thrust .keys { color: var(--muted); font-size: 0.88rem; }
.thrust .rep { margin: 0; color: #2e353c; font-size: 0.88rem; line-height: 1.5; }
.thrust .rep em { color: var(--muted); }

/* ===== Selected publications ===== */
.sel-pub { margin: 0 0 1rem; }
.sel-pub .t { margin: 0; color: var(--text); font-size: 0.97rem; font-weight: 600; line-height: 1.35; }
.sel-pub .a { margin: .12rem 0 0; color: var(--text-soft); font-size: 0.88rem; line-height: 1.4; }
.sel-pub .a strong { color: var(--text); }
.sel-pub .v { margin: .08rem 0 0; color: var(--muted); font-size: 0.88rem; }
.sel-pub .v em { color: #294e6d; }
.more-link { font-size: 0.97rem; font-weight: 600; }

@media (max-width: 980px) {
  .home-hero { grid-template-columns: minmax(0, 1fr) 190px; gap: 2rem; }
  .hero-photo-wrap { width: 190px; height: 253px; }
  .thrusts { grid-template-columns: 1fr; gap: 1.6rem; }
}
@media (max-width: 760px) {
  .home-hero { grid-template-columns: 1fr; gap: 1.2rem; }
  .hero-photo-wrap { grid-row: 1; justify-self: start; width: 150px; height: 200px; }
  .hero-name { font-size: 1.8rem; }
  .hero-title { font-size: 1.25rem; }
}
</style>

<section class="home-hero l-shell">
  <div>
    <h1 class="hero-name">Yeonju Lee</h1>
    <p class="hero-meta">
      Ph.D. Student in Machine Learning, Georgia Institute of Technology<br>
      H. Milton Stewart School of Industrial &amp; Systems Engineering · Advisor: <a href="https://isye.gatech.edu/users/jing-li" target="_blank" rel="noopener">Prof. Jing Li</a>
    </p>

    <h2 class="hero-title">Knowledge-Informed AI and ML for Complex Scientific and Physical Systems</h2>

    <p class="hero-description">
      In hospitals, farms, and factories, AI must work with scarce labels and conditions that keep changing.
      My research makes AI reliable in these settings by building scientific and engineering knowledge, such as anatomy and soil&ndash;water&ndash;crop dynamics,
      into foundation models, generative models, and adaptive world models.
    </p>

    <p class="hero-links">
      <a href="/files/Yeonju_Lee_CV.pdf">CV</a><span class="sep">|</span>
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a><span class="sep">|</span>
      <a href="https://www.linkedin.com/in/ylee845" target="_blank" rel="noopener">LinkedIn</a><span class="sep">|</span>
      <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>
    </p>
  </div>

  <div class="hero-photo-wrap">
    <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
  </div>
</section>

<section class="l-shell home-section">
  <h2 class="section-title">Research</h2>
  <p class="section-lede">
    How can AI make trustworthy decisions about the physical world when data are limited and the environment shifts?
    I approach this question by integrating domain knowledge with modern AI across three connected capabilities.
  </p>

  <div class="thrusts">
    <div class="thrust">
      <span class="num">01</span>
      <h3>Perception from scarce data</h3>
      <p>Teaching models what clinicians already know about anatomy, so they can segment and detect disease in 3D images from few labeled examples.</p>
      <p class="keys">Knowledge-informed semi-supervised learning · generative models · foundation models</p>
      <p class="rep">IEEE T-ASE 2025 · IISE THSE 2026 · Cytotherapy 2026</p>
    </div>
    <div class="thrust">
      <span class="num">02</span>
      <h3>Reasoning over scientific signals</h3>
      <p>Using large language models to read soil-moisture sensor data the way an agronomist would, recognizing meaningful patterns and anomalies to support prediction.</p>
      <p class="keys">LLM-based reasoning · spatiotemporal learning · anomaly detection</p>
      <p class="rep">Comput. Electron. Agric. (under review) · ACS ES&amp;T Eng. 2026</p>
    </div>
    <div class="thrust">
      <span class="num">03</span>
      <h3>Decisions under environment shifts</h3>
      <p>Giving controllers a learned simulator of how a system responds to actions, and letting it adapt to environments it has never seen.</p>
      <p class="keys">World models · meta-learning · test-time adaptation · model predictive control</p>
      <p class="rep">IISE Transactions (under review)</p>
    </div>
  </div>
  <p style="margin:1.6rem 0 0;"><a class="more-link" href="/research/">More about my research &rarr;</a></p>
</section>

<section class="l-shell home-section">
  <h2 class="section-title">Selected Publications</h2>
  <div class="sel-pub">
    <p class="t">Knowledge-Informed World Model Adaptation for Predictive Irrigation Control under Environmental Shifts</p>
    <p class="a"><strong>Y. Lee</strong>, X. Qiao, Y. Chen, J. Li</p>
    <p class="v"><em>IISE Transactions</em> (submitted).</p>
  </div>
  <div class="sel-pub">
    <p class="t">SPADE: A Large Language Model Framework for Soil Moisture Pattern Recognition and Anomaly Detection in Precision Agriculture</p>
    <p class="a"><strong>Y. Lee</strong>, R.Q. Chen, X. Qiao, Y. Shi, W. Liang, Y. Chen, J. Li</p>
    <p class="v"><em>Computers and Electronics in Agriculture</em> (revised paper under second-round review).</p>
  </div>
  <div class="sel-pub">
    <p class="t">BrainNormalizer: Anatomy-Informed Pseudo-Healthy Brain Reconstruction from Tumor MRI via Edge-Guided ControlNet</p>
    <p class="a">M.G. Kwak, <strong>Y. Lee</strong>, H. Wang, J. Li</p>
    <p class="v"><em>IISE Transactions on Healthcare Systems Engineering</em>, 16(4), 474&ndash;486, 2026.</p>
  </div>
  <div class="sel-pub">
    <p class="t">Foundation Model Cascades Enable Zero-Shot Microscopy Image Analysis for Cell Therapy Manufacturing</p>
    <p class="a">R.Q. Chen, <strong>Y. Lee</strong>, B. Joffe, P.C. Costa, C. Filan, B. Wang, S. Balakirsky, F. Robles, K. Roy, J. Li</p>
    <p class="v"><em>Cytotherapy</em>, 28(5), 102078, 2026.</p>
  </div>
  <div class="sel-pub">
    <p class="t">Oral-Anatomical Knowledge-Informed Semi-Supervised Learning for 3D Dental CBCT Segmentation and Lesion Detection</p>
    <p class="a"><strong>Y. Lee</strong>, M.G. Kwak, R.Q. Chen, H. Yan, M. Mupparapu, F. Lure, F.C. Setzer, J. Li</p>
    <p class="v"><em>IEEE Transactions on Automation Science and Engineering</em>, 22, 11205&ndash;11218, 2025. IISE DAIS Best Paper Finalist, 2024.</p>
  </div>
  <p style="margin:.4rem 0 0;"><a class="more-link" href="/publications/">All publications &rarr;</a></p>
</section>
