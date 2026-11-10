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

## SaaS/Hosted Platforms

- **[BrowserStack Extension Tools](https://www.browserstack.com/)**  
  Cloud testing platform supporting pre-loaded Chrome/Edge extensions from the Web Store or local `.zip`/`.crx` builds (up to 100 MB) on Windows and macOS; enables testing in-development extensions across browser/OS combinations before publishing, with Playwright automation support via `chromefortesting` for Chrome 137+ extension loading restrictions [citation:11].

- **[Chrome Web Store Developer Dashboard](https://chrome.google.com/webstore/devconsole)**  
  Google's official publishing console with verified uploads (RSA key signing to restrict releases), staged rollouts for 10k+ user extensions, trusted tester distribution, and beta labeling requirements to avoid repetitive content rejection [citation:6][citation:12].

- **[Firefox Add-on Developer Hub](https://addons.mozilla.org/developers/)**  
  Mozilla's AMO developer console for submitting, managing, and updating Firefox extensions; pairs with `web-ext` CLI for local build, run, and lint workflows [citation:8].

- **[Edge Add-ons Hub](https://partner.microsoft.com/dashboard/microsoftedge/)**  
  Microsoft's partner center for publishing and managing Edge extensions, with certification workflows and store listing management.

- **[Opera Addons Hub](https://addons.opera.com/developer/)**  
  Opera's developer portal for submitting and managing Opera browser extensions.

- **[CRXJS (Hosted CI)](https://crxjs.dev/)**  
  Vite plugin for Chrome extension development with HMR and manifest-based bundling; commonly run in hosted CI pipelines for cross-browser build validation .

- **[Web-Ext CLI (Hosted CI)](https://github.com/mozilla/web-ext)**  
  Mozilla's CLI for building, running, and testing web extensions; typically executed in GitHub Actions or GitLab CI for automated linting and Firefox testing [citation:8].

- **[ExtensionCLI / Extension.js](https://extension.js.org/)**  
  Zero-config cross-browser framework (Chrome, Edge, Firefox, Safari) with HMR, manifest V3 default, and `--zip` production builds; hosted CI workflows can leverage its one-command `dev` and `build` commands [citation:15].

- **[Plasmo Framework](https://www.plasmo.com/)**  
  React-focused extension framework with Parcel bundler, live-reload, and declarative manifest generation; cloud builds available for team workflows .

- **[Safari Web Extension Converter](https://developer.apple.com/documentation/safariservices/safari_web_extensions/converting_a_web_extension_for_safari)**  
  Apple's command-line tool (`safari-web-extension-converter`) for converting existing web extensions into Safari App Extensions; integrated into Extension.js for automated Xcode project generation and `xcodebuild` orchestration [citation:4][citation:10].

## Open-Source GitHub Projects

- **[pikabo](https://github.com/pikabo/pikabo)**  
  Playwright-based extension testing framework with fixtures for popup, options, side panel, and service worker; provides fresh-profile test isolation, permission auditing (declared vs. used `chrome.*` namespaces), console error capture from MV3 service workers, and self-contained HTML/JSON reports with screenshots and traces [citation:7].

- **[chrome-extension-tester-mcp](https://github.com/BHUVAN-RJ/chrome-extension-testing-mcp)**  
  MCP server enabling Claude to interactively test unpacked Chrome extensions via Playwright: load/reload extensions, interact with popup/options pages, inspect `chrome.storage`, read service worker logs, monitor network requests, check badges, send background messages, and run PASS/FAIL assertions—all through natural language [citation:1].

- **[WebdriverIO Extension Testing](https://webdriver.io/docs/platforms/apps-and-extensions)**  
  Native WebDriver-based testing for Chrome (`--load-extension`), Firefox (`browser.installAddOn` with `.xpi`), and VS Code extensions; supports BiDi `installExtension()`/`uninstallExtension()` for mid-session management; Safari requires separate handling due to no BiDi support [citation:13].

- **[Extension.js](https://github.com/extension-js/extension.js)**  
  Zero-config cross-browser framework with manifest.json as source of truth, Rspack bundler (internal), hot reload for popup/options/devtools, targeted content-script reloads, and Safari build pipeline (converter → Xcode → `xcodebuild`) with bundle ID enforcement and registration polling [citation:4][citation:10].

- **[WXT](https://github.com/wxt-dev/wxt)**  
  Vite-powered extension framework with file-convention manifest generation, cross-browser builds (Chrome, Edge, Firefox, Safari build-only), and HMR; actively tracks Vite major versions .

- **[CRXJS](https://github.com/crxjs/chrome-extension-tools)**  
  Vite plugin for Chrome extension development (Firefox via `browser` option); reads `manifest.json` through Vite's plugin API, requires compatibility work per Vite major (supports Vite 3–8) .

- **[Plasmo](https://github.com/PlasmoHQ/plasmo)**  
  React-focused framework with Parcel bundler, declarative manifest in `package.json`, CSUI (Custom UI) support, and cross-browser targets (Chrome MV3, Firefox MV2/MV3 experimental) .

- **[web-ext](https://github.com/mozilla/web-ext)**  
  Mozilla's CLI for building, running, and linting web extensions; essential for Firefox AMO submission workflows and local development [citation:8].

- **[chrome-extension-test-framework](https://github.com/ibushimaru/chrome-extension-test-framework)**  
  Fast static analysis framework (no browser required) for Chrome extensions: validates Manifest V3 compliance, security (CSP, external scripts, `eval()` usage), performance (file sizes, optimization), structure, and localization; supports console/JSON/HTML/Markdown output and CI exit codes [citation:14].

### Additional Strong Open-Source Options

- **[Playwright](https://github.com/microsoft/playwright)** with `--disable-extensions-except` and `--load-extension` flags for custom extension test harnesses.
- **[Puppeteer](https://github.com/puppeteer/puppeteer)** for headless Chrome extension automation with CDP-based service worker inspection.
- **[Selenium WebDriver](https://github.com/SeleniumHQ/selenium)** with ChromeOptions/`addExtension` for cross-browser extension loading.
- **Community `web-ext` wrappers** and **ESLint plugins** for extension-specific linting rules.
- Many **manifest validation scripts** and **permission audit tools** for pre-submission store checks.

**Frameworks for building custom systems**: Combine **pikabo** for Playwright-native extension testing, **chrome-extension-tester-mcp** for AI-assisted interactive validation, **Extension.js** for cross-browser build pipelines, and **web-ext** for Firefox-specific linting—orchestrated via **GitHub Actions** with store submission gates.

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
