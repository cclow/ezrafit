---
layout: single
title: Testimonies
permalink: "/testimonies/"
---
{% for testimony in site.testimonies %}
  <h2>
    <a href="{{ testimony.url }}">
      {{ testimony.person }}
      {% if testimony.born %}
        : {{ testimony.born }}
      {% endif %}
    </a>
  </h2>
  {{ testimony.content | markdownify }}
{% endfor %}