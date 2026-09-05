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
/* Homepage palette: slightly brighter, still academic */
:root {
  --accent: #2f5f91;
  --accent-dark: #244c76;
  --ink-strong: #1f252b;
  --text-soft-home: #4c555e;
  --line-home: #e5e9ed;
}

#main,
.page,
.page__inner-wrap,
.page__content {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

.page__content {
  max-width: 1240px !important;
}

/* Hero */
.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 245px;
  gap: 3.6rem;
  align-items: stretch;
  padding: 1.1rem 0 1.8rem;
  border-bottom: 1px solid var(--line-home);
}

.hero-copy {
  align-self: center;
}

.hero-name {
  margin: 0 0 .18rem;
  color: var(--ink-strong);
  font-size: 2rem;
  font-weight: 600;
  line-height: 1.08;
}

.hero-meta {
  margin: 0 0 .9rem;
  color: #46515b;
  font-size: .92rem;
  line-height: 1.5;
}

.hero-meta a {
  color: var(--accent-dark);
  text-decoration: underline;
  text-decoration-color: #9fb5c8;
  text-underline-offset: 2px;
}

.hero-title {
  max-width: 760px;
  margin: 0 0 .65rem;
  color: var(--accent-dark);
  font-size: 1.42rem;
  font-weight: 600;
  line-height: 1.22;
}

.hero-description {
  max-width: 760px;
  margin: 0 0 .8rem;
  color: #333b43;
  font-size: .96rem;
  line-height: 1.58;
}

.hero-links {
  margin: 0;
  color: #59636d;
  font-size: .88rem;
  font-weight: 500;
}

.hero-links a {
  color: var(--accent);
}

.hero-links a:hover {
  color: var(--accent-dark);
}

.cv-updated {
  margin-left: .28rem;
  color: #7a838b;
  font-size: .74rem;
  font-weight: 400;
}

.hero-photo-wrap {
  width: 245px;
  height: 100%;
  min-height: 285px;
  overflow: hidden;
  justify-self: end;
  align-self: stretch;
}

.hero-photo {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  object-position: center top;
}

/* Research program */
.research-program {
  padding: 1.65rem 0 .8rem;
}

.research-label {
  margin: 0 0 .95rem;
  color: #5d6974;
  font-size: .76rem;
  font-weight: 600;
  text-transform: uppercase;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 3.5rem;
}

.research-column {
  min-width: 0;
}

.research-stage {
  margin: 0 0 .22rem;
  color: var(--ink-strong);
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.3;
}

.research-focus {
  margin: 0 0 .38rem;
  color: var(--accent);
  font-size: .87rem;
  font-weight: 600;
  line-height: 1.4;
}

.research-description {
  margin: 0 0 .62rem;
  color: var(--text-soft-home);
  font-size: .84rem;
  line-height: 1.46;
}

.research-paper {
  margin: 0;
  padding-top: .52rem;
  border-top: 1px solid var(--line-home);
  color: #4a535c;
  font-size: .79rem;
  line-height: 1.42;
}

.research-paper-label {
  display: block;
  margin-bottom: .12rem;
  color: var(--accent);
  font-size: .70rem;
  font-weight: 600;
  text-transform: uppercase;
}

.research-paper-title {
  color: #313941;
  font-weight: 500;
}

@media (max-width: 900px) {
  .page__content {
    max-width: 1040px !important;
  }

  .home-hero {
    grid-template-columns: minmax(0, 1fr) 200px;
    gap: 2.2rem;
  }

  .hero-photo-wrap {
    width: 200px;
  }

  .research-grid {
    gap: 2rem;
  }
}

@media (max-width: 760px) {
  .home-hero {
    grid-template-columns: 1fr;
    gap: 1rem;
    padding-top: .7rem;
  }

  .hero-photo-wrap {
    grid-row: 1;
    justify-self: start;
    width: 150px;
    height: 188px;
    min-height: 0;
  }

  .research-grid {
    grid-template-columns: 1fr;
    gap: 1.35rem;
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

    <p class="hero-links">
      <a href="/files/Yeonju_Lee_CV.pdf">CV</a><span class="cv-updated">Last updated Sep 4, 2026</span>
      &nbsp;·&nbsp;
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
      &nbsp;·&nbsp;
      <a href="mailto:ylee845@gatech.edu">Email</a>
      &nbsp;·&nbsp;
      <a href="/publications/">Publications</a>
    </p>
  </div>

  <div class="hero-photo-wrap">
    <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
  </div>
</section>

<section class="research-program">
  <p class="research-label">Research Program</p>

  <div class="research-grid">
    <div class="research-column">
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

    <div class="research-column">
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

    <div class="research-column">
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
