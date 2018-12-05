---
layout: default
---
{% assign faction = page.title %}

{{ content }}



<h2>Notable Members</h2>
<table>
<tr>
<th>Member</th><th>Player</th>
{% for page in site.pages %}{% if page.categories contains faction and page.dnd == true %}
<tr>
<td>
<a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
</td>
<td>
{% if page.categories contains "pc" %}
{{ page.player }}
{% elsif page.categories contains "npc" %}
NPC
{% endif %}
</td>
</tr>
{% endif %}{% endfor %}
