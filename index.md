---
layout: default
title: Home
---

<section class="hero">
  <div class="terminal-window">
    <div class="terminal-window-bar">
      <span class="terminal-dot red"></span>
      <span class="terminal-dot yellow"></span>
      <span class="terminal-dot green"></span>
    </div>
    <div class="terminal-window-body">
      <p class="prompt">whoami</p>
      <p>
        Senior SDET and former QA team lead with 10+ years across manual and automation
        testing. Recent focus is Python and Playwright test frameworks spanning UI, API, and
        MCP services, owning the whole framework end-to-end on scheduled Jenkins runs, plus
        building smoke-test dashboards for service health. Background also spans mobile test
        automation with Appium, ETL/data-pipeline validation, and web UI testing with Java,
        Selenium, and Cypress. Comfortable across AWS, GCP, and reporting tools like Allure
        Report.
      </p>
    </div>
  </div>
</section>

<section class="projects">
  <h2 class="prompt">ls ./projects</h2>

  <div class="project-grid">
    {% assign projects = site.projects | sort: 'order' %}
    {% for project in projects %}
    <article class="project-card" id="{{ project.title | slugify }}">
      <h3>{{ project.title }}</h3>
      <p>
        {{ project.summary }}
      </p>
      <ul>
        {% for bullet in project.bullets %}
        <li>{{ bullet }}</li>
        {% endfor %}
      </ul>
      <div class="tags">
        {% for tag in project.tags %}
        <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
      <div class="project-links">
        <a href="{{ project.github }}">GitHub &rarr;</a>
        {% if project.report %}
        <a href="{{ project.report }}">{{ project.report_label | default: "Report" }} &rarr;</a>
        {% endif %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>
