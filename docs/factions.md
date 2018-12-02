# Factions

There exist many factions in the world.  Some are straight out of the PHB/DMG (such as the Thieves Guild), but others are unique to this world.  Notable examples below.

Faction Name | Alignment
--- | ---
{% for faction in site.factions %} <a href="{{ faction.url }}"> {{ faction.name }} </a> | {{ faction.alignment }} {% endfor %}
