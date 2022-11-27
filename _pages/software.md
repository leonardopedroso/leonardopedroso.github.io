---
permalink: /software/
author_profile: true
---

{% if site.data.publications-selected %}
  {% include publications-selected.html %}
{% endif %}

{% if site.data.publications-journal %}
  {% if site.data.publications-selected %}
***
  {% endif %}
  {% include publications.html title="International Journal Papers" list=site.data.publications-journal %}
{% endif %}

{% if site.data.publications-chapter %}
***
  {% include publications.html title="Book Chapters" list=site.data.publications-chapter %}
{% endif %}

{% if site.data.publications-conference %}
***
  {% include publications.html title="International Conference Papers" list=site.data.publications-conference %}
{% endif %}

{% if site.data.publications-thesis %}
***
  {% include publications.html title="Theses" list=site.data.publications-thesis %}
{% endif %}
