# Accessibility Baseline & Repository Architecture Audit

## Purpose
Accessibility audit of the IRCTC train search page (irctc.co.in/nget/train-search) using Lighthouse and keyboard navigation, plus a monorepo-style starter skeleton for a full stack project.

## Repository Structure
- client/ - frontend (UI code)
- server/ - backend (APIs and business logic)
- docs/ - audit worksheet and screenshots
- test/ - automated tests

## Audit Summary
5 issues found (3 High, 2 Medium): missing image alt text, form inputs without labels, buttons and links without accessible names, invalid ARIA attributes, and low colour contrast.
Details: docs/accessibility-audit-worksheet.csv
Evidence: screenshots in docs/

## Local Setup
1. Clone: git clone https://github.com/kumarilucky816-eng/accessibility-baseline-architecture-audit.git
2. Client: cd client && npm install && npm start
3. Server: cd server && npm install && npm start

## First Vertical Feature
Train search: search form in client -> API endpoint in server -> results shown in UI. All form fields will have proper labels and sufficient colour contrast.
