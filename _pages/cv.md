---
layout: default
title: 个人履历
permalink: /cv/
excerpt: 李屹然的教育背景、专业技能、项目经历、资格证书与荣誉。
---

<main class="profile-shell profile-subpage" id="profile-main">
  <header class="profile-page-head">
    <p class="profile-kicker">CURRICULUM VITAE</p>
    <h1>个人履历</h1>
    <p class="profile-intro">李屹然 · 软件工程本科</p>
  </header>
  <div class="profile-prose" markdown="1">
## 教育背景

**武汉东湖学院 · 软件工程（本科）** · 2024.09–2026.06

主修课程包括操作系统原理、软件体系架构、大数据分析与开发、Python 程序设计、Java Web 工程和软件测试技术。

## 技术能力

- **编程与 Web 开发**　Java、Python、Spring Boot、MyBatis、MyBatis-Plus
- **数据处理**　Linux、Shell、Hadoop、HiveQL、HBase、MySQL
- **软件质量**　功能、性能与安全测试用例设计，SQL 查询与索引优化

## 项目经历

{% assign projects = site.portfolio | sort: "order" %}
{% for project in projects %}
- [{{ project.title }}]({{ project.url | relative_url }}) · {{ project.period }}
{% endfor %}

## 证书与荣誉

- 2026 年优秀毕业生
- 2023 年湖北“工匠杯”软件测试大赛省级三等奖
- 中级软件设计师、高级软件测试员、大学英语四级（CET-4）

{% if site.author.email or site.author.github %}
## 联系方式

{% if site.author.email %}
- [电子邮件](mailto:{{ site.author.email }})
{% endif %}
{% if site.author.github %}
- [GitHub](https://github.com/{{ site.author.github }})
{% endif %}
{% endif %}
  </div>
</main>
