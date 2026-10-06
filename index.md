---
layout: default
title: Home
---

<h1>Articoli</h1>

{% for post in site.posts %}
<article class="post-preview">

  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </h2>

  <p class="post-date">
    {{ post.date | date: "%d/%m/%Y" }}
  </p>

  <p>
    {{ post.excerpt }}
  </p>

</article>
{% endfor %}