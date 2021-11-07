---
layout: default
title: "Project Portfolio"
---

{% include nav.html %}

<h3>AI/Machine Learning & Big Data</h3>

{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}

<h3>Transit & New Mobility</h3>

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
