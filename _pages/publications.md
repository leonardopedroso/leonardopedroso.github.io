---
permalink: /publications/
author_profile: true
---

{% if site.data.publications-featured %}
  {% include publications-featured.html %}
{% endif %}

{% if site.data.publications-journal %}
  {% if site.data.publications-featured %}
***
  {% endif %}
  {% include publications.html title="International Jounal Papers" list=site.data.publications-journal %}
{% endif %}

{% if site.data.publications-chapter %}
***
  {% include publications.html %}
{% endif %}


{% if site.data.publications-conference %}
***
  {% include publications.html %}
{% endif %}
