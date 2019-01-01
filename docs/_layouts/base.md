---
layout: default
---
{% assign title = page.title | downcase %}

{{ content }}

<h2>Related Content</h2>
<table>
{% for page in site.pages %}{% if page.tags contains title and page.dnd == true %}
<tr>
<td><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></td>
</tr>
{% endif %}{% endfor %}
{% for tag in page.tags %}
{% for p in site.pages %}
{% assign title = p.title | downcase %}
{% if title contains tag %}<tr>
<td><a href="{{ site.url }}/{{ p.url }}">{{ p.title }}</a></td>
</tr>{% endif %}{% endfor %}
{% endfor %}
</table>
