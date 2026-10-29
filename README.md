# ProjectFlow — Basic Application Lifecycle Management System

A lightweight, responsive web prototype for tracking software projects across the application lifecycle. It was created as a basic academic project for Software Process Models and Application Lifecycle Management (ALM).

## Live deployment

Expected GitHub Pages URL: **https://praveenreddy-06.github.io/ase-alm2/**

The site is deployed through the GitHub Actions workflow in `.github/workflows/pages.yml`. The repository owner may need to select **Settings → Pages → Build and deployment → Source → GitHub Actions** once before the first successful deployment. Check the Actions tab for the deployment result.

## Features

- **Overview dashboard:** project counts, requirement totals, task completion, test summary, project progress, and recent activity.
- **Projects:** create and edit projects, choose a process model, set status and progress, and search/filter the list.
- **Requirements:** add requirement IDs, descriptions, priority, and status; cycle a requirement through planned, in-progress, and completed.
- **Task board:** organize tasks into To Do, In Progress, and Done columns; update or delete a task.
- **Test cases:** connect a test scenario to a requirement and record expected/actual results and Pass/Fail/Pending status.
- **Lifecycle tracker:** check off requirements, planning, design, development, testing, release, and maintenance; record a process model selection.
- **Browser persistence:** changes are saved to `localStorage` on the current browser and device.
- **Responsive layout:** navigation and tables adapt for smaller screens.

## Run locally

No package installation, build tool, database, or backend is required.

1. Download or clone this repository.
2. Open `index.html` directly in a modern browser, or use VS Code Live Server.
3. Add or edit projects and records in the interface.

## Technology stack

- HTML5 for page structure
- CSS3 for styling and responsive layout
- Vanilla JavaScript for interface behaviour and record management
- Browser `localStorage` for prototype persistence
- Git and GitHub for version control
- GitHub Pages and GitHub Actions for static hosting

## Software process model

The prototype uses an **Incremental** approach as the primary model: a small working dashboard is delivered first, then project tracking, requirements, tasks, testing, and lifecycle tracking are added as manageable increments. This is appropriate for a small, low-risk academic prototype whose interface can be improved from feedback.

## Scope and limitations

This is an educational, front-end-only prototype. Sample records are illustrative. It does not include user accounts, server-side storage, multi-user synchronization, access control, a real database, or a backend API. Browser data is local to the same browser profile and can be lost when its site data is cleared. Test results are user-entered demonstration records, not evidence of a production QA pipeline.

## Repository structure

```text
ase-alm2/
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── pages.yml
```

## Deployment workflow

When code is pushed to `main`, GitHub Actions uploads this repository as a static Pages artifact and deploys it. Manual runs are also available from **Actions → Deploy to GitHub Pages → Run workflow**.

## Academic report

The project report describes the problem, requirements, process-model comparison, ALM lifecycle, design, implementation, and test plan. Before submission, fill in the institution/course details and confirm any required team member names with the instructor.
