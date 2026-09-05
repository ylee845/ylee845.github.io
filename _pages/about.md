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
/* Homepage only */
:root {
  --gt-navy: #003057;
  --gt-gold: #B3A369;
  --ink: #202428;
  --text-soft-home: #4b545d;
  --muted-home: #6d747b;
  --card-bg: #fbfbfa;
  --card-line: #e4e7ea;
}

#main,
.page,
.page__inner-wrap,
.page__content {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

.page {
  float: none !important;
  width: 100% !important;
}

#main {
  max-width: none !important;
  padding-left: 0 !important;
  padding-right: 0 !important;
}

.page__content {
  width: 100% !important;
  max-width: none !important;
  margin: 0 auto !important;
}

.home-hero,
.research-program {
  width: min(1540px, calc(100vw - 56px));
  margin-left: auto !important;
  margin-right: auto !important;
}

/* ===== Hero ===== */
.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 250px;
  gap: 4rem;
  align-items: stretch;
  padding: 1.05rem 0 1.7rem;
  border-bottom: 1px solid #e7eaed;
}

.hero-copy {
  align-self: center;
}

.hero-name {
  margin: 0 0 .18rem;
  color: var(--ink);
  font-size: 1.95rem;
  font-weight: 600;
  line-height: 1.08;
}

.hero-meta {
  margin: 0 0 .82rem;
  color: #46515b;
  font-size: .91rem;
  line-height: 1.48;
}

.hero-meta a {
  color: var(--gt-navy);
  text-decoration: underline;
  text-decoration-color: #9db0bf;
  text-underline-offset: 2px;
}

.hero-title {
  max-width: 800px;
  margin: 0 0 .58rem;
  color: var(--gt-navy);
  font-size: 1.40rem;
  font-weight: 600;
  line-height: 1.22;
}

.hero-description {
  max-width: 800px;
  margin: 0 0 .34rem;
  color: #333b43;
  font-size: .95rem;
  line-height: 1.55;
}

.hero-applications {
  margin: 0 0 .72rem;
  color: #56616b;
  font-size: .84rem;
  line-height: 1.45;
}

.hero-applications strong {
  color: #3e474f;
  font-weight: 600;
}

.hero-links {
  margin: 0;
  color: #59636d;
  font-size: .87rem;
  font-weight: 500;
}

.hero-links a {
  color: var(--gt-navy);
}

.cv-updated {
  margin-left: .24rem;
  color: #7b838a;
  font-size: .72rem;
  font-weight: 400;
}

.hero-photo-wrap {
  width: 250px;
  height: 292px;
  overflow: hidden;
  justify-self: end;
  align-self: center;
}

.hero-photo {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  object-position: center 12%;
}

/* ===== Research program ===== */
.research-program {
  padding: 1.55rem 0 .9rem;
}

.research-label {
  margin: 0 0 .82rem;
  color: #5f6871;
  font-size: .74rem;
  font-weight: 600;
  text-transform: uppercase;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.6rem;
}

.research-card {
  position: relative;
  min-width: 0;
  background: var(--card-bg);
  border: 1px solid var(--card-line);
  border-radius: 4px;
  padding: 1.15rem 1.2rem 1.05rem;
}

.research-card::before {
  content: "";
  position: absolute;
  top: -1px;
  left: -1px;
  right: -1px;
  height: 3px;
  background: var(--gt-gold);
  border-radius: 4px 4px 0 0;
}

.research-stage {
  margin: .08rem 0 .2rem;
  color: var(--ink);
  font-size: 1.02rem;
  font-weight: 600;
  line-height: 1.28;
}

.research-focus {
  margin: 0 0 .48rem;
  color: var(--gt-navy);
  font-size: .88rem;
  font-weight: 600;
  line-height: 1.38;
}

.research-description {
  margin: 0 0 .8rem;
  color: var(--text-soft-home);
  font-size: .84rem;
  line-height: 1.48;
}

.research-paper {
  margin: 0;
  padding-top: .62rem;
  border-top: 1px solid #e4e7ea;
}

.research-paper-label {
  display: block;
  margin-bottom: .16rem;
  color: #867b4f;
  font-size: .68rem;
  font-weight: 600;
  text-transform: uppercase;
}

