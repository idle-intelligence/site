---
layout: default
title: Home
wide: true
---

<div class="title-row">
  <img src="{{ '/assets/logo.jpeg' | relative_url }}" alt="" class="title-logo">
  <h1>Idle Intelligence</h1>
</div>

<p class="lead">{{ site.description }}</p>

<h2 class="section-label">Collection</h2>

{% include catalogue.html %}
