---
layout: page
permalink: /repositories/
title: Repositories
description: 研究代码、竞赛方案与个人主页项目。
nav: true
nav_order: 3
---

<div class="repositories-intro">
  <div>
    <span class="repositories-kicker">Open Source & Research</span>
    <p>这里汇总了我的研究实现、竞赛代码与网站项目。每个仓库都可以直接前往 GitHub 查看源码和最新进展。</p>
  </div>
  <a class="github-profile-link" href="https://github.com/{{ site.data.repositories.github_username }}">
    <i class="fa-brands fa-github"></i>
    <span>@{{ site.data.repositories.github_username }}</span>
    <i class="fa-solid fa-arrow-up-right-from-square"></i>
  </a>
</div>

<div class="repository-grid">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
