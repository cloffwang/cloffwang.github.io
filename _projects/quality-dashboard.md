---
order: 2
title: quality-dashboard
summary: >-
  A mock "Quality &amp; Uptime Control Center" dashboard paired with a Playwright suite, built
  to demonstrate three SDET framework practices at once: bird's-eye test-health reporting,
  modular per-feature test organization, and environment-agnostic test logic.
bullets:
  - A weekly calendar view (the live Allure report's landing page) surfaces every UI/API run by day — an at-a-glance status view instead of digging through individual CI logs
  - Tests are organized into independent modules per feature area (ui/ and api/, each split into frontend smoke, backend API, ETL, MCP) — a pattern that scales to more services without restructuring the suite
  - The same spec files run unmodified against prod and stage environments; environment differences are injected through one shared fixture rather than forked test files
  - GitHub Actions runs the suite on every PR and on a 4-hour schedule, publishing live Allure reports to GitHub Pages
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
