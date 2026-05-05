---
layout: page
permalink: /repositories/
title: repositories
description: GitHub 个人主页与开源项目仓库。
nav: true
nav_order: 3
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_users %}

## GitHub Contributions

{% for user in site.data.repositories.github_users %}
<div class="repositories">
  <a href="https://github.com/{{ user }}">
    <img class="only-light w-100" src="https://ghchart.rshah.org/YYYYXL1004" alt="GitHub Contributions" />
    <img class="only-dark w-100" src="https://ghchart.rshah.org/409ba5/YYYYXL1004" alt="GitHub Contributions" />
  </a>
</div>
{% endfor %}

---

{% endif %}

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
