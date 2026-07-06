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
    <article class="project-card">
      <h3>quality-dashboard</h3>
      <p>
        A Playwright test suite for a mock "Quality &amp; Uptime Control Center" dashboard, built to
        show how much richer an Allure report can be when tests are instrumented deliberately.
      </p>
      <ul>
        <li>Per-step screenshots on UI specs and native HTTP-exchange attachments (request/response logs) on API specs, all surfaced in the Allure report</li>
        <li>Every test carries an explicit description and suite label, enforced by a lint check so reports stay self-documenting</li>
        <li>GitHub Actions runs the UI/API suites on a schedule and publishes the generated Allure reports (with history) to GitHub Pages</li>
        <li>The dashboard itself (Next.js, fully mocked data) exists only to give the suite something realistic to test against</li>
      </ul>
      <div class="tags">
        <span class="tag">Playwright</span>
        <span class="tag">Allure</span>
        <span class="tag">TypeScript</span>
        <span class="tag">CI/CD</span>
        <span class="tag">Next.js</span>
      </div>
      <div class="project-links">
        <a href="https://github.com/cloffwang/quality-dashboard">GitHub &rarr;</a>
        <a href="https://cloffwang.github.io/quality-dashboard/">Allure report &rarr;</a>
      </div>
    </article>
    <article class="project-card">
      <h3>selenium-demo</h3>
      <p>
        A Web UI testing framework using Java, Selenium, and Cucumber with a BDD approach.
      </p>
      <ul>
        <li>Flexible execution on local, CI, Selenium Grid, and BrowserStack via YAML configuration</li>
        <li>Parallel execution with thread-safe browser driver management using TestNG data providers</li>
        <li>Integrated with GitHub Actions for CI, with reporting via Allure</li>
      </ul>
      <div class="tags">
        <span class="tag">Java</span>
        <span class="tag">Selenium</span>
        <span class="tag">Cucumber</span>
        <span class="tag">TestNG</span>
        <span class="tag">CI/CD</span>
      </div>
      <div class="project-links">
        <a href="https://github.com/cloffwang/selenium-demo">GitHub &rarr;</a>
        <a href="https://cloffwang.github.io/selenium-demo/">Allure report &rarr;</a>
      </div>
    </article>
  </div>
</section>
