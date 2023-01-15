---
layout: single
title: "Bookish things"
permalink: /books/
author_profile: true
entries_layout: grid
---

I understand Collections now!

(but there's still a todo for content, but...)

{% for book in site.books %}
  <img src="{{book.img}}">
  <h2>{{ book.name }} - {{ book.position }}</h2>
  <p>{{ book.content | markdownify }}</p>
{% endfor %}