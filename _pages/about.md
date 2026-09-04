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
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Source+Serif+4:opsz,wght@8..60,500;8..60,600&display=swap');

:root {
  --ink: #17191c;
  --muted: #626a73;
  --accent: #31577a;
  --line: #e4e7ea;
}

.sidebar, .page__sidebar { display: none !important; }
.page__content { float: none !important; width: 100% !important; }

.page__content {
  max-width: 1120px !important;
  margin: 0 auto !important;
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  color: var(--ink);
  font-size: 16px;
  line-height: 1.65;
}

.page__content a {
  color: var(--accent);
  text-decoration: none;
}

.page__content a:hover { text-decoration: underline; }

.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1.6fr) minmax(210px, .62fr);
  gap: 4.5rem;
  align-items: center;
  padding: 3.8rem 0 3.5rem;
  border-bottom: 1px solid var(--line);
}

.eyebrow {
  margin: 0 0 .85rem;
  color: var(--muted);
  font-size: .82rem;
  font-weight: 600;
  letter-spacing: .08em;
  text-transform: uppercase;
}

.hero-name {
  margin: 0 0 .55rem;
  font-family: 'Source Serif 4', Georgia, serif;
  font-size: clamp(2.35rem, 5vw, 4.15rem);
  font-weight: 600;
  line-height: 1.02;
  letter-spacing: -.035em;
  color: var(--ink);
}

.hero-title {
  margin: 0 0 1.25rem;
  font-family: 'Source Serif 4', Georgia, serif;
  font-size: clamp(1.45rem, 2.7vw, 2.15rem);
  font-weight: 500;
  line-height: 1.2;
  letter-spacing: -.018em;
  color: var(--accent);
  max-width: 760px;
}

.hero-description {
  max-width: 720px;
  margin: 0 0 1.15rem;
  color: #34393f;
  font-size: 1.02rem;
  line-height: 1.7;
}

.hero-meta {
  margin: 0 0 1.35rem;
  color: var(--muted);
  font-size: .94rem;
}

.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: .55rem;
}

.hero-links a {
  display: inline-block;
  padding: .48rem .78rem;
  border: 1px solid #ccd2d7;
  border-radius: 3px;
  color: #253340;
  font-size: .88rem;
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
  max-width: 255px;
  justify-self: end;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  object-position: center;
}

.home-section {
  padding: 3rem 0 2.5rem;
  border-bottom: 1px solid var(--line);
}

.section-kicker {
  margin: 0 0 .55rem;
  color: var(--muted);
  font-size: .78rem;
  font-weight: 600;
  letter-spacing: .08em;
  text-transform: uppercase;
}

.section-title {
  margin: 0 0 1.8rem;
  font-family: 'Source Serif 4', Georgia, serif;
  font-size: 1.85rem;
  font-weight: 600;
  color: var(--ink);
  letter-spacing: -.018em;
}

.research-item {
  display: grid;
  grid-template-columns: 150px minmax(0, 1fr);
  gap: 1.5rem;
  padding: 1.45rem 0;
  border-top: 1px solid var(--line);
}

.research-item:first-of-type { border-top: 0; padding-top: 0; }

.research-status {
  color: var(--muted);
  font-size: .82rem;
  font-weight: 600;
  line-height: 1.5;
}

.research-title {
  margin: 0 0 .4rem;
  font-size: 1.06rem;
  font-weight: 650;
  line-height: 1.45;
  color: var(--ink);
}

.research-desc {
  margin: 0;
  color: #4f565d;
  font-size: .93rem;
  line-height: 1.6;
}

.research-tags {
  margin-top: .55rem;
  color: var(--accent);
  font-size: .79rem;
  font-weight: 600;
}

.area-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2.1rem;
}

.area h3 {
  margin: 0 0 .55rem;
  color: var(--ink);
  font-size: 1rem;
  font-weight: 650;
}

.area p {
  margin: 0;
  color: var(--muted);
  font-size: .9rem;
  line-height: 1.6;
}

.highlights {
  padding: 2.4rem 0 1.2rem;
}

.highlight-line {
  margin: 0;
  color: #4f565d;
  font-size: .9rem;
  line-height: 1.8;
}

.highlight-line strong { color: var(--ink); font-weight: 600; }

@media (max-width: 760px) {
  .home-hero {
    grid-template-columns: 1fr;
    gap: 2rem;
    padding-top: 2rem;
  }

  .hero-photo {
    grid-row: 1;
    justify-self: start;
    width: 155px;
  }

  .research-item { grid-template-columns: 1fr; gap: .35rem; }
  .area-grid { grid-template-columns: 1fr; gap: 1.6rem; }
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
    <div class="research-status">2026<br>Computers and Electronics in Agriculture</div>
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
  <h2 class="section-title">How I Approach Scientific Machine Learning</h2>

  <div class="area-grid">
    <div class="area">
      <h3>Knowledge-Informed Learning</h3>
      <p>Using domain and scientific knowledge as supervision, structure, and inductive bias when data alone are insufficient.</p>
    </div>
    <div class="area">
      <h3>Foundation Models for Scientific Data</h3>
      <p>Leveraging foundation models to represent and operationalize domain knowledge in complex scientific data.</p>
    </div>
    <div class="area">
      <h3>Reliable Learning for Complex Systems</h3>
      <p>Developing models that remain useful under limited data, heterogeneity, and changing deployment environments.</p>
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
