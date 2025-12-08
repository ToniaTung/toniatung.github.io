---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% if page.project_start %}
  <i class="fa fa-calendar"></i>
  {{ page.project_start | date: "%b %Y" }}
  {% if page.project_end %}
    – {{ page.project_end | date: "%b %Y" }}
  {% endif %}
{% elsif page.date %}
  <i class="fa fa-calendar"></i>
  Published: {{ page.date | date: "%B %d, %Y" }}
{% endif %}
