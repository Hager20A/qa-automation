# QA Automation Framework - Design Demo

## Overview
This repository demonstrates my **automation design approach** for dynamic web applications.

## Challenge Solved
- Dynamic elements with unstable `slot="field-XXX"` attributes  
- DOM changes on scroll causing stale element references  

## Locator Strategy
Locate stable parent using visible text, then traverse to child input.  

## Project Structure
pages/
├── BasePage.js
├── AdminTabsPage.js
└── components/
└── DynamicField.js
tests/
data/
└── test-data.json
docs/
└── locator-strategy.md
utils/

text

## Tech Stack (Proposed)
- Playwright with JavaScript/TypeScript
- Page Object Model
- Data-driven testing with JSON

## Author
Hager - Senior QA Automation Engineer
