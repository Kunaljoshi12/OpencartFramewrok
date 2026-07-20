# OpenCart Playwright Automation Framework

[![Playwright](https://img.shields.io/badge/Playwright-1.40+-green.svg)](https://playwright.dev/)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-blue.svg)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Node.js-18+-brightgreen.svg)](https://nodejs.org/)
[![Allure Report](https://img.shields.io/badge/Report-Allure-ff69b4.svg)](https://allurereport.org/)
[![CI/CD](https://img.shields.io/badge/CI%2FCD-Jenkins-orange.svg)](https://www.jenkins.io/)

A scalable, robust End-to-End (E2E) Test Automation Framework for the **OpenCart** application built using **Playwright**, **TypeScript**, and the **Page Object Model (POM)** design pattern. It includes continuous integration setup via **Jenkins** and rich reporting with **Allure**.

---

## 📌 Features

- **Page Object Model (POM):** Clean separation of UI elements, actions, and test assertions.
- **Cross-Browser Testing:** Supports Chromium, Firefox, WebKit, and mobile viewports out of the box.
- **Parallel Test Execution:** High-speed execution with Playwright's built-in runner.
- **Data-Driven Automation:** Dynamic test data management using external JSON fixtures.
- **Rich Test Reporting:** Integrated with **Allure Reports** and standard Playwright HTML reports.
- **CI/CD Ready:** Configured for local and remote execution via **Jenkins**.

---

## 📂 Framework Directory Structure

```text
OpencartFramewrok/
├── pages/                   # Page Object Classes
│   ├── HomePage.ts          # Locators & actions for Home Page
│   ├── LoginPage.ts         # Locators & actions for Login Page
│   ├── AccountPage.ts       # Locators & actions for User Account Page
│   ├── RegistrationPage.ts  # Locators & actions for Registration Page
│   └── ProductPage.ts       # Locators & actions for Cart/Product pages
├── tests/                   # Test Suite Specs
│   ├── Login.spec.ts        # Login test scenarios
│   ├── Registration.spec.ts # User registration test scenarios
│   └── AddToCart.spec.ts    # E-commerce purchase flow tests
├── testData/                # Data-driven JSON files
│   └── loginData.json
├── utils/                   # Shared utility & helper classes
├── allure-results/          # Raw output data for Allure reporting
├── playwright.config.ts     # Core Playwright configuration settings
├── package.json             # NPM dependencies and scripts
├── tsconfig.json            # TypeScript compiler settings
└── README.md                # Project documentation
