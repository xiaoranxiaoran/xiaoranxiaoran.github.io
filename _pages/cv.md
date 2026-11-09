---
layout: single
author_profile: true
title: Curriculum Vitae
permalink: /cv/
excerpt: Education, technical skills, projects, and honors of Yiran Li.
---

## Education

**Wuhan University of Technology**<br>
School of Artificial Intelligence<br>
Graduate Student, September 2026 – Present

**Wuhan Donghu University**<br>
Undergraduate Degree in Software Engineering · Sep 2024–Jun 2026

Selected coursework included operating systems, software architecture, big data analytics and development, Python programming, Java web development, and software testing.

## Technical Skills

- **Programming and web development** — Java, Python, Spring Boot, MyBatis, MyBatis-Plus
- **Data processing** — Linux, shell scripting, Hadoop, HiveQL, HBase, MySQL
- **Software quality** — Functional, performance, and security test design, SQL query tuning, and indexing

## Projects

{% assign projects = site.portfolio | sort: "order" %}
{% for project in projects %}
- [{{ project.title }}]({{ project.url | relative_url }}) · {{ project.period }}
{% endfor %}

## Honors and Qualifications

- Outstanding Graduate, 2026
- Third Prize (Provincial Level), Hubei Craftsman Cup Software Testing Competition, 2023
- Software Designer (Intermediate Level), Software Tester (Advanced Level), and College English Test Band 4 (CET-4)

{% if site.author.email or site.author.github %}
## Contact

{% if site.author.email %}
- [Email](mailto:{{ site.author.email }})
{% endif %}
{% if site.author.github %}
- [GitHub](https://github.com/{{ site.author.github }})
{% endif %}
{% endif %}
