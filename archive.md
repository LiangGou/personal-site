---
layout: default
title: Archive
permalink: /archive/
---

# Archive

{% for post in site.posts %}
- {{ post.date | date: '%Y-%m-%d' }} — [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
