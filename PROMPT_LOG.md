# Prompt Log

## Purpose

This file is a reconstructed record of the major prompts used in this workspace session and the resulting outcomes. It is intended as a durable project memory for future review.

## Notes

- This log captures the substantive prompts and outcomes from the session.
- Short acknowledgements such as "ok" or "yes do that" are only included where they changed direction or approved a concrete implementation step.
- The outcomes below are based on the session history and the current repository state.

## Session Record

### 1. Import and reference review

**Prompt:** clone/import `https://github.com/kaw393939/nextjs_ai_orchestration_spec_sprint_process` into GitHub.

**What happened:**

- Repository import and GitHub access/setup were investigated.
- The AI museum repository and live site were then used as a reference point for later design and process decisions.

**Outcome:**

- The reference project became the structural and workflow model for this museum repo.

---

### 2. Evaluate the AI museum as a reference

**Prompt:** review the AI museum repo and site, identify the strongest ideas, review the process used to create it, and evaluate it not just as a website but as an exhibit.

**What happened:**

- The AI museum project was analyzed for narrative flow, exhibition logic, curation, room structure, and workflow patterns.
- Its strongest transferable ideas were identified as chronology-led structure, durable documentation, specs-driven workflow, and exhibit-style interpretation.

**Outcome:**

- The Marvel project direction was reframed around museum logic instead of generic website presentation.

---

### 3. Build a Marvel museum modeled on the reference project

**Prompt:** recreate the design in this repo based on the Marvel comic museum idea and the structure of the AI History Museum design.

**What happened:**

- An initial app-style implementation was scaffolded with process documentation inspired by the AI museum workflow.
- That version was later replaced after the project direction changed to static HTML/CSS.

**Outcome:**

- The repo briefly had an app-based implementation, but this was later removed in favor of a static museum.

---

### 4. Switch to HTML/CSS pages

**Prompt:** make it as HTML/CSS files for the site, with page-to-page navigation.

**What happened:**

- The project was rebuilt as a multi-page static museum.
- A dedicated static site structure was created with linked pages, shared CSS, and media assets.

**Outcome:**

- The museum became a static multi-page exhibition rather than an app framework project.

---

### 5. Make it a real museum exhibition, not a process-explainer

**Prompt:** the site should be a genuine museum exhibition with artifacts, images, objects, and interpretation, not a site that explains the design process.

**What happened:**

- Visitor-facing copy and structure were rewritten to present the museum as an exhibition.
- The focus shifted to rooms, artifacts, creators, studios, chronology, and publication lineage.

**Outcome:**

- The public site became museum-facing, while process explanation moved into documentation rather than visitor pages.

---

### 6. Remove abstract shapes and use pictures of what is being presented

**Prompt:** get rid of the shapes and use pictures of what is being presented across the whole website.

**What happened:**

- Abstract geometric display elements were replaced with object-based, comic-based, and portrait-based illustrations.
- New SVG media assets were created for comic issues, creators, studios, and museum-style objects.

**Outcome:**

- The visual language became object-driven and more aligned with a real exhibition.

**Key assets created/used:**

- `docs/media/marvel-comics-1.svg`
- `docs/media/fantastic-four-1.svg`
- `docs/media/amazing-fantasy-15.svg`
- `docs/media/infinity-gauntlet.svg`
- `docs/media/bullpen-desk.svg`
- `docs/media/mcu-helmets.svg`
- portrait SVGs in `docs/media/`

---

### 7. Perform visual QA and fix alignment issues

**Prompt:** review the site for font, size, and border alignment issues, including problems like the `Amazing Fantasy` title alignment, and then check for other similar errors.

**What happened:**

- Multiple QA passes were performed on the comic cards and supporting visual systems.
- Typography, title strips, caption boxes, nameplates, and border alignment were standardized.
- A broader card-system normalization followed to prevent one-off fixes.

**Outcome:**

- The visual system became more consistent across comic cards, object cards, and portrait cards.

---

### 8. Delete files that were no longer used

**Prompt:** delete all files that are not being used.

**What happened:**

- The repository was audited for active versus obsolete surfaces.
- The earlier app stack and related configuration/build files were identified as unused and removed.

**Outcome:**

- The repo was simplified around the active museum implementation and supporting documentation.

---

### 9. Compare the repo against the AI museum and identify missing process/curatorial structure

**Prompt:** look back at the AI museum repo and see what process or structure was missing in terms of a specs-driven and curator application.

**What happened:**

- The current repo was compared against the AI museum's durable process layer.
- Missing foundations were identified: curator-facing philosophy, implementation codex, workstream specs, sprint docs, content model, and QA guidance.

**Outcome:**

- A formal documentation and governance layer was planned and added under `docs/`.

---

### 10. Rebuild the missing process layer

**Prompt:** yes, do that.

**What happened:**

- The repo gained a durable docs/process system.
- Foundation docs, specs, sprint docs, and a collection model were added.

**Outcome:**

- The museum became both a visitor-facing site and a documented, maintainable system.

**Key files added:**

- `docs/foundation/site-design-philosophy.md`
- `docs/foundation/site-implementation-codex.md`
- `docs/foundation/site-spec-patterns.md`
- `docs/foundation/orchestration-method.md`
- `docs/content/collection-model.md`
- `docs/_specs/README.md`
- `docs/_specs/site-exhibition/spec.md`
- `docs/_specs/site-exhibition/sprints/*.md`
- `docs/_specs/curatorial-enrichment/spec.md`
- `docs/_specs/curatorial-enrichment/sprints/*.md`
- `docs/_specs/visual-qa/spec.md`
- `docs/_specs/visual-qa/sprints/*.md`

