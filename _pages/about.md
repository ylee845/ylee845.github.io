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
.hero-meta { margin: 0 0 1.3rem; color: var(--text-soft); font-size: .95rem; line-height: 1.55; }
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
.hero-description { max-width: 740px; margin: 0; color: #333b43; font-size: 1rem; line-height: 1.65; }
.hero-links { margin: 1.2rem 0 0; color: var(--muted); font-size: .92rem; }
.hero-links a { font-weight: 600; text-decoration: none !important; }
.hero-links .sep { margin: 0 .45rem; color: #c2c8ce; }
.hero-photo-wrap { width: 225px; height: 300px; overflow: hidden; border-radius: 3px; justify-self: end; }
.hero-photo { width: 100%; height: 100%; display: block; object-fit: contain; }

/* ===== Shared section rhythm ===== */
.home-section { border-top: 1px solid var(--line); padding-top: 2rem !important; }
.section-lede { max-width: 820px; margin: -.3rem 0 1.6rem; color: var(--text-soft); font-size: .98rem; line-height: 1.6; }

/* ===== Research thrusts ===== */
.thrusts { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 2.4rem; }
.thrust .num { display: block; margin-bottom: .35rem; color: var(--gt-gold); font-size: .9rem; font-weight: 600; }
.thrust h3 { margin: 0 0 .5rem; color: var(--text); font-size: 1.05rem; font-weight: 600; line-height: 1.3; }
.thrust p { margin: 0 0 .7rem; color: var(--text-soft); font-size: .9rem; line-height: 1.6; }
.thrust .keys { color: var(--muted); font-size: .82rem; }
.thrust .rep { margin: 0; color: #3a4148; font-size: .82rem; line-height: 1.5; }
.thrust .rep em { color: var(--muted); }

/* ===== Publications + news ===== */
.two-col { display: grid; grid-template-columns: minmax(0, 1.55fr) minmax(0, 1fr); gap: 3rem; }
.sel-pub { margin: 0 0 1rem; }
.sel-pub .t { margin: 0; color: var(--text); font-size: .94rem; font-weight: 600; line-height: 1.35; }
.sel-pub .a { margin: .12rem 0 0; color: var(--text-soft); font-size: .85rem; line-height: 1.4; }
.sel-pub .a strong { color: var(--text); }
.sel-pub .v { margin: .08rem 0 0; color: var(--muted); font-size: .85rem; }
.sel-pub .v em { color: #294e6d; }
.more-link { font-size: .9rem; font-weight: 600; }
.news { margin: 0; padding: 0; list-style: none; }
.news li { display: grid; grid-template-columns: 2.8rem minmax(0, 1fr); gap: .5rem; margin: 0 0 .7rem; color: var(--text-soft); font-size: .88rem; line-height: 1.5; }
.news .yr { color: var(--muted); font-weight: 600; }

@media (max-width: 980px) {
  .home-hero { grid-template-columns: minmax(0, 1fr) 190px; gap: 2rem; }
  .hero-photo-wrap { width: 190px; height: 253px; }
  .thrusts { grid-template-columns: 1fr; gap: 1.6rem; }
  .two-col { grid-template-columns: 1fr; gap: 1.4rem; }
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
  <div class="two-col">
    <div>
      <h2 class="section-title">Selected Publications</h2>
      <div class="sel-pub">
        <p class="t">Oral-Anatomical Knowledge-Informed Semi-Supervised Learning for 3D Dental CBCT Segmentation and Lesion Detection</p>
        <p class="a"><strong>Y. Lee</strong>, M.G. Kwak, R.Q. Chen, H. Yan, M. Mupparapu, F. Lure, F.C. Setzer, J. Li</p>
        <p class="v"><em>IEEE Transactions on Automation Science and Engineering</em>, 2025. IISE DAIS Best Paper Finalist.</p>
      </div>
      <div class="sel-pub">
        <p class="t">Dentin-Normalized CBCT Radiomics within a Periapical Lesion Differential Diagnosis System for Differentiating Granulomas and Radicular Cysts</p>
        <p class="a"><strong>Y. Lee</strong>, R.Q. Chen, H. Yan, M. Mupparapu, F. Lure, J. Li, F.C. Setzer</p>
        <p class="v"><em>Journal of Endodontics</em>, in press, 2026.</p>
      </div>
      <div class="sel-pub">
        <p class="t">BrainNormalizer: Anatomy-Informed Pseudo-Healthy Brain Reconstruction from Tumor MRI via Edge-Guided ControlNet</p>
        <p class="a">M.G. Kwak, <strong>Y. Lee</strong>, H. Wang, J. Li</p>
        <p class="v"><em>IISE Transactions on Healthcare Systems Engineering</em>, 2026.</p>
      </div>
      <div class="sel-pub">
        <p class="t">Foundation Model Cascades Enable Zero-Shot Microscopy Image Analysis for Cell Therapy Manufacturing</p>
        <p class="a">R.Q. Chen, <strong>Y. Lee</strong>, B. Joffe, P.C. Costa, C. Filan, B. Wang, S. Balakirsky, F. Robles, K. Roy, J. Li</p>
        <p class="v"><em>Cytotherapy</em>, 2026.</p>
      </div>
      <p style="margin:.4rem 0 0;"><a class="more-link" href="/publications/">All publications &rarr;</a></p>
    </div>

    <div>
      <h2 class="section-title">News</h2>
      <ul class="news">
        <li><span class="yr">2026</span><span>Paper on knowledge-informed world models for irrigation control submitted to <em>IISE Transactions</em>.</span></li>
        <li><span class="yr">2026</span><span><em>BrainNormalizer</em> selected for the journal&rsquo;s Monthly Spotlight Series and featured in <em>ISE Magazine</em>.</span></li>
        <li><span class="yr">2025</span><span>George Fellowship and Stewart Fellowship, Georgia Tech ISyE.</span></li>
        <li><span class="yr">2025</span><span>Invited talk, INFORMS Annual Meeting, Atlanta.</span></li>
        <li><span class="yr">2024</span><span>Finalist, Best Track Paper Award, IISE DAIS.</span></li>
      </ul>
    </div>
  </div>
</section>
