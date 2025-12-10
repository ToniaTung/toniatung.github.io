---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
collection: portfolio
---
{% include base_path %}

{% assign projects = site.portfolio | sort: "order" %}
{% for post in projects %}
  {% include archive-single.html %}
{% endfor %}

