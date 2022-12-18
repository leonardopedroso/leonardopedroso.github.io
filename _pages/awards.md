---
title: Awards
layout: single
permalink: /awards/
author_profile: true
---

{% include if-empty-message list=site.data.awards %}

{% if site.data.awards-selected %}
# Selected awards
{% include awards-selected.html  %}
{% endif %}

***

# Awards and Achievements
{% assign sorted_awards = site.data.awards | sort: "date" %}{% assign current_year = 0 %}{% for item in sorted_awards reversed %}{% assign item_year = item.date | date:"%Y" %}{% if item_year != current_year %}{% assign current_year = item_year %}

## {{current_year}}
{% endif %}
- {{item.title}}{% if item.read_more %} [Read more...]({{item.read_more}}){:target="_blank"}{% endif %}{% endfor %}
