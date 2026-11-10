# Awesome-Browser-Extension-Testing-Plugins

## Top Browser Extension Testing & Plugins Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cross-Browser Extension Testing, Developer Tooling & Automated Validation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Browser Extension Testing & Plugins**. These tools help developers build, test, and validate browser extensions across Chrome, Firefox, Edge, and Safari—covering automated end-to-end testing, static analysis, developer dashboards, and cross-browser build pipelines.

**Examples** include BrowserStack Extension Tools, Chrome Web Store Developer Dashboard, Firefox Add-on Developer Hub, Edge Add-ons Hub, Opera Addons Hub, CRXJS, Web-Ext CLI, ExtensionCLI, Plasmo Framework, and Safari Web Extension Converter (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted extension testing frameworks, cross-browser build tooling, and static validation—ideal for extension developers, QA engineers, and platform teams building transparent, vendor-neutral extension quality pipelines.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS Products

| Platform | Description | Pricing / Limits |
| --- | --- | --- |
| **[BrowserStack Extension Tools](https://www.browserstack.com/)** | Cloud testing platform supporting pre-loaded Chrome/Edge extensions from the Web Store or local `.zip`/`.crx` builds (up to 100 MB) on Windows and macOS; enables testing in-development extensions across browser/OS combinations before publishing, with Playwright automation support via `chromefortesting` for Chrome 137+ extension loading restrictions. | Commercial (Free trial available with limited test minutes) |
| **[Chrome Web Store Developer Dashboard](https://chrome.google.com/webstore/devconsole)** | Google's official publishing console with verified uploads (RSA key signing to restrict releases), staged rollouts for 10k+ user extensions, trusted tester distribution, and beta labeling requirements. | $5 one-time registration fee; no recurring charge |
| **[Firefox Add-on Developer Hub](https://addons.mozilla.org/developers/)** | Mozilla's AMO developer console for submitting, managing, and signing Firefox extensions; pairs with `web-ext` CLI for local build, run, and lint workflows. | Free (Open submission and automated validation) |
| **[Edge Add-ons Hub](https://partner.microsoft.com/dashboard/microsoftedge/)** | Microsoft's partner center for publishing and managing Edge extensions, with certification workflows and store listing management. | Free developer account for extension submissions |
| **[Opera Addons Hub](https://addons.opera.com/developer/)** | Opera's developer portal for submitting and managing Opera browser extensions and review cycles. | Free submission and review process |
| **[Plasmo Cloud](https://www.plasmo.com/)** | Cloud extension workflows offering automated cross-browser packaging, team deployments, and submission pipelines. | Free tier available; paid team tiers for scale |

## Open-Source GitHub Projects

*Sorted descending by GitHub stars count.*

- **[Playwright](https://github.com/microsoft/playwright)** [![GitHub stars](https://img.shields.io/github/stars/microsoft/playwright?style=social&color=white)](https://github.com/microsoft/playwright/stargazers)  
  High-performance browser automation library supporting Chromium, Firefox, and WebKit; supports custom extension testing harnesses via `--disable-extensions-except` and `--load-extension` flags, service worker inspection, and background context fixtures.

- **[Puppeteer](https://github.com/puppeteer/puppeteer)** [![GitHub stars](https://img.shields.io/github/stars/puppeteer/puppeteer?style=social&color=white)](https://github.com/puppeteer/puppeteer/stargazers)  
  Node.js library providing a high-level API over the Chrome DevTools Protocol (CDP); frequently used for headless/headful extension automation, background worker debugging, and popup interaction.

- **[Cypress](https://github.com/cypress-io/cypress)** [![GitHub stars](https://img.shields.io/github/stars/cypress-io/cypress?style=social&color=white)](https://github.com/cypress-io/cypress/stargazers)  
  Next-generation front-end testing tool capable of loading unpacked Chrome extensions via browser launch arguments and validating page-injection behaviors.

- **[Selenium WebDriver](https://github.com/SeleniumHQ/selenium)** [![GitHub stars](https://img.shields.io/github/stars/SeleniumHQ/selenium?style=social&color=white)](https://github.com/SeleniumHQ/selenium/stargazers)  
  Standard browser automation ecosystem supporting cross-browser extension pre-loading via `ChromeOptions.addExtensions` / `FirefoxProfile.addExtension` and WebDriver BiDi extension management.

- **[Plasmo](https://github.com/PlasmoHQ/plasmo)** [![GitHub stars](https://img.shields.io/github/stars/PlasmoHQ/plasmo?style=social&color=white)](https://github.com/PlasmoHQ/plasmo/stargazers)  
  Modular framework for browser extensions with Parcel bundler, declarative `package.json` manifests, hot-reloading CSUI (Content Scripts UI), and cross-browser target building.

- **[WXT](https://github.com/wxt-dev/wxt)** [![GitHub stars](https://img.shields.io/github/stars/wxt-dev/wxt?style=social&color=white)](https://github.com/wxt-dev/wxt/stargazers)  
  Next-generation Vite-powered extension framework featuring file-convention manifest generation, unified cross-browser APIs (Chrome, Edge, Firefox, Safari), TypeScript support, and blazing fast HMR.

- **[WebdriverIO](https://github.com/webdriverio/webdriverio)** [![GitHub stars](https://img.shields.io/github/stars/webdriverio/webdriverio?style=social&color=white)](https://github.com/webdriverio/webdriverio/stargazers)  
  Next-gen browser automation framework for Node.js with native support for Chrome extensions (`--load-extension`), Firefox `.xpi` add-on installation, and WebDriver BiDi `installExtension()` / `uninstallExtension()` APIs.

- **[Extension.js](https://github.com/extension-js/extension.js)** [![GitHub stars](https://img.shields.io/github/stars/extension-js/extension.js?style=social&color=white)](https://github.com/extension-js/extension.js/stargazers)  
  Zero-config cross-browser framework using `manifest.json` as the single source of truth; includes an internal Rspack bundler, targeted live-reload for popups/content scripts, and automated Safari conversion and build pipelines.

- **[CRXJS Vite Plugin](https://github.com/crxjs/chrome-extension-tools)** [![GitHub stars](https://img.shields.io/github/stars/crxjs/chrome-extension-tools?style=social&color=white)](https://github.com/crxjs/chrome-extension-tools/stargazers)  
  Vite plugin for modern Chrome Extension development; parses `manifest.json` directly into the Vite build pipeline with full HMR for content scripts, popups, options pages, and background service workers.

- **[web-ext](https://github.com/mozilla/web-ext)** [![GitHub stars](https://img.shields.io/github/stars/mozilla/web-ext?style=social&color=white)](https://github.com/mozilla/web-ext/stargazers)  
  Mozilla's official CLI to build, run, package, and lint WebExtensions; integrates directly into CI/CD workflows for AMO automated linting and Firefox testing.

- **[vite-plugin-web-extension (aklinker1)](https://github.com/aklinker1/vite-plugin-web-extension)** [![GitHub stars](https://img.shields.io/github/stars/aklinker1/vite-plugin-web-extension?style=social&color=white)](https://github.com/aklinker1/vite-plugin-web-extension/stargazers)  
  Vite plugin that facilitates building cross-browser extensions (Manifest V2 and V3) with automatic multi-page setup, asset bundling, and browser launch commands.

- **[playwright-crx](https://github.com/ruifigueira/playwright-crx)** [![GitHub stars](https://img.shields.io/github/stars/ruifigueira/playwright-crx?style=social&color=white)](https://github.com/ruifigueira/playwright-crx/stargazers)  
  Playwright port customized to execute and automate testing directly inside Chrome extensions and web extension contexts.

- **[DeploySentinel Recorder](https://github.com/DeploySentinel/Recorder)** [![GitHub stars](https://img.shields.io/github/stars/DeploySentinel/Recorder?style=social&color=white)](https://github.com/DeploySentinel/Recorder/stargazers)  
  Browser extension that captures real user browser interactions and automatically generates Cypress, Playwright, and Puppeteer test scripts.

- **[addons-linter](https://github.com/mozilla/addons-linter)** [![GitHub stars](https://img.shields.io/github/stars/mozilla/addons-linter?style=social&color=white)](https://github.com/mozilla/addons-linter/stargazers)  
  Mozilla's open-source suite for validating and linting add-ons against security, compatibility, and manifest structure rules before release.

- **[vite-plugin-web-extension (samrum)](https://github.com/samrum/vite-plugin-web-extension)** [![GitHub stars](https://img.shields.io/github/stars/samrum/vite-plugin-web-extension?style=social&color=white)](https://github.com/samrum/vite-plugin-web-extension/stargazers)  
  A Vite plugin enabling streamlined bundling and live reloading for WebExtension manifest configurations across browsers.

- **[jest-webextension-mock](https://github.com/clarkbw/jest-webextension-mock)** [![GitHub stars](https://img.shields.io/github/stars/clarkbw/jest-webextension-mock?style=social&color=white)](https://github.com/clarkbw/jest-webextension-mock/stargazers)  
  A Jest helper module providing complete mocks for the `browser` and `chrome` extension APIs for isolated unit testing.

- **[cypress-browser-extension-plugin](https://github.com/ejoubaud/cypress-browser-extension-plugin)** [![GitHub stars](https://img.shields.io/github/stars/ejoubaud/cypress-browser-extension-plugin?style=social&color=white)](https://github.com/ejoubaud/cypress-browser-extension-plugin/stargazers)  
  Cypress plugin allowing end-to-end testing of browser extensions by streamlining extension bundle loading into Cypress browser instances.

- **[mockzilla-webextension](https://github.com/Lusito/mockzilla-webextension)** [![GitHub stars](https://img.shields.io/github/stars/Lusito/mockzilla-webextension?style=social&color=white)](https://github.com/Lusito/mockzilla-webextension/stargazers)  
  TypeScript-first mocking toolkit for WebExtension APIs designed for Jest and Vitest unit test suites.

- **[chrome-extension-testing-mcp](https://github.com/BHUVAN-RJ/chrome-extension-testing-mcp)** [![GitHub stars](https://img.shields.io/github/stars/BHUVAN-RJ/chrome-extension-testing-mcp?style=social&color=white)](https://github.com/BHUVAN-RJ/chrome-extension-testing-mcp/stargazers)  
  Model Context Protocol (MCP) server enabling AI coding agents to test unpacked Chrome extensions interactively via Playwright (service worker logs, popups, storage, badges).

- **[chrome-extension-test-framework](https://github.com/ibushimaru/chrome-extension-test-framework)** [![GitHub stars](https://img.shields.io/github/stars/ibushimaru/chrome-extension-test-framework?style=social&color=white)](https://github.com/ibushimaru/chrome-extension-test-framework/stargazers)  
  Fast static analysis and verification framework (no browser needed) for validating Manifest V3 compliance, security, CSP restrictions, and file structure in CI.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Extension testing must account for browser-specific API differences (e.g., `chrome.sidePanel` not available in Safari), manifest version fragmentation (MV2/MV3), and store review policies.
- Self-hosted open-source testing frameworks require maintenance as browser APIs and store requirements evolve; always validate against target browser versions.

---

**Made for extension developers, QA engineers, platform teams, and developer tooling builders.**  
Let's make browser extension testing more open, automated, and cross-browser reliable.
