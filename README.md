# michael-claude-design-files

Design work built with Claude, organized as a browsable static site.

```
/
  index.html                                   landing → categories
  prototypes/
    index.html                                 → product modules
    applications/
      index.html                               → Applications prototypes
      availability-nav/
        index.html                             Application Settings & Availability
```

## Structure

1. **Type** — `prototypes/` (add siblings like `mockups/` later).
2. **Module** — `prototypes/applications/` (add `prototypes/communications/`, etc.).
3. **Prototype** — each in its own folder with a self-contained `index.html`.

Each level has a landing page that links down; breadcrumbs link back up.

## Deploy (Vercel)

Static site, no build step.

1. Vercel: **Add New… → Project → Import** this repo.
2. Framework Preset: **Other**. No build command. Output Directory: default (`.`).
3. **Deploy.** Every push auto-deploys.

Live URLs:
- `https://<project>.vercel.app/`
- `https://<project>.vercel.app/prototypes/applications/availability-nav/`

## Add a new prototype

1. Create `prototypes/<module>/<name>/index.html` (self-contained).
2. Add a linking card to that module's `index.html` (create the module landing page if it's new).
3. Commit and push — Vercel redeploys automatically.
