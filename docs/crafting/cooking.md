---
dnd: true
categories: [crafting]
title: Cooking
layout: default
---

In an attempt to make the cooking skill interesting, below are known recipies.


Recipe | Effect |  Prep Time | Duration |
--- | --- | --- | --- |
{% for page in site.pages %}{% if page.categories contains "cooking" and page.categories contains "recipe" and page.dnd == true %}<a href="{{site.baseurl}}{{ page.url }}">{{ page.title }}</a>| {{ page. effect }} | {{ page.prep }} | {{ page.duration }}
{% endif %}{% endfor %}
