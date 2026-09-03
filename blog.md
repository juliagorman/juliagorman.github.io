---
layout: page
title: writing
subtitle: Science for general audiences, written for NeuWrite San Diego. Some of it in Spanish.
permalink: /blog/
wide: true
---

<div class="cards">
{% for post in site.data.posts %}
  <div class="card">
    <a class="card-link" href="{{ post.url }}">
      <span class="card-img"><img src="{{ post.image }}" alt="" loading="lazy"></span>
      <span class="card-title">{{ post.title }}</span>
    </a>
    <span class="card-meta">{{ post.date | date: "%B %Y" }}{% if post.spanish %} · <a href="{{ post.spanish }}">en español</a>{% endif %}</span>
  </div>
{% endfor %}
</div>

<p class="cards-foot">All posts live on <a href="https://neuwritesd.org/author/gormanjc/">NeuWrite SD</a>.</p>
