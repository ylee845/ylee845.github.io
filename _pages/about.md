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
:root {
  --ink: #202327;
  --muted: #687078;
  --accent: #294f73;
  --line: #e8ebee;
}

/* Remove the large vertical gap inherited from the theme */
#main {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

.page,
.page__inner-wrap,
.page__content {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

.page__content {
  max-width: 1080px !important;
  margin-left: auto !important;
  margin-right: auto !important;
}

/* Compact first screen */
.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 210px;
  gap: 3.2rem;
  align-items: center;
  padding: 1.35rem 0 2.1rem;
  border-bottom: 1px solid var(--line);
}

.eyebrow {
  margin: 0 0 .42rem;
  color: #59626b;
  font-size: .77rem;
  font-weight: 600;
  letter-spacing: .07em;
  text-transform: uppercase;
}

.hero-name {
  margin: 0 0 .32rem;
  font-size: clamp(2.25rem, 4vw, 3.35rem);
  font-weight: 650;
  line-height: 1.03;
  letter-spacing: -.035em;
  color: var(--ink);
}

.hero-title {
  margin: 0 0 .9rem;
  max-width: 720px;
  font-size: clamp(1.35rem, 2.5vw, 1.9rem);
  font-weight: 600;
  line-height: 1.18;
  letter-spacing: -.025em;
  color: var(--accent);
}

.hero-description {
  max-width: 680px;
  margin: 0 0 .72rem;
  color: #2f3439;
  font-size: .98rem;
  line-height: 1.58;
}

.hero-meta {
  margin: 0 0 .95rem;
  color: #4e565e;
  font-size: .87rem;
  line-height: 1.5;
}

.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: .4rem;
}

.hero-links a {
  display: inline-block;
  padding: .36rem .62rem;
  border: 1px solid #d2d7dc;
  border-radius: 2px;
  color: #2d3b47;
  font-size: .82rem;
  font-weight: 600;
  line-height: 1.2;
}

.hero-links a:hover {
  border-color: var(--accent);
  color: var(--accent);
  text-decoration: none;
}

.hero-photo {
  width: 100%;
  max-width: 210px;
  justify-self: end;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  object-position: center;
}

/* Main sections */
.home-section {
  padding: 2.35rem 0 2rem;
  border-bottom: 1px solid var(--line);
}

.section-kicker {
  margin: 0 0 .3rem;
  color: var(--muted);
  font-size: .74rem;
  font-weight: 600;
  letter-spacing: .07em;
  text-transform: uppercase;
}

.section-title {
  margin: 0 0 1.2rem;
  font-size: 1.45rem;
  font-weight: 650;
  color: var(--ink);
  letter-spacing: -.018em;
}

.research-item {
  display: grid;
  grid-template-columns: 135px minmax(0, 1fr);
  gap: 1.25rem;
  padding: 1.05rem 0;
  border-top: 1px solid var(--line);
}

.research-item:first-of-type {
  border-top: 0;
  padding-top: 0;
}

.research-status {
  color: var(--muted);
  font-size: .78rem;
  font-weight: 600;
  line-height: 1.45;
}

.research-title {
  margin: 0 0 .25rem;
  font-size: .99rem;
  font-weight: 650;
  line-height: 1.4;
  color: var(--ink);
}

.research-desc {
  margin: 0;
  color: #50575e;
  font-size: .88rem;
  line-height: 1.52;
}

.research-tags {
  margin-top: .4rem;
  color: var(--accent);
  font-size: .75rem;
  font-weight: 600;
}

.area-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.65rem;
}

.area h3 {
  margin: 0 0 .35rem;
  color: var(--ink);
  font-size: .95rem;
  font-weight: 650;
}

.area p {
  margin: 0;
  color: var(--muted);
  font-size: .84rem;
  line-height: 1.5;
}

.highlights {
  padding: 1.9rem 0 .6rem;
}

.highlight-line {
  margin: 0;
  color: #555d64;
  font-size: .84rem;
  line-height: 1.65;
}

.highlight-line strong {
  color: var(--ink);
  font-weight: 600;
}