---

### 11. Set up the repo for GitHub Pages from `main` and `/docs`

**Prompt:** set up the files so the repo can publish with GitHub Pages from branch `main` and folder `docs`.

**What happened:**

- The active museum was copied into `docs/`.
- `docs/.nojekyll` was added so `_specs/` would not be ignored by GitHub Pages.
- The README was updated to reflect Pages publishing.

**Outcome:**

- The repo became compatible with GitHub Pages deployment from `main` → `/docs`.

---

### 12. Make `docs/` the single source of truth

**Prompt:** yes, do that.

**What happened:**

- References to the old `static-site/` folder were updated across docs and specs.
- The duplicate `static-site/` folder was deleted after `docs/` was confirmed as the canonical source.

**Outcome:**

- `docs/` now serves as both the live museum and the process/documentation source of truth.

---

### 13. Tighten the README for presentation and handoff

**Prompt:** yes, do that.

**What happened:**

- The root README was rewritten as a clearer project overview.
- It now explains the museum concept, repo structure, Pages deployment, and the role of the docs/process layer.

**Outcome:**

- The repo gained a cleaner presentation document suitable for review, grading, and maintenance.

**Key file updated:**

- `README.md`

---

### 14. Provide a GitHub Pages publishing checklist

**Prompt:** provide a quick checklist for publishing on GitHub Pages.

**What happened:**

- A concise deployment checklist was provided covering GitHub settings, sanity checks, and troubleshooting.

**Outcome:**

- The project now has clear manual steps for publishing from `main` → `/docs`.

---

### 15. Standardize sprint docs to a required format

**Prompt:** make sure each sprint doc follows this format: Goal, Scope (in/out), Tasks, Files to touch, Acceptance criteria, Verification checklist, Completion evidence.

**What happened:**

- All sprint documents were reviewed and normalized.
- Older headings such as `Header`, `Verify`, and `Completion Checklist` were replaced with the required section structure.

**Outcome:**

- All sprint docs now follow one consistent template.

**Affected areas:**

- `docs/_specs/site-exhibition/sprints/`
- `docs/_specs/curatorial-enrichment/sprints/`
- `docs/_specs/visual-qa/sprints/`

---

### 16. Create an `AGENTS.md` file with project instructions

**Prompt:** create an `AGENTS.md` file with all the instructions given during the session.

**What happened:**

- A root `AGENTS.md` file was created capturing the standing rules for project identity, docs-as-source-of-truth, visual discipline, writing style, process model, sprint requirements, QA, and GitHub Pages deployment.

**Outcome:**

- Future agents now have an explicit instruction file tailored to this repository.

**Key file added:**

- `AGENTS.md`

---

### 17. Create a prompt log

**Prompt:** create a `PROMPT_LOG.md` that records the prompts run here and what happened.

**What happened:**

- This file was created as a durable, high-level reconstruction of the session.

**Outcome:**

- The repo now contains a session memory artifact documenting the major requests and resulting changes.

**Key file added:**

- `PROMPT_LOG.md`

---

### 18. Add a dedicated hero entry page before the museum homepage

**Prompt:** create a separate hero page that visitors see first, with a collage background, a centered museum card, author credit, and an `Enter Exhibit` button leading to the main homepage.

**What happened:**

- The site entry flow was changed so `docs/index.html` acts as a dedicated threshold page.
- The prior homepage content was moved to `docs/home.html` so the main exhibition could still open as a full room after the splash screen.
- The hero page was styled with a centered entry card and supporting CSS in the shared stylesheet.

**Outcome:**

- The museum now begins with a distinct arrival surface before the visitor enters the main exhibition homepage.

**Key files updated:**

- `docs/index.html`
- `docs/home.html`
- `docs/styles.css`

---

### 19. Replace placeholder hero imagery with local comic-cover collage assets

**Prompt:** use actual images for the hero background collage and keep them stored locally in `docs/media/` rather than relying on brittle external hotlinks.

**What happened:**

- Candidate image sources were researched and a local-asset approach was chosen for reliability.
- Downloaded comic-cover JPGs were added to `docs/media/` and then wired into the hero background collage.
- The collage CSS was updated so the entry page uses museum assets already inside the repository.

**Outcome:**

- The hero page now uses a stable, locally served comic collage instead of remote placeholder imagery.

**Key files updated:**

- `docs/media/*.jpg`
- `docs/styles.css`

---

### 20. Change the hero backdrop to a galaxy starfield

**Prompt:** change the background behind the comic collage from white to a galaxy field with stars.

**What happened:**

- The base hero background layer was reworked from a light museum-paper gradient to a dark starfield built from layered gradients.
- The comic-cover collage remained in place on top of the new backdrop.

**Outcome:**

- The entry page now presents the comic covers against a darker, more dramatic space-like field.

## Current Repository State

At the end of this log, the repository is organized around these active areas:

- `docs/` — live museum and all supporting documentation
- `docs/index.html` — public hero-entry page
- `docs/home.html` — main opening-gallery homepage
- `README.md` — project overview and publishing guidance
- `AGENTS.md` — standing agent instructions for future work
- `PROMPT_LOG.md` — reconstructed session history

## Current Publishing Model

- GitHub Pages branch: `main`
- GitHub Pages folder: `/docs`
- Public entry point: `docs/index.html`
- Opening-gallery homepage: `docs/home.html`
- Required Pages support file: `docs/.nojekyll`
