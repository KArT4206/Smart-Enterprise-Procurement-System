# Changelog

## 2026-11-06: UI rework

- New design system: tokens for colour, spacing, radii, shadows and motion; light and dark themes with a toggle and no flash on load.
- New app shell: light collapsible sidebar, mobile drawer, sticky blurred top bar with breadcrumbs, ⌘K search, notifications and account menu.
- Redesigned sign-in and sign-up as a split layout, with links between them.
- Role dashboards rebuilt around KPI cards and one action-queue renderer, with skeleton loading and empty states.
- Shared table: cleaner toolbar, sort indicators, column menu, compact pagination; fixed row hover that broke dark mode.
- Restyled workflow stepper, timeline and status badges.
- About 640 hardcoded colours across all pages replaced with theme tokens; error messages are now styled alerts; layouts wrap at phone width.

## Initial release

- Source-to-Pay workflow across nine roles: requisitions, rule-based approvals, RFQs, POs, receipts, invoices, payments.
- Spring Boot API with JWT auth and RBAC; PostgreSQL schema and seed data.
