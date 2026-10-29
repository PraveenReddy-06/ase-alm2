# CivicFlow — Smart Drainage & Water Supply Reporting System

A responsive, front-end-only academic prototype where citizens can report drainage blockages, water shortages, water leakage, drain overflow, suspected contaminated water and other local civic issues. Reports can include a description, locality/address, optional browser geolocation, and optional photo evidence. A simulated authority view can prioritize reports and update status.

## Live demo

**https://praveenreddy-06.github.io/ase-alm2/**

The static site is deployed using the GitHub Actions workflow at [`.github/workflows/pages.yml`](.github/workflows/pages.yml). Check the [Actions tab](https://github.com/PraveenReddy-06/ase-alm2/actions) for the latest deployment status.

## Features

- **Community dashboard:** total reports, reports awaiting action, in-progress issues, resolved issues and a type breakdown.
- **Issue submission:** type, impact level, address/locality, detailed description and optional reporter name.
- **Optional location:** asks browser permission to add coordinates; users can instead enter a location manually.
- **Optional photo evidence:** preview and resize an image locally before saving it with the report.
- **Issue tracker:** search by ID, issue type, location or description; filter by type/status.
- **Authority demo mode:** prioritize urgent/high-severity reports and change issue status or priority.
- **Status workflow:** Submitted → Acknowledged → In Progress → Resolved.
- **Issue details:** show report ID, location, timestamps, status, priority, optional coordinates/map link and attached image.
- **Browser persistence:** records are saved in the current browser profile using `localStorage`.
- **Responsive interface:** adapts to laptop and mobile widths.

## Run locally

No build step, framework, database, or package installation is required.

1. Clone or download the repository.
2. Open `index.html` in a modern browser, or use VS Code Live Server.
3. Create a report and test status changes. The records remain local to that browser profile.

## Technology stack

- HTML5
- CSS3 with responsive layout
- Vanilla JavaScript
- Browser `localStorage`
- Browser Geolocation API (permission required)
- FileReader and Canvas APIs for local image preview/compression
- Git/GitHub and GitHub Actions
- GitHub Pages for static hosting

## Proposed software process model

The report selects the **Incremental Model**. The prototype can be delivered through small increments: (1) page shell and sample issue dashboard, (2) report form, validation, optional photo/location and persistence, and (3) search, filters, authority demo controls, testing and deployment. Each increment can be reviewed and refined without requiring a complete rewrite.

## Data and privacy limitations

This is a classroom prototype, not an official government service. It does **not** send complaints to a municipality, dispatch field staff, verify identity, or provide emergency response. It has no server, database, authentication, authorization, cross-device synchronization, or trusted audit trail. The authority mode is a demonstration switch, not secure role-based access. All records and photos remain in the current browser profile; clearing site data can delete them. Do not submit sensitive personal information or use this demo for urgent public-safety reports.

A production version would need a secure backend and database, authenticated citizen/staff roles, data retention and privacy controls, a protected evidence store, server-side validation, audit logs, abuse prevention, and integration with the responsible local authority.

## Repository structure

```text
ase-alm2/
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── pages.yml
```

## Report

The DOCX project report follows the course's supplied Project Report Format for CO2, covering introduction, requirement analysis, process-model selection, ALM, design, implementation, testing and project progress evidence. Update course section, instructor and team-member details as needed. Capture real site screenshots and record manual test outcomes before submission.
