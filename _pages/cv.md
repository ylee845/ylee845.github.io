---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}
<div style="margin-top: 1.5rem;">
  <p style="margin-top:0.8rem; text-align:left;">
    <a href="/files/Yeonju_Lee_CV.pdf"
       style="text-decoration:underline; font-weight:600; color:#4169E1;">
       📄 Download full CV (PDF)
    </a>
  </p>

  <!-- 데스크탑용 CV 뷰어 -->
  <div style="text-align:center;">
    <iframe
      src="/files/Yeonju_Lee_CV.pdf#zoom=page-width&view=FitH"
      style="
        border:none;
        box-shadow: 0 2px 10px rgba(0,0,0,0.15);
        margin-top: 1rem;
        width: 80%;
        height: 950px;
        max-width: 1000px;
      "
    ></iframe>
  </div>
</div>

<!-- 모바일 전용 -->
<div style="text-align:center;">
  <iframe
    src="/files/Yeonju_Lee_CV.pdf#zoom=page-fit"
    style="
      display:none;
      border:none;
      width: 95%;
      height: 600px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    "
    id="cv-mobile"
  ></iframe>
</div>

<script>
  // 모바일 화면이면 자동으로 작은 iframe만 보여줌
  if (window.innerWidth < 880) {
    document.querySelector('iframe[style*="width: 80%"]').style.display = 'none';
    document.querySelector('#cv-mobile').style.display = 'block';
  }
</script>


