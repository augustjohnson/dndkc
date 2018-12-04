# Factions

There exist many factions in the world.  Some are straight out of the PHB/DMG (such as the Thieves Guild), but others are unique to this world.  Notable examples below.

Faction Name | Alignment
--- | ---
{% for faction in site.factions %} <a href="{{site.base-url}}{{ faction.url }}"> {{ faction.name }} </a> | {{ faction.alignment }} 
{% endfor %}


{% for cat in site.category-list %}
### {{ cat }}
<ul>
  {% for page in site.pages %}
    {% if page.dnd == true %}
      {% for pc in page.categories %}
        {% if pc == cat %}
          <li><a href="{{ page.url }}">{{ page.title }}</a></li>
        {% endif %}   <!-- cat-match-p -->
      {% endfor %}  <!-- page-category -->
    {% endif %}   <!-- resource-p -->
  {% endfor %}  <!-- page -->
</ul>
{% endfor %}  <!-- cat -->