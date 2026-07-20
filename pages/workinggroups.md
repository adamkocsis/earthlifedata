---
title: The Broader Community 
layout: page
show_sidebar: false
hero_image: "../images/heros/pexels-jeffrey-eisen-1257101-31749011.jpg"
permalink: /groups/
---

Here is a list of working groups that we are aware of that focus on some aspects of digital data in researching Earth-Life coevolution.  
 
{% for wg in site.data.projects %}
- [{{wg.long}}]({{wg.website}})

{% endfor %}
