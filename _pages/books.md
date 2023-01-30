---
layout: single
title: "Bookish things"
permalink: /books/
author_profile: true
entries_layout: grid
---
{% assign test = "#1" %} 
{% assign rank = site.books | where: "position", "#1" %}
{% for r in rank %}
<p> {{ r.position }} </p>
{% endfor %}
I understand Collections now!

(but there's still a todo for content)



{% for book in site.books %}
  <h2>{{ book.name }} - {{ book.position }}</h2>
  <p>{{ book.content | markdownify }}</p>
{% endfor %}