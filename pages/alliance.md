---
layout: page
title: The Alliance
permalink: /about/alliance/
show_sidebar: false
hero_image: "../../images/heros/pexels-photo-13010774.jpeg"
---



## Why is this model necessary

The research community that focuses on Earth-Life coevolution is incredibly fragmented for multiple reasons. Some of the causes for this fragmentation are rooted in our disciplinary history, some of the attrition of resources are more result of the way how academic research is rewarded. The goal of the ELDA community is to transcend the well-established publish-cite-recognize reward system that permeates the academic community, which is one othe main reasons for the fragemntation of the community, initiatives and resources. 

Compared to their immediate societal value and use, the most types of data that we need are very expensive. The financial costs of satisfying community's need for a globally integrated data system can only be fulfilled if we stand united as one when communicating our interests to the larger scienfic community. The purpose of the ELDA is to gather this critical mass. Since academics are primarily interested in writing scientific studies, the shortest way to build our community is to publish together, as one. 

## Coordination

{% assign i = 0 %}
{% assign basic = site.data.people | where: 'special', 'pi' %}
{% assign basic = basic | sort: 'last' %}
{% for person in basic %}
{% assign i = i | plus:1 %}
{% assign something = i | modulo:2 %}
{% if something == 1 %}
<div class="columns is-vcentered">
{% endif %}

<div class="column">
	<div class="box">
	<div class="columns">
		<div class="column is-3">
		<a href="{{person.webpage}}"><img src="{{site.url}}{{site.baseurl}}/images/people/{{person.image}}" style="border-radius:3%;border:1px solid #ddd"></a>
		</div>
		<div class="column">
		<h4 id="{{ person.first | append: " " | append: person.last | slugify }}"><a href="{{person.webpage}}">{{person.first}} {{person.last}}</a></h4>
		{{person.institute}}
		</div>
	</div>
	</div>
</div>

{% if something == 0 %}
</div>
{% endif %}
{% endfor %}

{% if something == 1 %}
<div class="column">
</div>
</div>
{% endif %}

## The future organization

As senior academics are universally overcommitted and early-career researchers are overburdened with publication pressure to maintain their academic affiliation, the onset phase of the Alliance is coordinated (for now) by late-early to mid-career researchers. We have been involved with data-related research through our entire careers and are aware of many issues that hinder the development of our digital collaboration. We also have experience in the coordination of large collaborations and would like to lay down the foundations for establishing a global-scale organization that takes responsibility for our joint interests and for future proofing the achievements of the community and for the democratization of our shared intellectual heritage.
