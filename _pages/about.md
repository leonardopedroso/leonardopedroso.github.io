---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<h1>About me</h1>
{{ site.data.author.author.about-me}}

***

{% if site.data.news %}
  {% include news.html %}
{% endif %}

***

Featured
======
Lorem ipsum

***

Selected publications
======
Lorem ipsum

***

Awards
======
