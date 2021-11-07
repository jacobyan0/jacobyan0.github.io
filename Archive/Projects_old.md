---
layout: default
title: "Project Portfolio"
---

{% include nav.html %}

{% if site.show_excerpts %}
  {% include home.html %}
{% else %}
  {% include archive.html title="Posts" %}
{% endif %}
