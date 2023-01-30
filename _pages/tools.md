---
layout: single
title: "TOOOOOLS!"
permalink: /tools/
author_profile: true
classes: wide
---

<h1>Books!</h1>
{% for book in site.books %}

<figure>
    <a href="{{book.url}}"><img src="{{book.img}}" alt="{{book.name}}"></a>
    <figcaption>{{book.name}}</figcaption>
</figure>

{% endfor %}

<h1> Tools!</h1>
{% for tool in site.tools %}
  
  <figure>
    <a href="{{tool.url}}"><img src="{{tool.img}}" alt="{{tool.name}}" width="25%"></a>
    <figcaption>{{tool.name}}</figcaption>
</figure>

{% endfor %}