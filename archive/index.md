---
layout: default
title: Архив эпизодов
---

<span class="meta-label">// ПОЛНАЯ ХРОНОЛОГИЯ</span>

# Архив проекта «Здесь был Буратино»

{% for post in site.posts %}
<div style="margin-bottom: 2rem; border-bottom: 1px dashed var(--line-color); padding-bottom: 1rem;">
  <span class="meta-label">{{ post.date | date: "%Y" }} // {{ post.date | date: "%d.%m" }}</span>
  <h3 style="margin: 0.5rem 0;"><a href="{{ post.url }}" style="text-decoration: none; color: inherit;">{{ post.title }}</a></h3>
  <p style="font-size: 0.9rem; color: #666;">{{ post.excerpt | strip_html | truncate: 150 }}</p>
</div>
{% endfor %}
