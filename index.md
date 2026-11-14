---
layout: default
title: Главная
---


Процесс важнее результата. Честность важнее красоты.

## Эпизоды

{% for post in site.posts %}
* [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%d.%m.%Y" }}
{% endfor %}
