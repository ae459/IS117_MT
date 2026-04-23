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

---

### 21. Review web design archetypes and compare the museum against them

**Prompt:** explain the general archetypes for web design, identify famous designers associated with them, compare the museum design against those archetypes, and review the site as if it were being critiqued through a Khoi Vinh-style lens.

**What happened:**

- General web design archetypes were outlined, including landing, editorial, portfolio, e-commerce, dashboard, documentation, and museum/exhibition models.
- The museum was compared against notable web-design figures, with the strongest fit identified as a systems-first, grid-based editorial approach rather than an experimental or portfolio-driven one.
- A targeted critique was produced describing what to refine: more restrained hierarchy, stronger grid discipline, standardized cards, simplified navigation, tighter type rhythm, and better alignment between the entry page and the main opening gallery.

**Outcome:**

- The museum was more clearly framed as a curated editorial/exhibition system rather than a flashy experimental website.
- The critique directly informed the next implementation pass.

---

### 22. Apply a first-pass archetype-driven design refinement to the live site

**Prompt:** start applying the design changes first so the results could be reviewed before any further documentation updates.

**What happened:**

- The entry page and homepage were refined to feel more restrained and museum-like.
- Shared CSS was updated to tighten typography, spacing, card consistency, and overall visual hierarchy.
- The opening sequence was strengthened with a calmer threshold page and a cleaner homepage structure.

**Outcome:**

- The live museum gained a more deliberate first-pass visual system aligned with the earlier archetype critique.

**Key files updated:**

- `docs/index.html`
- `docs/home.html`
- `docs/styles.css`

---

### 23. Confirm the design direction and propagate approved system changes site-wide

**Prompt:** confirm the direction, then extend the approved changes across the museum and update the necessary files afterward.

**What happened:**

- Shared brand wording and internal route logic were propagated across the active museum pages.
- Internal `Opening gallery` navigation was standardized to point to `docs/home.html` as the real opening-gallery surface.
- Companion pages were aligned with the approved object-gallery route and the active guide page naming.
- The visual QA sprint record was updated to reflect completed review items and touched paths.

**Outcome:**

- The museum became more internally consistent across chronology pages, companion rooms, and route labels.

**Key files updated:**

- `docs/home.html`
- `docs/people-and-studios.html`
- `docs/eras/golden-age.html`
- `docs/eras/marvel-age.html`
- `docs/eras/cinematic-age.html`
- `docs/reading-maps/publication-lineage.html`
- `docs/guides/bauhaus-marvel-language.html`
- `docs/_specs/visual-qa/sprints/sprint-2-full-site-visual-review.md`

---

### 24. Commit design work and correct Git identity

**Prompt:** commit and push the recent changes, then set the Git username/email and amend the latest commit so the new identity is used.

**What happened:**

- Recent museum changes were committed and pushed to `main`.
- Global Git identity was updated to use the provided NJIT email and username.
- The latest commit was amended with `--reset-author` and force-pushed safely with `--force-with-lease`.

**Outcome:**

- The repository history now reflects the intended Git identity for later commits.

---

### 25. Make another focused live-site refinement pass

**Prompt:** fix the design a little more for the website.

**What happened:**

- The live entry page and homepage received another small visual pass focused on first-impression clarity.
- A stronger opening orientation was added with supporting note blocks and signpost cards.
- Shared styling was adjusted to improve hero rhythm, header presence, and museum-style framing.

**Outcome:**

- The live opening experience became clearer and more curated without changing the overall site structure.

**Key files updated:**

- `docs/index.html`
- `docs/home.html`
- `docs/styles.css`

---

### 26. Create isolated placeholder examples outside the live museum

**Prompt:** use placeholders only and put everything in a folder named `Example` so layout experiments can be deleted later without affecting the museum site.

**What happened:**

- An isolated `Example/` folder was created.
- A first demo page was added to show a comic-inspired layout using only framed placeholders and card systems.
- A second demo page was then created to mirror the museum homepage structure more closely while still using placeholder content.

**Outcome:**

- The repo gained a safe prototyping space separate from the live museum implementation.

**Key files added:**

- `Example/index.html`
- `Example/styles.css`
- `Example/museum-layout.html`
- `Example/museum-layout.css`

---

### 27. Review and redesign the isolated museum example through a more immersive lens

**Prompt:** compare the `museum-layout` example as if reviewed by designers like Bruno Simon or Daniel Spatzek, then proceed with a more immersive design pass while keeping all work inside the example files only.

**What happened:**

