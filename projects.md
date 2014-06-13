---
layout: page
title: Projects
---


<div class="project">
  {% for project in paginator.projects %}
  <div class="project">
    <h1 class="project-title">
      <a href="{{ project.url }}">
        {{ project.title }}
      </a>
    </h1>

    <span class="project-date">{{ project.date | date_to_string }}</span>

    {{ project.content }}
  </div>
  {% endfor %}
</div>

<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-item older" href="/page{{paginator.next_page}}">Older</a>
  {% else %}
    <span class="pagination-item older">Older</span>
  {% endif %}
  {% if paginator.previous_page %}
    {% if paginator.page == 2 %}
      <a class="pagination-item newer" href="/">Newer</a>
    {% else %}
      <a class="pagination-item newer" href="/page{{paginator.previous_page}}">Newer</a>
    {% endif %}
  {% else %}
    <span class="pagination-item newer">Newer</span>
  {% endif %}
</div>