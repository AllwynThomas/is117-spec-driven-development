Sprint 1 – Project Scaffolding (1–2 hrs)
Goal

Initialize a minimal static site with working local dev and deploy pipeline.

Tasks

Initialize Git repository

Create folder structure:

/ (root)
├── index.html
├── projects/
├── assets/
│   ├── css/
│   └── img/
├── data/
└── README.md

Add base index.html

Add empty styles.css

Configure GitHub Pages (deploy from /root branch)

Files

index.html

assets/css/styles.css

README.md

Acceptance Criteria

Visiting root loads a valid HTML page

CSS file is linked and applied

Repo deploys successfully via GitHub Pages

No console errors in browser

Verification Steps

Run locally with Live Server (or open in browser)

Push to GitHub

Confirm GitHub Pages URL renders correctly

What NOT to Do

Do not add JS frameworks

Do not add animations

Do not add external UI libraries

Sprint 2 – Global Design System (1–3 hrs)
Goal

Implement strict Swiss/International Typographic Style foundation.

Tasks

Implement 12-column CSS grid

Define typography scale

Set color tokens:

Black #000

White #FFF

Neutral gray

One accent color

Define spacing system (8px base unit)

Files

assets/css/styles.css

Acceptance Criteria

Layout uses consistent grid columns

All content left-aligned

Only 1–2 typefaces used

No decorative shadows, gradients, or rounded UI

Accent color used consistently

Verification Steps

Overlay grid in dev tools → elements align

Inspect computed styles → typography matches scale

Search CSS → only defined color tokens used

What NOT to Do

No centered hero sections

No decorative dividers

No animations

Sprint 3 – Homepage Layout (1–2 hrs)
Goal

Build trust-first homepage.

Sections

Name + role

One-sentence positioning statement

Selected projects (3 max)

Contact link

Tasks

Structure content within grid

Add project preview components

Link to project detail pages

Files

index.html

projects/project-1.html (placeholder)

Acceptance Criteria

Page loads under 1 second

Maximum 1 screen scroll before projects visible

No lorem ipsum

All project links functional

Verification Steps

Lighthouse performance score > 90

Click all links → no 404 errors

What NOT to Do

No testimonials yet

No blog

No skill bars

Sprint 4 – Project Content Model (1–2 hrs)
Goal

Define structured case study template.

Content Fields (Required per Project)
title:
role:
timeline:
tools:
problem:
constraints:
hypothesis:
process:
solution:
metrics:
evidence_links:
lessons:
Tasks

Create reusable HTML structure for case study

Enforce section order

Add placeholder content

Files

projects/template.html

Acceptance Criteria

All required fields present

Every claim paired with metric or artifact

No empty sections allowed

Verification Steps

Manually check each section exists

Confirm at least 1 “receipt” per major claim

What NOT to Do

No storytelling fluff

No vague claims (“improved UX”) without metric

Sprint 5 – Navigation & Footer (1 hr)
Goal

Add minimal global navigation.

Tasks

Add persistent top nav:

Home

Projects

Contact

Add footer with GitHub + LinkedIn links

Files

index.html

projects/*.html

Acceptance Criteria

Nav consistent across pages

Links functional

No dropdowns

Verification Steps

Test navigation between all pages

Confirm mobile layout does not break

What NOT to Do

No hamburger animation

No sticky scroll effects

Sprint 6 – Performance & Polish (1–2 hrs)
Goal

Ensure credibility through speed and clarity.

Tasks

Compress images

Remove unused CSS

Validate HTML

Check accessibility contrast

Files

All

Acceptance Criteria

Lighthouse Performance ≥ 90

Accessibility ≥ 90

No console warnings

Total page size < 1MB

Verification Steps

Run Lighthouse

Validate with W3C HTML validator

Inspect network tab

What NOT to Do

Do not add tracking scripts

Do not add analytics yet

Sprint 7 – Deployment Hardening (1 hr)
Goal

Reliable GitHub Pages deployment.

Tasks

Confirm build-free static deploy

Add .nojekyll file

Add 404 page

Files

.nojekyll

404.html

Acceptance Criteria

GitHub Pages builds without error

404 page renders for invalid route

HTTPS enforced

Verification Steps

Test invalid URL path

Confirm SSL lock in browser

What NOT to Do

No CI/CD pipelines yet

No domain configuration

Non-Goals (Prevent Scope Creep)

No CMS integration

No animations

No blog system

No dark mode

No React/Vue/Svelte

No backend

No form handling (use mailto)

Definition of Done (Final System)

Static site only

Strict Swiss typographic system

Every project includes measurable outcomes

GitHub Pages deploy stable

Lighthouse ≥ 90 across major categories

Total build complexity minimal