---
order: 2
title: quality-dashboard
summary: >-
  A Playwright test suite for a mock "Quality &amp; Uptime Control Center" dashboard, built to
  show how much richer an Allure report can be when tests are instrumented deliberately.
bullets:
  - Per-step screenshots on UI specs and native HTTP-exchange attachments (request/response logs) on API specs, all surfaced in the Allure report
  - Every test carries an explicit description and suite label, enforced by a lint check so reports stay self-documenting
  - GitHub Actions runs the UI/API suites on a schedule and publishes the generated Allure reports (with history) to GitHub Pages
  - The dashboard itself (Next.js, fully mocked data) exists only to give the suite something realistic to test against
tags:
  - Playwright
  - Allure
  - TypeScript
  - CI/CD
  - Next.js
github: https://github.com/cloffwang/quality-dashboard
report: https://cloffwang.github.io/quality-dashboard/
report_label: Allure report
---
