---
layout: default
---
{% if page.image %}
<img src="{{ page.image }}"></img>
{% endif %}

<h1>{{ page.title }}</h1>

{{ content }}