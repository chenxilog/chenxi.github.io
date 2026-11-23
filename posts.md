---
layout: page
title: 文章
permalink: /posts/
---

{% for post in site.posts %}
- **{{ post.date | date: "%Y-%m-%d" }}** · [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
