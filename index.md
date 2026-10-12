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

<h2 class="section-label">Projects</h2>

{% include catalogue.html %}

Click a card to know more about a project, or explore the [collection]({{ '/collection/' | relative_url }}) of all the Code, Models, Datasets for more details.
