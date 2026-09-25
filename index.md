---
layout: default
title: Home
---
<section class="hero">
  <h1>Building AI that ships.</h1>
  <p class="lede">I'm <strong>Liang Gou</strong>, Director of AI Engineering at Cisco. I write about machine learning, engineering leadership, and what it takes to turn research into products people use.</p>
  {% include subscribe-form.html %}
</section>

<section class="recent">
  <h2>Latest writing</h2>
  {% for post in site.posts limit:5 %}
  <article class="post-card">
    <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </article>
  {% endfor %}
  <p><a href="{{ '/archive/' | relative_url }}">Browse the archive →</a></p>
</section>
