---
layout: default
title: "Blog"
---

<div class="blog-list">
  <img src="/Imagenes/blog.jpg" alt="Listado de publicaciones" class="page-banner">
  
  <h1 class="blog-title">Últimas publicaciones</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li class="post-item">
        <a href="{{ post.url | relative_url }}" class="post-link">{{ post.title }}</a>
        <span class="post-date">— {{ post.date | date: "%d de %B de %Y" }}</span>
      </li>
    {% endfor %}
  </ul>

<a href="/" class="back-button">← Volver al inicio</a>

</div>
