---
layout: default
title: 站点地图
permalink: /sitemap/
---

<main class="profile-shell profile-subpage" id="profile-main">
  <header class="profile-page-head">
    <p class="profile-kicker">SITEMAP</p>
    <h1>站点地图</h1>
  </header>
  <ul>
    <li><a href="{{ '/' | relative_url }}">首页</a></li>
    <li><a href="{{ '/projects/' | relative_url }}">项目经历</a>
      <ul>
        {% assign projects = site.portfolio | sort: "order" %}
        {% for project in projects %}
        <li><a href="{{ project.url | relative_url }}">{{ project.title }}</a></li>
        {% endfor %}
      </ul>
    </li>
    <li><a href="{{ '/cv/' | relative_url }}">个人履历</a></li>
  </ul>
</main>
