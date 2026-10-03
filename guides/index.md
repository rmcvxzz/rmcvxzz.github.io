---
layout: page
title: Guides
permalink: /guides/
---

Hey! Welcome to the page containing all the list of my silly instructions/guides.

It isn't really finished yet, so enjoy 2 guides, i guess.

*"Pick one, read one, replicate one."* -rmcvxzz, 2026

<ul>
{% assign guides = site.pages | where_exp: "p", "p.path contains 'guides/'" | where_exp: "p", "p.name != 'index.md'" | sort: "title" %}
{% for g in guides %}
  <li><a href="{{ site.baseurl }}{{ g.url }}">{{ g.title }}</a>{% if g.description %} - {{ g.description }}{% endif %}</li>
{% endfor %}
</ul>