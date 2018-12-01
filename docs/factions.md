{% for faction in site.factions %}
* <a href="{{ faction.url }}">{{ faction.name }}</a>
{% endfor %}