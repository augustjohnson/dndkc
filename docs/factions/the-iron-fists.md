---
dnd: true
categories: [faction]
name: The Iron Fists
title: The Iron Fists
alignment: Lawful Neutral
---

# The Iron Fists
The Iron Fists are a human faction (although a few half-orcs can be found among them), that absolutely hate magic in any form.  They arrest and detain any outward magic user, or kill anyone that uses magic against them.  They are a militant theocracy, with a huge standing army of well trained soldiers.  They are highly mistrustful of races that have inherent magic (elves, gnomes, genasi).  They do not spread their doctrine beyond their borders, and are rarely outwardly hostile.

## Roles and Ranks within the Iron Fists
* **Reclaimer** - Responsible for protection of Valmest, and the enforcement of it's laws.
* **High Reclaimer** - Responsible for the direction of the Iron Fists. Usually reclusive, and by tradition speaks almost exclusively with the Reclaimer.
* **Arcane Hunter** - Select few of the Iron Fists who are allowed to dabble in magic.  A highly regarded position and highly regulated.  Only approved schools of magic and spells are taught...all others are strictly forbidden.

## Notable Members

Name | Rank
--- | ---
{% for page in site.pages %}{% if page.categories contains "The Iron Fists" and page.dnd == true %}<a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a> | {{ page.fist_rank }}  
{% endif %}{% endfor %}
