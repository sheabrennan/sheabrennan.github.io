---
layout: single
title: "Knots!"
permalink: /knots/
author_profile: true

---

>"No amount of theoretical knowledge in any of the arts or handicrafts can compensate for the lack of practical experience."

-- _Cifford Ashley_

I like knots for a lot of reasons, not the least of which is their practicality.  A few years ago I was gifted [Ashley's Book of Knots](/books/abok.html) and am looking for a way to transfer some of that awesome knowledge into my brain (and hands)

I'm going to give learning a subset (or several) of the knots a shot and we'll see what happens

{% assign tags =  site.knots | map: "focusgroup" | uniq %}

{% for tag in tags %}
<h1><a name="{{tag}}"> {{ tag }} </a></h1>

    {% assign knots = site.knots | where: "focusgroup", tag %}

{% for knot in knots %}
* <a href="{{knot.url}}">{{ knot.name }} - ABOK#{{ knot.aboknumber}}</a>
{% endfor %}

{% endfor %}



