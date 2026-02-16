---
layout: default
title: Blog
permalink: /blog/
---

# Blog

<p class="tagline">Research notes, technical writing, and occasional dispatches from the lab.</p>

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <br>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
{% else %}

Nothing published yet. We're writing. Check back.

{% endif %}