.research-paper-title {
  color: #353c43;
  font-size: .79rem;
  font-weight: 500;
  line-height: 1.4;
}

@media (max-width: 980px) {
  .page__content {
    max-width: 1120px !important;
  }

  .home-hero {
    grid-template-columns: minmax(0, 1fr) 205px;
    gap: 2.4rem;
  }

  .hero-photo-wrap {
    width: 220px;
    height: 275px;
  }

  .research-grid {
    gap: 1.4rem;
  }
}

@media (max-width: 760px) {
  .home-hero,
  .research-program {
    width: calc(100vw - 22px);
  }

  .home-hero {
    grid-template-columns: 1fr;
    gap: 1rem;
    padding-top: .7rem;
  }

  .hero-photo-wrap {
    grid-row: 1;
    justify-self: center;
    width: 230px;
    height: 288px;
    min-height: 0;
  }

  .research-program {
    width: auto;
    max-width: none;
    margin-left: 0;
    transform: none;
  }

  .research-grid {
    grid-template-columns: 1fr;
    gap: 1rem;
  }
}
</style>

<section class="home-hero">
  <div class="hero-copy">
    <h1 class="hero-name">Yeonju Lee</h1>

    <p class="hero-meta">
      Ph.D. Student in Machine Learning · Georgia Tech ISyE<br>
      Advised by <a href="https://isye.gatech.edu/users/jing-li" target="_blank" rel="noopener">Prof. Jing Li</a>
    </p>

    <h2 class="hero-title">Knowledge-Informed Machine Learning for Complex Systems</h2>

    <p class="hero-description">
      I develop learning methods that integrate domain and scientific knowledge to improve reliability under limited data and changing environments.
    </p>

    <p class="hero-applications">
      <strong>Applications:</strong> Healthcare · Precision Agriculture
    </p>

    <p class="hero-links">
      <a href="/files/Yeonju_Lee_CV.pdf">CV</a><span class="cv-updated">Last updated Sep 4, 2026</span>
      &nbsp;·&nbsp;
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
      &nbsp;·&nbsp;
      <a href="mailto:ylee845@gatech.edu">Email</a>
      &nbsp;·&nbsp;
      <a href="https://www.linkedin.com/in/ylee845" target="_blank" rel="noopener">LinkedIn</a>
    </p>
  </div>

  <div class="hero-photo-wrap">
    <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
  </div>
</section>

<section class="research-program">
  <p class="research-label">Research Areas</p>

  <div class="research-grid">
    <div class="research-card">
      <h3 class="research-stage">Representation</h3>
      <p class="research-focus">Knowledge-guided representation learning</p>
      <p class="research-description">
        Domain and anatomical knowledge for learning from limited and heterogeneous scientific data.
      </p>
      <p class="research-paper">
        <span class="research-paper-label">Representative paper</span>
        <span class="research-paper-title">
          Oral-Anatomical Knowledge-Informed Semi-Supervised Learning for 3D Dental CBCT Segmentation and Lesion Detection
        </span>
      </p>
    </div>

    <div class="research-card">
      <h3 class="research-stage">Reasoning</h3>
      <p class="research-focus">Knowledge-grounded scientific reasoning</p>
      <p class="research-description">
        Foundation models that use scientific knowledge to interpret complex spatiotemporal patterns.
      </p>
      <p class="research-paper">
        <span class="research-paper-label">Representative paper</span>
        <span class="research-paper-title">
          SPADE: A Large Language Model Framework for Soil Moisture Pattern Recognition and Anomaly Detection in Precision Agriculture
        </span>
      </p>
    </div>

    <div class="research-card">
      <h3 class="research-stage">Decision &amp; Control</h3>
      <p class="research-focus">Reliable learning-enabled decision-making</p>
      <p class="research-description">
        Knowledge-informed learning for robust decisions under changing physical environments.
      </p>
      <p class="research-paper">
        <span class="research-paper-label">Current paper</span>
        <span class="research-paper-title">
          LLM-Guided Knowledge Alignment for Robust Learned Control in Complex Physical Systems
        </span>
      </p>
    </div>
  </div>
</section>
