---
layout: default
title: 关于我
permalink: /
excerpt: 李屹然的软件工程主页。关注 Java 后端开发、软件质量与人工智能可信安全。
---

<main class="profile-shell" id="profile-main">
  <section class="profile-hero" aria-labelledby="profile-name">
    <div>
      <p class="profile-kicker"><span class="profile-dot"></span> SOFTWARE ENGINEERING</p>
      <h1 id="profile-name">李屹然</h1>
      <p class="profile-roman" lang="en">YIRAN LI</p>
      <p class="profile-lead">软件工程本科 · Java 后端开发与软件测试</p>
      <p class="profile-intro">毕业于武汉东湖学院软件工程专业。我做过高校讲座预约系统和用户行为数据分析，关注接口设计、并发下的数据一致性，以及如何通过测试验证系统行为。</p>
      <div class="profile-actions">
        <a class="profile-button" href="{{ '/projects/' | relative_url }}">查看项目 <span aria-hidden="true">↗</span></a>
        <a class="profile-secondary" href="{{ '/cv/' | relative_url }}">个人履历 <span aria-hidden="true">→</span></a>
      </div>
    </div>
    <figure class="profile-figure">
      <img src="{{ '/images/booking-flow.svg' | relative_url }}" width="520" height="340" alt="讲座预约链路示意图。用户发起预约请求，服务校验权限与名额，再通过事务和乐观锁写入预约记录。">
      <figcaption><span>FIG. 01</span> 讲座预约系统 · 预约链路示意</figcaption>
    </figure>
  </section>

  <section class="profile-section" aria-labelledby="projects-heading">
    <div class="profile-section-head">
      <div>
        <p class="profile-kicker">01 / SELECTED PROJECTS</p>
        <h2 id="projects-heading">代表项目</h2>
      </div>
      <a class="profile-secondary" href="{{ '/projects/' | relative_url }}">全部项目 <span aria-hidden="true">→</span></a>
    </div>
    {% include project-list.html heading="h3" %}
  </section>

  <section class="profile-section profile-focus" aria-labelledby="interests-heading">
    <div>
      <p class="profile-kicker">02 / INTERESTS</p>
      <h2 id="interests-heading">关注方向</h2>
    </div>
    <div>
      <p><strong>软件质量与性能</strong>　关注并发业务中的一致性、功能与安全测试，以及 SQL 和接口性能优化。</p>
      <p><strong>人工智能可信安全</strong>　希望在后续学习中探索如何评估 AI 系统的可靠性与安全性。</p>
    </div>
  </section>
</main>