@media (max-width: 760px) {
  .home-hero {
    grid-template-columns: 1fr;
    gap: 1.3rem;
    padding-top: .8rem;
  }

  .hero-photo {
    grid-row: 1;
    justify-self: start;
    width: 145px;
  }

  .research-item {
    grid-template-columns: 1fr;
    gap: .25rem;
  }

  .area-grid {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }
}
</style>

<section class="home-hero">
  <div>
    <p class="eyebrow">Machine Learning · Complex Systems</p>
    <h1 class="hero-name">Yeonju Lee</h1>
    <h2 class="hero-title">Knowledge-Informed Machine Learning for Complex Systems</h2>

    <p class="hero-description">
      I develop learning methods that integrate domain and scientific knowledge to improve reliability under limited data and changing environments.
    </p>

    <p class="hero-meta">
      Ph.D. Student in Machine Learning · H. Milton Stewart School of Industrial &amp; Systems Engineering · Georgia Institute of Technology
    </p>

    <div class="hero-links">
      <a href="/files/Yeonju_Lee_CV.pdf">CV</a>
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
      <a href="mailto:ylee845@gatech.edu">Email</a>
      <a href="/publications/">Publications</a>
    </div>
  </div>

  <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
</section>

<section class="home-section" id="selected-research">
  <p class="section-kicker">Selected Research</p>
  <h2 class="section-title">Recent and Representative Work</h2>

  <div class="research-item">
    <div class="research-status">Current research<br>Manuscript in preparation</div>
    <div>
      <p class="research-title">LLM-Guided Knowledge Alignment for Robust Learned Control in Complex Physical Systems</p>
      <p class="research-desc">Integrating scientific knowledge with learned control to improve robustness under changing physical environments.</p>
      <div class="research-tags">Knowledge alignment · Learned control · Distribution shift</div>
    </div>
  </div>

  <div class="research-item">
    <div class="research-status">2026<br>Revised manuscript under review</div>
    <div>
      <p class="research-title">SPADE: A Large Language Model Framework for Soil Moisture Pattern Recognition and Anomaly Detection in Precision Agriculture</p>
      <p class="research-desc">Using large language models with agronomic knowledge to analyze complex spatiotemporal soil-moisture patterns.</p>
      <div class="research-tags">Foundation models · Scientific data · Precision agriculture</div>
    </div>
  </div>

  <div class="research-item">
    <div class="research-status">2025<br>IEEE TASE</div>
    <div>
      <p class="research-title">Oral-Anatomical Knowledge-Informed Semi-Supervised Learning for 3D Dental CBCT Segmentation and Lesion Detection</p>
      <p class="research-desc">Embedding anatomical knowledge into semi-supervised learning to improve 3D medical-image learning with limited labels.</p>
      <div class="research-tags">Domain-guided learning · Limited labels · Medical imaging · IISE DAIS Best Paper Finalist</div>
    </div>
  </div>
</section>

<section class="home-section" id="research-areas">
  <p class="section-kicker">Research Areas</p>
  <h2 class="section-title">Research Themes</h2>

  <div class="area-grid">
    <div class="area">
      <h3>Knowledge-Informed Learning</h3>
      <p>Using domain and scientific knowledge as supervision, structure, and inductive bias when data alone are insufficient.</p>
    </div>
    <div class="area">
      <h3>Foundation Models for Scientific Reasoning</h3>
      <p>Using foundation models to represent and operationalize scientific knowledge in complex data.</p>
    </div>
    <div class="area">
      <h3>Robust Learning-Enabled Decision-Making</h3>
      <p>Developing learning methods for reliable decisions under limited data and changing environments.</p>
    </div>
  </div>
</section>

<section class="highlights">
  <p class="section-kicker">Selected Recognition</p>
  <p class="highlight-line">
    <strong>IISE DAIS Best Paper Finalist</strong> ·
    <strong>IISE Transactions on Healthcare Systems Engineering Monthly Spotlight</strong> ·
    <strong>2 U.S. Provisional Patent Applications</strong>
  </p>
</section>
