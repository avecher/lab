---
layout: page
title: Эпизоды фабулы
permalink: /episodes/
---
{% for post in site.categories.episodes %}
  <article class="post-item">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <time>{{ post.date | date: "%d.%m.%Y" }}</time>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
