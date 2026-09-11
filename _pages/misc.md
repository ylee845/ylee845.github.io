---
layout: page
title: "Personal"
permalink: /misc/
---

<style>
/* Personal keeps a narrower reading measure but the same centering
   axis, gutter, and breakpoint as every other section. */
.personal-section {
  --l-max: 820px;
}

.personal-gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 0.8rem;
  margin-bottom: 1.2rem;
}

.personal-gallery img {
  width: 32%;
  min-width: 220px;
  border-radius: 8px;
  object-fit: cover;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.08);
  transition: transform 0.25s ease;
}

.personal-gallery img:hover {
  transform: scale(1.02);
}

.personal-section p {
  font-size: 1rem;
  line-height: 1.7;
  letter-spacing: -0.1px;
  color: var(--text);
  text-align: justify;
  margin: .4rem 0 1rem;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

.personal-section p .emoji {
  vertical-align: -0.1em;
  margin: 0 .08em;
}

@media (max-width: 760px) {
  .personal-gallery {
    flex-direction: column;
    align-items: center;
    gap: 0.75rem;
  }

  .personal-gallery img {
    width: 100% !important;
    max-width: 360px;
  }

  .personal-section p {
    text-align: left;
  }
}
</style>

<section class="personal-section l-shell">

  <div class="personal-gallery">
    <img src="/images/personal_hiking.jpg" alt="Hiking around Atlanta">
    <img src="/images/personal_knitting.jpg" alt="Knitting at home">
  </div>

  <p>
    In my free time, I enjoy playing racquetball, exploring hiking trails around Atlanta,
    and relaxing with some knitting. I like getting deeply absorbed in what I do and then taking time to relax and reset.
    That rhythm of immersion and relaxation gives me good energy and keeps me balanced.
    It is the same kind of flow I try to bring into my research.
  </p>
</section>
