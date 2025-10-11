---
layout: page
title: "Personal"
permalink: /misc/
---

<style>
.personal-section {
  max-width: 760px;
  margin: 1rem auto 2rem;
  padding: 0;
}

.personal-section h3 {
  margin: 0 0 1rem;
  font-size: 1.6rem;
  font-weight: 800;
  color: #111;
}

/* 이미지 그룹 */
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

/* 본문 */
.personal-section p {
  font-family: "Inter","Helvetica Neue",Arial,sans-serif;
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

/* 이모지 정렬 */
.personal-section p .emoji {
  vertical-align: -0.1em;
  margin: 0 .08em;
}

/* 모바일: 세로 배치 */
@media (max-width: 768px) {
  .personal-gallery {
    flex-direction: column;
    align-items: center;
  }
  .personal-gallery img {
    width: 90%;
    max-width: 420px;
  }
  .personal-section p {
    text-align: left;
  }
}
</style>

<section class="personal-section">
  <h3>Personal</h3>

  <!-- 이미지 3장 -->
  <div class="personal-gallery">
    <img src="/images/personal_hiking.jpg" alt="Hiking around Atlanta">
    <img src="/images/personal_knitting.jpg" alt="Knitting at home">
  </div>

  <p>
    In my free time, I enjoy playing 🎾 racquetball, going for 🏃‍♀️ runs, exploring 🥾 hiking trails around Atlanta,
    and relaxing with some 🧶 knitting. I like getting deeply absorbed in what I do and then taking time to relax and reset.
    That rhythm of immersion and relaxation gives me good energy and keeps me balanced.
    It is the same kind of flow I try to bring into my research.
  </p>
</section>

