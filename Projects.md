---
layout: page
title: "Project Portfolio"
---
 
<article>
 <header><h3><a href="https://jacobyan0.github.io/aibigdata">AI/Machine Learning & Big Data</a></h3></header>
 
{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
  <header><h3><a href="https://jacobyan0.github.io/transitnewmobility">Transit & New Mobility</a></h3></header>

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
 <header><h3><a href="https://jacobyan0.github.io/equity">Transport Equity</a></h3></header>

{% for post in site.categories.equity %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
 <header><h3><a href="https://jacobyan0.github.io/accessibility">Spatial Accessibility</a></h3></header>

{% for post in site.categories.accessibility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
 <header><h3><a href="https://jacobyan0.github.io/travelbehavior">Travel Behavior</a></h3></header>

{% for post in site.categories.travelbehavior %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
