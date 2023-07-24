---
layout: single
title: Testimonies
permalink: "/testimonies/"
---
{% for testimony in site.testimonies %}
  <h2>
    <a href="{{ testimony.url }}">
      {{ testimony.person }}, born {{ testimony.born }}
    </a>
  </h2>
  {{ testimony.content | markdownify }}
{% endfor %}