---
title: Earth-Life Data Catalogue 
layout: page
show_sidebar: false
permalink: /workinggroups/
---

A list of working groups: 
 
{% for wg in site.data.projects %}
- [{{wg.long}}]({{wg.website}})

{% endfor %}
