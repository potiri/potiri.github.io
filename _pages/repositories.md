---
layout: page
permalink: /repositories/
title: repositories
description: Some selected GitHub repos, both from research and private projects.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %} <!-- Close github_repos if statement -->
