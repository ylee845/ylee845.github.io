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
/* Homepage-only styles. Shared layout (.l-shell, colours, chips)
   lives in _sass/custom.scss. */

/* ===== Hero ===== */
.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 240px;
  gap: 2.75rem;
  align-items: center;
}
.hero-name {
  margin: 0 0 .2rem;
  color: var(--text);
  font-size: 2.15rem;
  font-weight: 600;
  line-height: 1.05;
}
.hero-meta {
  margin: 0 0 1rem;
  color: var(--text-soft);
  font-size: .94rem;
  line-height: 1.5;
}
.hero-meta a { text-decoration: underline; text-decoration-color: #9db0bf; text-underline-offset: 2px; }
.hero-title {
  max-width: 780px;
  padding: 0 !important;
  border: 0 !important;
  margin: 0 0 .7rem;
  color: var(--gt-navy);
  font-size: 1.55rem;
  font-weight: 600;
  line-height: 1.22;
}
.hero-description {
  max-width: 760px;
  margin: 0 0 .55rem;
  color: #333b43;
  font-size: 1rem;
  line-height: 1.6;
}
.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: .5rem;
  margin: 1rem 0 0;
}
.hero-links a {
  display: inline-block;
  padding: .32rem .8rem;
  border: 1px solid #cfd8e0;
  border-radius: 4px;
  color: var(--gt-navy);
  font-size: .86rem;
  font-weight: 600;
  text-decoration: none !important;
}
.hero-links a.primary { background: var(--gt-navy); border-color: var(--gt-navy); color: #fff; }
.hero-links a:hover { text-decoration: none; border-color: var(--gt-navy); }
.hero-links a.primary:hover { background: #0b3d6b; color: #fff; }
.cv-updated { align-self: center; color: var(--muted); font-size: .74rem; }
.hero-photo-wrap { width: 240px; height: 320px; overflow: hidden; border-radius: 4px; justify-self: end; }
.hero-photo { width: 100%; height: 100%; display: block; object-fit: contain; }

/* ===== At a glance ===== */
.glance {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  border-top: 1px solid var(--line);
  border-bottom: 1px solid var(--line);
}
.glance div { padding: 1rem 1.1rem; }
.glance div + div { border-left: 1px solid var(--line); }
.glance b { display: block; color: var(--gt-navy); font-size: 1.9rem; font-weight: 600; line-height: 1; }
.glance span { display: block; margin-top: .3rem; color: var(--text-soft); font-size: .84rem; line-height: 1.35; }
.venues { margin: .8rem 0 0; color: var(--muted); font-size: .84rem; line-height: 1.5; }
.venues strong { color: var(--text-soft); font-weight: 600; }

/* ===== Research in one picture ===== */
.big-question {
  margin: 0 0 1.4rem;
  padding-left: 1rem;
  border-left: 3px solid var(--gt-gold);
  color: var(--text);
  font-size: 1.12rem;
  line-height: 1.5;
}
.big-question em { color: var(--gt-navy); font-style: normal; font-weight: 600; }
.pipeline {
  display: grid;
  grid-template-columns: 1fr auto 2.6fr auto 1fr;
  gap: .9rem;
  align-items: stretch;
}
.pipe-arrow { align-self: center; color: var(--gt-gold); font-size: 1.5rem; font-weight: 600; }
.pipe-box {
  padding: .95rem 1rem;
  border: 1px solid var(--line);
  border-radius: 4px;
  background: #fbfbfa;
}
.pipe-box h4 { margin: 0 0 .4rem; color: var(--muted); font-size: .72rem; font-weight: 600; text-transform: uppercase; letter-spacing: .04em !important; }
.pipe-box ul { margin: 0; padding-left: 1rem; color: var(--text-soft); font-size: .86rem; line-height: 1.5; }
.pipe-core { display: flex; flex-direction: column; background: var(--gt-navy); border-color: var(--gt-navy); }
.pipe-core h4 { color: #d9cfa6; }
.pipe-steps { flex: 1; display: grid; grid-template-columns: repeat(3, 1fr); gap: .7rem; }
.pipeline { align-items: center; }
.pipe-step { padding: .8rem .8rem; border-radius: 3px; background: rgba(255,255,255,.08); }
.pipe-step b { display: block; color: #fff; font-size: .95rem; font-weight: 600; }
.pipe-step span { display: block; margin-top: .2rem; color: #c9d5e0; font-size: .8rem; line-height: 1.4; }

/* ===== Research thrusts ===== */
.thrust-grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 1.4rem; }
.thrust {
  position: relative;
  display: flex;
  flex-direction: column;
  padding: 1.15rem 1.2rem 1.05rem;
  border: 1px solid var(--line);
  border-top: 3px solid var(--gt-gold);
  border-radius: 4px;
}
.thrust-kicker { margin: 0; color: #867b4f; font-size: .72rem; font-weight: 600; text-transform: uppercase; letter-spacing: .04em !important; }
.thrust h3 { margin: .2rem 0 .45rem; color: var(--text); font-size: 1.08rem; font-weight: 600; line-height: 1.28; }
.thrust .plain { margin: 0 0 .55rem; color: var(--gt-navy); font-size: .9rem; font-weight: 500; line-height: 1.45; }
.thrust .tech { margin: 0 0 .8rem; color: var(--text-soft); font-size: .84rem; line-height: 1.5; }
.thrust .reps { margin-top: auto; padding-top: .65rem; border-top: 1px solid var(--line); }
.thrust .reps p { margin: 0 0 .35rem; color: #353c43; font-size: .8rem; line-height: 1.4; }
.thrust .reps p em { color: var(--muted); }

/* ===== Featured paper ===== */
.featured {
  padding: 1.5rem 1.6rem;
  border: 1px solid #d6dee6;
  border-radius: 6px;
  background: linear-gradient(180deg, #f6f9fb 0%, #ffffff 100%);
}
.featured-head { display: flex; flex-wrap: wrap; gap: .5rem; align-items: center; margin-bottom: .45rem; }
.featured h3 { margin: 0 0 .3rem; color: var(--text); font-size: 1.22rem; font-weight: 600; line-height: 1.3; }
.featured .byline { margin: 0 0 .9rem; color: var(--muted); font-size: .86rem; }
.featured .byline strong { color: var(--text-soft); }
.featured .lede { max-width: 900px; margin: 0 0 1.1rem; color: #333b43; font-size: .97rem; line-height: 1.6; }
.steps { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: .8rem; margin-bottom: 1.2rem; counter-reset: step; }
.step { position: relative; padding: .8rem .85rem .8rem; border: 1px solid var(--line); border-radius: 4px; background: #fff; }
.step::before {
  counter-increment: step;
  content: counter(step);
  display: inline-flex; align-items: center; justify-content: center;
  width: 1.45rem; height: 1.45rem; margin-bottom: .4rem;
  border-radius: 50%; background: var(--gt-navy); color: #fff;
  font-size: .78rem; font-weight: 600;
}
.step b { display: block; color: var(--text); font-size: .92rem; font-weight: 600; line-height: 1.3; }
.step span { display: block; margin-top: .25rem; color: var(--text-soft); font-size: .8rem; line-height: 1.45; }
.step small { display: block; margin-top: .4rem; color: #867b4f; font-size: .72rem; font-weight: 600; }
.results { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: .8rem; }
.result { padding: .75rem .9rem; border-left: 3px solid var(--gt-gold); background: #fff; }
.result b { display: block; color: var(--gt-navy); font-size: 1.45rem; font-weight: 600; line-height: 1.1; }
.result span { display: block; margin-top: .25rem; color: var(--text-soft); font-size: .8rem; line-height: 1.4; }
.fine { margin: .8rem 0 0; color: var(--muted); font-size: .76rem; line-height: 1.45; }

/* ===== Highlights + selected pubs ===== */
.two-col { display: grid; grid-template-columns: minmax(0, 1.5fr) minmax(0, 1fr); gap: 2.5rem; }
.sel-pub { padding: .6rem 0; border-top: 1px solid #eef0f2; }
.sel-pub:first-of-type { border-top: 0; padding-top: 0; }
.sel-pub .t { margin: 0; color: var(--text); font-size: .94rem; font-weight: 600; line-height: 1.3; }
.sel-pub .a { margin: .12rem 0 0; color: var(--text-soft); font-size: .84rem; line-height: 1.35; }
.sel-pub .a strong { color: var(--text); }
.sel-pub .v { margin: .1rem 0 0; color: var(--muted); font-size: .83rem; }
.sel-pub .v em { color: #294e6d; }
.more-link { display: inline-block; margin-top: .7rem; font-size: .88rem; font-weight: 600; }
.news { margin: 0; padding: 0; list-style: none; }
.news li { display: grid; grid-template-columns: 3rem minmax(0, 1fr); gap: .6rem; padding: .45rem 0; border-top: 1px solid #eef0f2; font-size: .86rem; line-height: 1.45; color: var(--text-soft); }
.news li:first-child { border-top: 0; padding-top: 0; }
.news .yr { color: var(--gt-navy); font-weight: 600; }

@media (max-width: 980px) {
  .home-hero { grid-template-columns: minmax(0, 1fr) 200px; gap: 2rem; }
  .hero-photo-wrap { width: 200px; height: 267px; }
  .pipeline { grid-template-columns: 1fr; }
  .pipe-arrow { justify-self: center; transform: rotate(90deg); }
  .thrust-grid { grid-template-columns: 1fr; }
  .steps { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .two-col { grid-template-columns: 1fr; gap: 1.8rem; }
}
@media (max-width: 760px) {
  .home-hero { grid-template-columns: 1fr; gap: 1rem; }
  .hero-photo-wrap { grid-row: 1; justify-self: center; width: min(70vw, 260px); height: auto; aspect-ratio: 3 / 4; }
  .hero-name { font-size: 1.85rem; }
  .hero-title { font-size: 1.3rem; }
  .glance { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .glance div:nth-child(3) { border-left: 0; }
  .glance div:nth-child(n+3) { border-top: 1px solid var(--line); }
  .pipe-steps, .steps, .results { grid-template-columns: 1fr; }
  .featured { padding: 1.1rem 1rem; }
}
</style>

<!-- ============ HERO ============ -->
<section class="home-hero l-shell l-shell--wide">
  <div class="hero-copy">
    <h1 class="hero-name">Yeonju Lee</h1>
    <p class="hero-meta">
      Ph.D. in Machine Learning (expected 2027) · H. Milton Stewart School of Industrial &amp; Systems Engineering, Georgia Tech<br>
      Advised by <a href="https://isye.gatech.edu/users/jing-li" target="_blank" rel="noopener">Prof. Jing Li</a>
    </p>

    <h2 class="hero-title">Knowledge-informed AI that perceives, predicts, and decides in complex physical and biomedical systems</h2>

    <p class="hero-description">
      AI models are powerful, but in hospitals, farms, and factories they often face <strong>scarce labels</strong> and <strong>conditions that keep changing</strong>.
      My research makes AI reliable in exactly those settings by building in what scientists and engineers already know &mdash; anatomy, soil&ndash;water&ndash;crop physics, process knowledge &mdash;
      into modern architectures such as foundation models, generative models, and adaptive world models.
    </p>

    <div class="hero-links">
      <a class="primary" href="/files/Yeonju_Lee_CV.pdf">CV (PDF)</a>
      <a href="/research/">Research</a>
      <a href="/publications/">Publications</a>
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
      <a href="mailto:ylee845@gatech.edu">ylee845@gatech.edu</a>
      <a href="https://www.linkedin.com/in/ylee845" target="_blank" rel="noopener">LinkedIn</a>
      <span class="cv-updated">CV updated Nov 2026</span>
    </div>
  </div>

  <div class="hero-photo-wrap">
    <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
  </div>
</section>

<!-- ============ AT A GLANCE ============ -->
<section class="l-shell l-shell--wide">
  <div class="glance">
    <div><b>13</b><span>journal papers<br>(8 published / accepted)</span></div>
    <div><b>7</b><span>first-author papers<br>(3 published, 2 under review)</span></div>
    <div><b>2</b><span>U.S. provisional patents on 3D medical-image AI</span></div>
    <div><b>5</b><span>conference talks, incl. INFORMS invited session</span></div>
  </div>
  <p class="venues"><strong>Published in</strong> IEEE Transactions on Automation Science and Engineering · IISE Transactions on Healthcare Systems Engineering · International Journal of Production Research · Journal of Endodontics · Cytotherapy · ACS ES&amp;T Engineering · Dental Clinics of North America</p>
</section>

<!-- ============ RESEARCH IN ONE PICTURE ============ -->
<section class="l-shell l-shell--wide">
  <p class="eyebrow">Research in one picture</p>
  <p class="big-question">
    The question that drives my work: <em>How can AI make trustworthy decisions about the physical world when data are limited and the environment shifts?</em>
    My answer is to let scientific knowledge do the work that missing data cannot.
  </p>

  <div class="pipeline">
    <div class="pipe-box">
      <h4>Inputs</h4>
      <ul>
        <li><strong>Domain knowledge</strong>: anatomy, crop &amp; soil physics, process rules, text descriptions</li>
        <li><strong>Sparse data</strong>: 3D CT/MRI, microscopy, field sensors</li>
      </ul>
    </div>
    <div class="pipe-arrow" aria-hidden="true">&rarr;</div>
    <div class="pipe-box pipe-core">
      <h4>Knowledge-informed AI</h4>
      <div class="pipe-steps">
        <div class="pipe-step"><b>Perceive</b><span>Knowledge-guided segmentation &amp; detection from few labels</span></div>
        <div class="pipe-step"><b>Reason &amp; predict</b><span>Foundation-model reasoning over spatiotemporal signals</span></div>
        <div class="pipe-step"><b>Decide &amp; control</b><span>Adaptive world models for control under environment shifts</span></div>
      </div>
    </div>
    <div class="pipe-arrow" aria-hidden="true">&rarr;</div>
    <div class="pipe-box">
      <h4>Impact</h4>
      <ul>
        <li><strong>Precision diagnosis</strong> in dental &amp; brain imaging</li>
        <li><strong>Sustainable agriculture</strong>: water &amp; nutrient management</li>
        <li><strong>Intelligent manufacturing</strong>: quality &amp; fault discovery</li>
      </ul>
    </div>
  </div>
</section>

<!-- ============ THRUSTS ============ -->
<section class="l-shell l-shell--wide">
  <h2 class="section-title">Research Thrusts</h2>
  <div class="thrust-grid">
    <article class="thrust">
      <p class="thrust-kicker">Thrust 1 · Perception</p>
      <h3>Knowledge-guided learning from scarce, high-dimensional data</h3>
      <p class="plain">Teach a model what a clinician already knows about anatomy, so it finds lesions in 3D scans without thousands of labeled examples.</p>
      <p class="tech">Anatomy-informed semi-supervised learning, generative (ControlNet) reconstruction, and foundation-model cascades for 3D CBCT, brain MRI, and microscopy.</p>
      <div class="reps">
        <p>Oral-anatomical knowledge-informed semi-supervised learning &mdash; <em>IEEE T-ASE 2025 · Best Paper Finalist</em></p>
        <p>BrainNormalizer &mdash; <em>IISE Trans. Healthcare Sys. Eng. 2026 · Spotlight</em></p>
        <p>Foundation model cascades for zero-shot microscopy &mdash; <em>Cytotherapy 2026</em></p>
      </div>
    </article>

    <article class="thrust">
      <p class="thrust-kicker">Thrust 2 · Reasoning &amp; Prediction</p>
      <h3>Foundation-model reasoning over scientific time series</h3>
      <p class="plain">Let a language model read soil-moisture signals the way an agronomist would, recognizing meaningful patterns and flagging anomalies, and use them to forecast what the season will bring.</p>
      <p class="tech">LLM frameworks for pattern recognition and anomaly detection, and spatiotemporal learning of depth-specific trajectories for cross-year yield prediction.</p>
      <div class="reps">
        <p>SPADE: LLM framework for soil-moisture pattern recognition &mdash; <em>Comput. Electron. Agric., 2nd-round review</em></p>
        <p>Lightweight anomaly detection for nutrient management &mdash; <em>ACS ES&amp;T Eng. 2026</em></p>
      </div>
    </article>

    <article class="thrust">
      <p class="thrust-kicker">Thrust 3 · Decision &amp; Control</p>
      <h3>Adaptive world models for decisions under environment shifts</h3>
      <p class="plain">Give an AI controller a &ldquo;mental simulator&rdquo; of how crops respond to water, and let it re-tune itself to a farm it has never seen before.</p>
      <p class="tech">Knowledge-conditioned meta-learning, LLM-driven hypernetworks, test-time adaptation, and model predictive control, with regret guarantees.</p>
      <div class="reps">
        <p>KIWIC: Knowledge-informed world model adaptation for predictive irrigation control &mdash; <em>IISE Transactions, submitted</em></p>
      </div>
    </article>
  </div>
</section>

<!-- ============ FEATURED ============ -->
<section class="l-shell l-shell--wide">
  <h2 class="section-title">Featured: Newest Work</h2>
  <div class="featured">
    <div class="featured-head">
      <span class="chip chip--gold">New</span>
      <span class="chip">IISE Transactions (submitted)</span>
      <span class="chip">World models · Meta-learning · LLMs · MPC</span>
    </div>
    <h3>Knowledge-Informed World Model Adaptation for Predictive Irrigation Control under Environmental Shifts</h3>
    <p class="byline"><strong>Y. Lee</strong>, X. Qiao, Y. Chen, J. Li</p>

    <p class="lede">
      Agriculture uses about 72% of the world&rsquo;s freshwater, yet the same irrigation decision can help or hurt a crop depending on the soil and climate.
      An AI controller trained on some farms therefore breaks down on new ones, and a new farm rarely has enough sensor data to re-learn from scratch.
      <strong>KIWIC</strong> closes this gap by combining what we can <em>read</em> about a new farm with the few things we can <em>measure</em> there.
    </p>

    <div class="steps">
      <div class="step"><b>Learn shared physics</b><span>A world model learns how irrigation drives soil moisture, canopy cover, and biomass across many source farms.</span><small>Action-conditioned world model</small></div>
      <div class="step"><b>Read the new farm</b><span>An LLM encodes the farm&rsquo;s soil and climate description; a hypernetwork turns it into a tailored starting point.</span><small>LLM + hypernetwork initialization</small></div>
      <div class="step"><b>Adapt on the fly</b><span>A lightweight adapter is refined from a handful of soil-moisture readings, trained with factual &amp; counterfactual supervision.</span><small>Meta-learning + test-time adaptation</small></div>
      <div class="step"><b>Plan irrigation</b><span>The adapted model simulates candidate schedules and picks the best one under a water budget.</span><small>Model predictive control</small></div>
    </div>

    <div class="results">
      <div class="result"><b>+11.6%</b><span>crop yield vs. the non-adapted world model, while using less water (45.0 vs. 40.3 t/ha)</span></div>
      <div class="result"><b>&minus;15%</b><span>decision regret vs. the strongest adaptation baseline (0.044 vs. 0.052)</span></div>
      <div class="result"><b>+31%</b><span>yield with the <em>same</em> 500 mm of water in a representative site, from smarter timing alone</span></div>
    </div>
    <p class="fine">Evaluated in AquaCrop simulation on sugar beet across 60 environments unseen during training. The paper also proves decision-preservation conditions and a regret bound that links prediction error to control quality.</p>
  </div>
</section>

<!-- ============ HIGHLIGHTS + SELECTED PUBS ============ -->
<section class="l-shell l-shell--wide">
  <div class="two-col">
    <div>
      <h2 class="section-title">Selected Publications</h2>
      <div class="sel-pub">
        <p class="t">Oral-Anatomical Knowledge-Informed Semi-Supervised Learning for 3D Dental CBCT Segmentation and Lesion Detection</p>
        <p class="a"><strong>Y. Lee</strong>, M.G. Kwak, R.Q. Chen, H. Yan, M. Mupparapu, F. Lure, F.C. Setzer, J. Li</p>
        <p class="v"><em>IEEE Transactions on Automation Science and Engineering</em>, 2025 <span class="chip chip--gold">IISE DAIS Best Paper Finalist</span></p>
      </div>
      <div class="sel-pub">
        <p class="t">Dentin-Normalized CBCT Radiomics within a Periapical Lesion Differential Diagnosis System for Differentiating Granulomas and Radicular Cysts</p>
        <p class="a"><strong>Y. Lee</strong>, R.Q. Chen, H. Yan, M. Mupparapu, F. Lure, J. Li, F.C. Setzer</p>
        <p class="v"><em>Journal of Endodontics</em>, in press, 2026</p>
      </div>
      <div class="sel-pub">
        <p class="t">BrainNormalizer: Anatomy-Informed Pseudo-Healthy Brain Reconstruction from Tumor MRI via Edge-Guided ControlNet</p>
        <p class="a">M.G. Kwak, <strong>Y. Lee</strong>, H. Wang, J. Li</p>
        <p class="v"><em>IISE Transactions on Healthcare Systems Engineering</em>, 2026 <span class="chip chip--gold">Monthly Spotlight · ISE Magazine feature</span></p>
      </div>
      <div class="sel-pub">
        <p class="t">Foundation Model Cascades Enable Zero-Shot Microscopy Image Analysis for Cell Therapy Manufacturing</p>
        <p class="a">R.Q. Chen, <strong>Y. Lee</strong>, B. Joffe, P.C. Costa, C. Filan, B. Wang, S. Balakirsky, F. Robles, K. Roy, J. Li</p>
        <p class="v"><em>Cytotherapy</em>, 2026</p>
      </div>
      <div class="sel-pub">
        <p class="t">Discovery of Fault-Introducing Tool Groups with a Numerical Association Rule Mining Method in a Printed Circuit Board Production Line</p>
        <p class="a"><strong>Y. Lee</strong>, Y. Kim, B. Lee, C.O. Kim</p>
        <p class="v"><em>International Journal of Production Research</em>, 2024</p>
      </div>
      <a class="more-link" href="/publications/">All 13 papers &rarr;</a>
    </div>

    <div>
      <h2 class="section-title">Highlights</h2>
      <ul class="news">
        <li><span class="yr">2026</span><span>Paper on knowledge-informed world models for irrigation control submitted to <em>IISE Transactions</em>.</span></li>
        <li><span class="yr">2026</span><span><em>BrainNormalizer</em> selected for the journal&rsquo;s Monthly Spotlight Series and featured in <em>ISE Magazine</em>.</span></li>
        <li><span class="yr">2026</span><span>Four more journal articles published or in press in <em>J. Endodontics</em>, <em>Cytotherapy</em>, <em>ACS ES&amp;T Eng.</em>, and <em>Dental Clinics of N. America</em>.</span></li>
        <li><span class="yr">2025</span><span>George Fellowship and Stewart Fellowship, Georgia Tech ISyE.</span></li>
        <li><span class="yr">2025</span><span>Invited talk, INFORMS Annual Meeting (Atlanta).</span></li>
        <li><span class="yr">2024</span><span>Finalist, Best Track Paper Award, IISE Data Analytics &amp; Information Systems (DAIS).</span></li>
        <li><span class="yr">2024</span><span>Two U.S. provisional patent applications filed on 3D CBCT segmentation and lesion detection.</span></li>
      </ul>
    </div>
  </div>
</section>
