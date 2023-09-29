---
title: Publications
layout: single
permalink: /publications/
author_profile: true
sidebar:
  nav: "publications"
---

{% if site.data.publications-selected %}
# Selected Publications
  {% include publications-selected.html %}
{% endif %}

{% if site.data.bibliography.parsed-website.publications-journal %}
  {% if site.data.publications-selected %}
***
  {% endif %}
  {% include publications.html title="International Journal Papers" list=site.data.bibliography.parsed-website.publications-journal %}
{% endif %}

{% if site.data.bibliography.parsed-website.publications-chapter %}
***
  {% include publications.html title="Book Chapters" list=site.data.bibliography.parsed-website.publications-chapter %}
{% endif %}

{% if site.data.bibliography.parsed-website.publications-preprint %}
***
  {% include publications.html title="Preprints" list=site.data.bibliography.parsed-website.publications-preprint %}
{% endif %}

{% if site.data.bibliography.parsed-website.publications-conference %}
***
  {% include publications.html title="International Conference Papers" list=site.data.bibliography.parsed-website.publications-conference %}
{% endif %}

{% if site.data.bibliography.parsed-website.publications-thesis %}
***
  {% include publications.html title="Theses" list=site.data.bibliography.parsed-website.publications-thesis %}
{% endif %}
