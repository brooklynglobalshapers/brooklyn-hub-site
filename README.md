# Global Shapers Brooklyn Hub — Website

A free, static website for the Global Shapers Community NYC – Brooklyn Hub, built to be handed off cleanly to each new curatorship.

**Live once deployed at:** `[https://brooklynglobalshapers.github.io/brooklyn-hub-site/]`

## What's in here

```
index.html                    Home — must stay at the root (GitHub Pages looks for
                               this file to serve your site's base URL)
main-pages/
  about.html                   Team, values, community photos
  projects.html                 Active / on-hold / proposed projects — links into projects/
  events.html                   Upcoming events, Hub Meetings, past event history
  apply.html                    Join/application form
projects/
  so-fresh-so-clean.html
  sow-rhythm-seed.html
  link-the-lunch.html          individual project pages
  climate-connect.html
  myco.html
  equal-air-collaborative.html
css/style.css                 All styling (one file)
js/main.js                    Mobile nav toggle
assets/                       Logo, team photos, project images
HANDOVER.md                   Read this before your curatorship ends
```

**A structural note:** `index.html` is the one file that can't be moved into a folder —
static hosts (GitHub Pages included) look for it at the root to know what to show when
someone visits your bare domain. Every other page lives one folder deep (`main-pages/`
or `projects/`), so their internal links all start with `../` to reach `index.html`,
`assets/`, `css/`, and `js/` back at the root.

## Adding Collaborators

   In **Settings → Collaborators and teams**, add your Curator, Communications Officer,
   and whoever else should be able to edit the site, as **Owners** of the organization
   (not just the repo) — that's what makes next year's handover a 2-minute settings
   change instead of a migration.

## Editing day-to-day

- **New project:** copy one of the existing files in `projects/` as a starting template,
  update the content, and add a linked entry (with a thumbnail image) to
  `main-pages/projects.html`. Since it lives in `projects/`, its internal links to
  CSS/JS/images/other pages all start with `../` — copying an existing file gets this
  right automatically.
- **New event / past-event entry:** edit the plain bullet lists in `main-pages/events.html`
  directly.
- **New team member or copy change:** edit the relevant `.html` file directly —
  everything is plain HTML with clearly named sections.
- **New images:** drop them in `assets/` and reference `assets/your-file.jpg` from
  `index.html`, or `../assets/your-file.jpg` from anything inside `main-pages/` or
  `projects/`.
- **Signup form:** replace the `iframe src` in `main-pages/apply.html` with a new Google
  Form - embed link whenever a new form goes out.

## Handing this off next term

See `HANDOVER.md`.
