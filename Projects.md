---
layout: page
title: "Project Portfolio"
---
 
<article>
**[AI/Machine Learning & Big Data](https://jacobyan0.github.io/aibigdata/)**

{% for post in site.categories.aibigdata %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Transit & New Mobility](https://jacobyan0.github.io/transitnewmobility/)**

{% for post in site.categories.transitnewmobility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Transport Equity](https://jacobyan0.github.io/equity/)**

{% for post in site.categories.equity %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Spatial Accessibility](https://jacobyan0.github.io/accessibility/)**

{% for post in site.categories.accessibility %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>

<br>

<article>
**[Travel Behavior](https://jacobyan0.github.io/travel behavior/)**

{% for post in site.categories.travelbehavior %}
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
{% endfor %}
</article>
