---
title:
layout: single
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<meta name="description" content="Leonardo Pedroso's personal academic website.">

<h1>👋 About me</h1>
{{ site.data.author.author.about-me}}

{% if site.data.news %}
***
# 📣 News
  {% include news.html %}
{% endif %}

{% if site.data.publications-selected %}
***
# 📰 Selected Publications
  {% include publications-selected.html %}
{% endif %}


{% if site.data.awards-selected %}
***
# 🏅 Selected awards
{% include awards-selected.html  %}
{% endif %}
