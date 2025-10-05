---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

<style>
/* ===== CV 페이지 전용 스타일 ===== */
.cv-container {
  margin-top: 1.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.cv-link {
  margin-top: 0.8rem;
  font-weight: 600;
  color: #4169E1;
  text-decoration: underline;
}

.cv-iframe {
  width: 90%;
  height: 1000px;
  border: none;
  box-shadow: 0 2px 10px rgba(0,0,0,0.15);
  margin-top: 1rem;
  border-radius: 8px;
}

/* ===== 모바일 대응 ===== */
@media (max-width: 768px) {
  .cv-iframe {
    width: 100%;
    height: 600px;         /* 세로 길이 축소 */
  }
  .cv-container {
    padding: 0 0.5rem;     /* 좌우 여백 추가로 깔끔하게 */
  }
  .cv-link {
    font-size: 1rem;
  }
}
</style>

<div class="cv-container">
  <p>
    <a href="/files/Yeonju_Lee_CV.pdf" class="cv-link">
      📄 Download full CV (PDF)
    </a>
  </p>

  <iframe
    src="/files/Yeonju_Lee_CV.pdf"
    class="cv-iframe">
  </iframe>
</div>


