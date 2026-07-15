---
order: 1
title: pytest-automation
summary: >-
  A single pytest repo covering API, browser UI, and mobile testing, built to show how pytest
  marks let CI target one module at a time instead of running the whole mono-repo on every change.
bullets:
  - Three test surfaces live in one repo — API (requests, against NASA's NEO API), browser UI (Playwright), and mobile (Appium, against a Sauce Labs demo app)
  - Custom pytest markers (mobile, android, ios, in_dev) select platform-specific subsets without touching test code
  - "Goal: a CI pipeline that runs only the module/platform touched by a given change, instead of the full suite every time — workflow wiring is in progress"
  - Allure reporting across all three surfaces, dependencies managed with uv
tags:
  - Python
  - pytest
  - Playwright
  - Appium
  - Allure
github: https://github.com/cloffwang/pytest-automation
---
