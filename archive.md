---
layout: page
title: 归档
permalink: /archive/
---

{% for post in site.posts %}
{% assign curyear = post.date | date: "%Y" %}
{% if curyear != prevyear %}
{% unless forloop.first %}</ul>{% endunless %}
<h2>{{ curyear }} 年</h2>
<ul>
{% assign prevyear = curyear %}
{% endif %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> &nbsp;·&nbsp; {{ post.date | date: "%m-%d" }}</li>
{% if forloop.last %}</ul>{% endif %}
{% endfor %}
