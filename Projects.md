---
layout: page
title: "Project Portfolio"
---
 
<article>
<h2>[AI/Machine Learning & Big Data](https://jacobyan0.github.io/aibigdata/)</h2>

{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
<h2>[Transit & New Mobility](https://jacobyan0.github.io/transitnewmobility/)</h2>

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
<h2>[Transport Equity](https://jacobyan0.github.io/equity/)</h2>

{% for post in site.categories.equity %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

* [Spatial accessibility](https://jacobyan0.github.io/accessibility/)

<article>
<h2>[Spatial Accessibility](https://jacobyan0.github.io/accessibility/)</h2>

{% for post in site.categories.accessibility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
<h2>[Travel Behavior](https://jacobyan0.github.io/travel behavior/)</h2>

{% for post in site.categories.travelbehavior %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
