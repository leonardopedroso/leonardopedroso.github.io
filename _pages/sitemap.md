---
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

# Sitemap

A list of all the posts and pages found on the site. For you robots out there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

## Pages
{% for page in site.pages %}{% if page.title %}{% if page.sitemap %}
- [{{page.title}}](page.permalink){% endif %}{% endif %}{% endfor %}

## Posts
{% for post in site.posts %}{% if post.title %}{% if post.sitemap %}
- [{{post.title}}](post.permalink){% endif %}{% endif %}{% endfor %}
