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
#main, .page, .page__inner-wrap, .page__content {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 175px;
  gap: 2.8rem;
  align-items: center;
  padding: 1.1rem 0 1.8rem;
  border-bottom: 1px solid var(--line);
}

.hero-name {
  margin: 0 0 .2rem;
  color: var(--text);
  font-size: 2rem;
  font-weight: 600;
  line-height: 1.08;
}

.hero-meta {
  margin: 0 0 .95rem;
  color: var(--text-soft);
  font-size: .92rem;
  line-height: 1.5;
}

.hero-meta a {
  color: var(--text-soft);
  text-decoration: underline;
  text-decoration-color: #c5cbd0;
  text-underline-offset: 2px;
}

.hero-title {
  max-width: 690px;
  margin: 0 0 .7rem;
  color: var(--text);
  font-size: 1.42rem;
  font-weight: 600;
  line-height: 1.22;
}

.hero-description {
  max-width: 690px;
  margin: 0 0 .85rem;
  color: #3c4247;
  font-size: .96rem;
  line-height: 1.58;
}

.hero-links {
  margin: 0;
  color: var(--muted);
  font-size: .88rem;
  font-weight: 500;
}

.hero-links a { color: var(--accent); }

.hero-photo {
  width: 175px;
  height: 218px;
  justify-self: end;
  object-fit: cover;
  object-position: center;
}

.research-program {
  padding: 1.75rem 0 .8rem;
}

.research-label {
  margin: 0 0 1rem;
  color: var(--muted);
  font-size: .76rem;
  font-weight: 600;
  text-transform: uppercase;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 2.2rem;
}

.research-column {
  min-width: 0;
}

.research-stage {
  margin: 0 0 .26rem;
  color: var(--text);
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.3;
}

.research-focus {
  margin: 0 0 .45rem;
  color: var(--accent);
  font-size: .87rem;
  font-weight: 500;
  line-height: 1.4;
}

.research-description {
  margin: 0 0 .65rem;
  color: var(--text-soft);
  font-size: .85rem;
  line-height: 1.48;
}

.research-work {
  margin: 0;
  padding-top: .55rem;
  border-top: 1px solid #edf0f2;
  color: #555d64;
  font-size: .80rem;
  line-height: 1.4;
}

.research-work strong {
  color: #394047;
  font-weight: 500;
}

@media (max-width: 760px) {
  .home-hero {
    grid-template-columns: 1fr;
    gap: 1.1rem;
    padding-top: .7rem;
  }

  .hero-photo {
    grid-row: 1;
    justify-self: start;
    width: 135px;
    height: 168px;
  }

  .research-grid {
    grid-template-columns: 1fr;
    gap: 1.4rem;
  }
}
</style>

<section class="home-hero">
  <div>
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
      <a href="/files/Yeonju_Lee_CV.pdf">CV</a>
      &nbsp;·&nbsp;
      <a href="https://scholar.google.com/citations?user=5iO-_XgAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Google Scholar</a>
      &nbsp;·&nbsp;
      <a href="mailto:ylee845@gatech.edu">Email</a>
      &nbsp;·&nbsp;
      <a href="/publications/">Publications</a>
    </p>
  </div>

  <img class="hero-photo" src="/images/prof_headshot7.jpg" alt="Portrait of Yeonju Lee">
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
      <p class="research-work">
        <strong>Representative work:</strong> Oral-Anatomical Knowledge-Informed Semi-Supervised Learning
      </p>
    </div>

    <div class="research-column">
      <h3 class="research-stage">Reasoning</h3>
      <p class="research-focus">Knowledge-grounded scientific reasoning</p>
      <p class="research-description">
        Foundation models that use scientific knowledge to interpret complex spatiotemporal patterns.
      </p>
      <p class="research-work">
        <strong>Representative work:</strong> SPADE
      </p>
    </div>

    <div class="research-column">
      <h3 class="research-stage">Decision &amp; Control</h3>
      <p class="research-focus">Reliable learning-enabled decision-making</p>
      <p class="research-description">
        Knowledge-informed learning for robust decisions under changing physical environments.
      </p>
      <p class="research-work">
        <strong>Current work:</strong> LLM-Guided Knowledge Alignment for Robust Learned Control
      </p>
    </div>
  </div>
</section>
