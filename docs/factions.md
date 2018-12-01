Below is a list of factions.
{% for faction in site.factions %}
* <a href="{{ faction.url }}"> {{ faction.name }} </a>
{% endfor %}

Below is a list of collections.
{% for collection in site.collections %}
* {{ collection.name }}
{% endfor %}