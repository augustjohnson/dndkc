---
---
# Crafting

In an effort to create some new and fun things to do, this section will expand upon the crafting system already laid out in the 5e rules



| Craft Name |
| --- |
{% for page in site.pages %}{% if page.categories contains "crafting" %}| <a href="{{site.baseurl}}{{ page.url }}">{{ page.title }}</a> |{% endif %}{% endfor %}
