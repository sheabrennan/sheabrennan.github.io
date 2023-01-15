---
layout: single
title: "TOOOOOLS!"
permalink: /tools/
author_profile: true
entries_layout: grid
---

Including books!



{% for tool in site.tools %}
  
  <figure>
    <a href="{{tool.url}}"><img src="{{tool.img}}" alt="{{tool.name}}"></a>
    <figcaption>{{tool.name}}</figcaption>
</figure>
  <p>{{ tool.content | markdownify }}</p>
{% endfor %}