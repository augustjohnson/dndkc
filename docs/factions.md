
Here is a list of all of the factions currently specced out.
{% for faction in site.factions %}
* <a href="{{ faction.url }}">{{ faction.name }}</a>
{% endfor %}