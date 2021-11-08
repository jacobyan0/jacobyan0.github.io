---
layout: page
title: "Project Portfolio"
---
 
<article>
 <header><h2><a href="https://jacobyan0.github.io/aibigdata">AI/Machine Learning & Big Data</a></h2></header>
 
{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
<header><h2><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h2></header>
 **[Transit & New Mobility](https://jacobyan0.github.io/transitnewmobility)**

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Transport Equity](https://jacobyan0.github.io/equity)**

{% for post in site.categories.equity %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Spatial Accessibility](https://jacobyan0.github.io/accessibility)**

{% for post in site.categories.accessibility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Travel Behavior](https://jacobyan0.github.io/travelbehavior)**

{% for post in site.categories.travelbehavior %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
