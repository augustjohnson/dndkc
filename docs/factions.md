# Factions

There exist many factions in the world.  Some are straight out of the PHB/DMG (such as the Thieves Guild), but others are unique to this world.  Notable examples below.


Faction Name | Alignment
--- | ---
  {% for page in site.pages %}
    {% if page.dnd == true %}
      {% for pc in page.categories %}
        {% if pc == "faction" %}
          <a href="{{site-baseurl}}{{ page.url }}">{{ page.title }}</a> | {{page.alignment}}
        {% endif %}   <!-- cat-match-p -->
      {% endfor %}  <!-- page-category -->
    {% endif %}   <!-- resource-p -->
  {% endfor %}  <!-- page -->
