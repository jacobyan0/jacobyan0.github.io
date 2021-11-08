---
layout: page
title: "Project Portfolio"
---
 
<article>
<h3>AI/Machine Learning & Big Data</h3>

{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
 
<article>
<h3>Transit & New Mobility</h3>

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
