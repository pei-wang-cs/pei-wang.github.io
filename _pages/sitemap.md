---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A concise index of the public content on this site. An [XML sitemap]({{ base_path }}/sitemap.xml) is also available.

<h2>Pages</h2>

- [Home]({{ base_path }}/)
- [Publications]({{ base_path }}/publications/)
- [Curriculum Vitae]({{ base_path }}/cv/)

<h2>Publication Details</h2>

{% for publication in site.publications reversed %}
- [{{ publication.title }}]({{ base_path }}{{ publication.url }})
{% endfor %}
