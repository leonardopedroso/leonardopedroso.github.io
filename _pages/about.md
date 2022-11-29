---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<h1>About me</h1>
{{ site.data.author.author.about-me}}

{% if site.data.news %}
***
  {% include news.html %}
{% endif %}

{% if site.data.publications-selected %}
***
  {% include publications-selected.html %}
{% endif %}