- The example prototype was critiqued as being strong in structure but less theatrical and experience-driven than those designers' work.
- The isolated museum-layout preview was redesigned with a more dominant hero object, layered floating inset cards, stronger asymmetry, a route-band gesture, and a more dramatic highlight mosaic.
- The changes remained fully sandboxed in the `Example/` folder and did not alter the live museum site.

**Outcome:**

- The repository now includes a stronger prototype for experimenting with bolder homepage treatments before transferring any ideas to the real museum.

**Key files updated:**

- `Example/museum-layout.html`
- `Example/museum-layout.css`

---

### 28. Compare the live museum against the `museum-layout` prototype

**Prompt:** compare and review the museum design with the `museum-layout.html` and CSS example in the `Example` folder, and read the prompt log session history.

**What happened:**

- The update log and both the example prototype and live museum files were reviewed together.
- The live museum was judged stronger as a curatorial exhibition system, while the example prototype was judged stronger as a single-page immersive homepage concept.
- A hybrid direction was identified: borrow scale contrast, asymmetry, and route gestures from the prototype while preserving the museum's chronology-first logic, object evidence, and interpretive writing.

**Outcome:**

- The repository gained a documented basis for merging the prototype's spatial energy into the live museum without discarding the curator-facing exhibition model.

---

### 29. Redefine the live structure as hero page plus one single-page exhibition

**Prompt:** preserve the separate hero page but turn everything else into a single page.

**What happened:**

- The design decision was clarified so `docs/index.html` would remain the only separate threshold page.
- `docs/home.html` was selected as the main single-page museum route containing the opening gallery, chronology, companion rooms, lineage, and collection highlights.
- Existing room pages were retained as reference/fallback surfaces rather than the primary route.

**Outcome:**

- The live museum's structure shifted from multi-page primary navigation to a hero-entry page plus a single long-form exhibition page.

---

### 30. Implement the live hybrid redesign

**Prompt:** proceed with the redesign.

**What happened:**

- `docs/home.html` was rebuilt into a single-page exhibition route with anchored room sections.
- `docs/styles.css` was extended with a more immersive opening stage, route band, room-band treatments, and highlight mosaic logic.
- `docs/index.html` was updated so the threshold page still leads visitors into the new single-page route.

**Outcome:**

- The live site adopted the approved hybrid model: a separate threshold page plus a single curator-led museum route.

**Key files updated:**

- `docs/home.html`
- `docs/index.html`
- `docs/styles.css`

---

### 31. Perform a spacing and visibility QA pass on the live museum

**Prompt:** review the live museum site and make sure the spacing is proper, all words remain visible, and nothing overlaps.

**What happened:**

- Shared CSS rules were tightened for text wrapping, grid item min-width behavior, sticky-header anchor offsets, and medium-width layout collapse.
- The live museum's opening gallery, gallery walls, and companion pages were reviewed for cramped spacing and title/caption fit.
- A second pass specifically targeted opening-gallery and collection-wall spacing.

**Outcome:**

- The live museum became more resilient against overflow, hidden section titles, cramped captions, and medium-width layout failures.

**Key files updated:**

- `docs/styles.css`

---

### 32. Fix visible overlap in the opening gallery and wall presentation

**Prompt:** address the visible overlap where wording was colliding with pictures on the opening and wall pages.

**What happened:**

- The opening-gallery feature-object caption was separated more clearly from the hero object stack.
- Floating-card sizing and positioning were revised so supporting evidence no longer collided with the main object label.
- Highlight and gallery-wall figures were given stronger framed-card behavior so captions stayed below imagery instead of collapsing into it.

**Outcome:**

- The live opening and collection-wall sections no longer exhibited the same caption/image overlap seen in browser screenshots.

**Key files updated:**

- `docs/styles.css`

---

### 33. Remove the extra opening-gallery logic card and do a targeted cleanup pass

**Prompt:** remove the small `Exhibit logic` card in the opening gallery and proceed with a very targeted pass.

**What happened:**

- The unnecessary lower floating card was removed from the opening gallery in `docs/home.html`.
- The opening hero was simplified so the main threshold object and the single supporting inset card read more clearly.
- Gallery-wall presentation styles were refined so collection objects felt more like framed museum surfaces.

**Outcome:**

- The opening gallery became cleaner and the object wall gained a more controlled museum-display feel.

**Key files updated:**

- `docs/home.html`
- `docs/styles.css`

---

### 34. Replace placeholder exhibit art with real local image assets

**Prompt:** use actual pictures for people, comic issues, and the prop wall, then test them in the live museum.

