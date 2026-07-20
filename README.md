# Odoo Reverse-Engineering Documentation

Full reverse-engineered functional + data-structure documentation of the user's Odoo instance (https://www.odoo.com/web/login), built page-by-page and function-by-function from the live front end (no source code access).

## Scale reality

Odoo is a 40+ app ERP suite (Sales, CRM, Inventory, Manufacturing, Accounting, Invoicing, Purchase, Point of Sale, Project, Timesheets, Employees, Recruitment, Expenses, Field Service, Helpdesk, Website, eCommerce, Marketing, Events, Livechat, Surveys, Documents, Sign, Approvals, Knowledge, Subscriptions, Fleet, Maintenance, Quality, Repair, Rental, and more). 'Complete, every module, every function' documentation is a genuinely large effort. It is broken into:

1. A scoping/mapping task: log in, enumerate every app actually installed/visible on this account (a trial account may not have every app enabled), and record it in `docs/00-installed-apps-map.md`. This becomes the checklist for everything after.
2. One dedicated task per app/module, each following the same deep-documentation methodology as the infisuite CRM work (purpose, data fields, inferred data model, logic/conditions, inputs/outputs) PLUS, per the Owner's explicit ask for this project: reports/analysis views within the app, and both success AND error/failure paths for key workflows (not just the happy path).

## Structure

`docs/<app-slug>/` and `screenshots/<app-slug>/` per app, e.g. `docs/sales/`, `docs/accounting/`, `docs/inventory/`.

Login credentials are NOT stored in this repo. They live in the AI-OS task prompt.txt on the dispatching server only.
