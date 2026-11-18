---
layout: page
title: Дневник процесса
permalink: /journal/
---
{% for post in site.categories.diary %}
  <article class="post-item">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <time>{{ post.date | date: "%d.%m.%Y" }}</time>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