**What happened:**

- A concrete image shopping list was derived from the live pages so portraits, cover objects, and prop-wall imagery could be sourced deliberately.
- Real JPEG assets for key covers, portraits, and exhibit objects were added under `docs/media/` using normalized filenames.
- The active museum pages were updated to use those real local assets in place of the earlier placeholder SVG object surfaces.

**Outcome:**

- The live museum now presents real comic-cover, portrait, and prop imagery on its main object surfaces instead of relying on placeholder illustrations.

**Key files updated:**

- `docs/home.html`
- `docs/people-and-studios.html`
- `docs/reading-maps/publication-lineage.html`
- `docs/guides/collection-highlights.html`
- `docs/eras/golden-age.html`
- `docs/eras/marvel-age.html`
- `docs/eras/cinematic-age.html`
- `docs/media/*.jpeg`

---

### 35. Refine the live opening route after project-progress feedback

**Prompt:** continue refining the live museum by removing redundant opening sections, reducing the oversized header, and tightening the closing CTA behavior.

**What happened:**

- The oversized top header was reduced so the exhibit title and route controls felt less dominant.
- A redundant homepage signpost / route-intro section was removed so the opening gallery moved more directly into the chronology spine.
- The closing transition block was simplified so it kept only the useful `Back to top` action.

**Outcome:**

- The opening route became cleaner and more museum-like, with less explanatory clutter between the threshold object and the main chronology.

**Key files updated:**

- `docs/home.html`
- `docs/styles.css`

---

### 36. Prototype and adopt a hybrid exhibit-map navigation system

**Prompt:** explore a hybrid navigation pattern based on the example layout and then transfer the approved direction into the live museum.

**What happened:**

- An isolated prototype in `Example/museum-layout.html` tested visible desktop route tabs with a compact mobile treatment.
- The live museum first adopted the prototype's exhibit-map tabs, then was simplified again so the main chronology spine kept four large route tabs while companion rooms moved into a smaller secondary strip.
- Additional framing and border work separated the primary route tray from the companion-room row.

**Outcome:**

- The live header now reflects the example's stronger hierarchy: a primary chronology-led route and a distinct supporting-room band.

**Key files updated:**

- `Example/museum-layout.html`
- `Example/museum-layout.css`
- `docs/home.html`
- `docs/people-and-studios.html`
- `docs/reading-maps/publication-lineage.html`
- `docs/guides/collection-highlights.html`
- `docs/eras/golden-age.html`
- `docs/eras/marvel-age.html`
- `docs/eras/cinematic-age.html`
- `docs/guides/bauhaus-marvel-language.html`
- `docs/styles.css`

---

### 37. Preserve the reinvention inset card as a layered mobile object

**Prompt:** keep the `Reinvention object` visually staged over the threshold cover in the mobile layout instead of letting it collapse into a flat stacked card.

**What happened:**

- Responsive CSS for the opening gallery was revised so the inset `Fantastic Four #1` card remained absolutely positioned over the `Marvel Comics #1` object on smaller screens.
- Follow-up browser checks led to stronger mobile selectors and a larger inward offset so the inset card clearly overlaps the main cover rather than sitting beside it.

**Outcome:**

- The opening gallery now preserves more of its exhibit-style layering on smaller screens instead of flattening the supporting object into the normal document flow.

**Key files updated:**

- `docs/styles.css`

---

### 38. Prune the media folder to active exhibit assets only

**Prompt:** clean the media folder and remove pictures or SVGs that are no longer used.

**What happened:**

- The `docs/media/` directory was compared against all current references in the live `docs/` HTML and CSS.
- Duplicate source JPEGs, old placeholder SVGs, and other unreferenced media files were removed.

**Outcome:**

- `docs/media/` now contains only assets still referenced by the live museum implementation.

**Key files updated:**

- `docs/media/`

## Current Repository State

At the end of this log, the repository is organized around these active areas:

- `docs/` — live museum and all supporting documentation
- `docs/index.html` — public hero-entry page
- `docs/home.html` — main single-page exhibition route after the hero entry
- `Example/` — isolated placeholder and prototype layouts for design experiments
- `README.md` — project overview and publishing guidance
- `AGENTS.md` — standing agent instructions for future work
- `PROMPT_LOG.md` — reconstructed session history

## Current Publishing Model

- GitHub Pages branch: `main`
- GitHub Pages folder: `/docs`
- Public entry point: `docs/index.html`
- Main museum route: `docs/home.html`
- Required Pages support file: `docs/.nojekyll`
