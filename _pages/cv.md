---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Machine Learning, Georgia Institute of Technology, 2027 (expected)
* M.S. in Industrial Engineering, Yonsei University, 2022
* B.S. in Information and Industrial Engineering, Yonsei University, 2021

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  {% include base_path %}

  <h2>Teaching</h2>
  <div class="teach-list">
    {% assign teachs = site.teaching | sort: "date" | reverse %}
    {% for t in teachs %}
      <div class="teach">
        <div class="left">
          <div><span class="role">{{ t.role }}</span> at {{ t.institution }}</div>
          <div class="course">
            {{ t.course }}{% if t.code %} ({{ t.code }}){% endif %}
          </div>
          {% if t.note %}<div class="note">{{ t.note }}</div>{% endif %}
        </div>
        <div class="term">{{ t.term }}</div>
      </div>
    {% endfor %}
</div>
  
Service and leadership
======
* Member in Institute of Industrial and Systems Engineers (IISE)
* Member in Institute for Operations Research and the Management Sciences (INFORMS)
* Reviewer for IEEE TASE
