---
title: Software
layout: single
permalink: /software/
author_profile: true
---

{% include if-empty-message list=site.data.software %}
{% include software.html %}

***

{% if site.data.settings.software.github_profile %}
<h1>GitHub Profile</h1><br>
<img src="https://github-readme-stats.vercel.app/api?username={{site.data.settings.software.github_profile}}&show_icons=true&theme=dark" width ="54%"  >
<img src="https://github-readme-stats.vercel.app/api/top-langs?username={{site.data.settings.software.github_profile}}&theme=dark&layout=compact" width ="45%">
{% endif %}
