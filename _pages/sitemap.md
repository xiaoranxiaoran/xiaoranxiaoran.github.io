---
layout: single
title: Sitemap
permalink: /sitemap/
---

- [Home]({{ '/' | relative_url }})
- [Projects]({{ '/projects/' | relative_url }})
{% assign projects = site.portfolio | sort: "order" -%}
{% for project in projects -%}
  - [{{ project.title }}]({{ project.url | relative_url }})
{% endfor -%}
- [Curriculum Vitae]({{ '/cv/' | relative_url }})
