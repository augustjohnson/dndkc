---
tags: sitemap
---
## The World
Please visit [The World](places/the-world) for a world map.
If you're interested in world history, please visit the [history](history/world-history) page.

## Places
There are many places in the world, (and growing all the time).  Some highlights include:
{% for page in site.pages %}
{% if page.categories contains "place" %}
* [{{ page.title }}]({{ site.baseurl }}/{{ page.url}})
{% endif %}
{% endfor %}

### The Western Continent
The western continent is fairly well contained and has four mountain ranges and five major rivers.  It is well settled and has few truly wild areas.

### The Eastern Continents
The Northern island has a central mountain range (the Frebrand range) and many islands (mostly parts of the Orcish Isles).  It stretches from the Northcrown, a cold wasteland to the Strait of Agnuan seperating it from the Southern Island.

The southern island has a small central mountain range as well, and is home to both the corruption and the High Elves.


## People
The inhabitants of this world are what make it interesting.  Notable inhabitants can be found in the /people folder.  Here are a few examples.
* [Fookwire](people/fookwire), the NPC Magic Item Salesman.
* [The Flotterclan Family](people/the_flotterclan_family.md), a family of Dwarven Nobles.
* [Ra'jur](people/rajur), a fiend, vanquished by the High Flyers during the Sixdays War.

### Factions
See the [Factions](factions) page for more information.

### Player Characters
{% for page in site.pages %}
{% if page.categories contains "pc" %}
* [{{ page.title }}]({{ site.baseurl }}/{{ page.url}})
{% endif %}
{% endfor %}

### Recurring NPCs
{% include npc.html %}


### Crafting
See the [Crafting](crafting) page for more information
