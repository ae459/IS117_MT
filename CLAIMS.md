# Claims Log

## Purpose

This file is the verification log for factual claims used in this repository. It records what the project claims, whether the claim has been verified, what evidence supports it, and what follow-up may still be needed.

## How To Use This File

- Add a new row when a factual claim is introduced in site copy, documentation, specs, or process notes.
- Prefer repository evidence first for implementation and project-structure claims.
- For historical or interpretive Marvel content, cite the research source or internal content model used to support the claim.
- Update the verification status when the claim is checked.

## Verification Status Legend

- `Verified` — confirmed by the current repository state or a documented source.
- `Partially verified` — supported in part, but still needs additional evidence or review.
- `Needs source` — currently asserted without a cited basis.
- `Superseded` — no longer current and kept only for recordkeeping.

## Verification Workflow

1. Identify the exact claim.
2. Locate where the claim appears.
3. Record the evidence source.
4. Mark the verification status.
5. Add follow-up notes if more research or QA is required.

## Current Repository Claims

| ID    | Claim                                                                                                                                                                               | Location                                                            | Status   | Evidence                                                                                                                                 | Notes                                                                   |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| C-001 | `docs/` is the single source of truth for the live site and project documentation.                                                                                                  | `README.md`, `AGENTS.md`                                            | Verified | Repository structure contains `docs/` as the active site and docs layer; root no longer contains `static-site/`.                         | Recheck if the repo structure changes.                                  |
| C-002 | The live GitHub Pages site is intended to publish from branch `main` and folder `/docs`.                                                                                            | `README.md`, `AGENTS.md`                                            | Verified | Deployment instructions are documented in both files; `docs/index.html` exists as the entry point.                                       | GitHub repository settings must still be configured manually in GitHub. |
| C-003 | `docs/.nojekyll` must remain present so `_specs/` is not ignored by GitHub Pages.                                                                                                   | `README.md`, `AGENTS.md`                                            | Verified | `docs/.nojekyll` exists in the repository.                                                                                               | Recheck after any deployment-related cleanup.                           |
| C-004 | The museum is a static HTML/CSS exhibition rather than an app framework surface.                                                                                                    | `README.md`, `AGENTS.md`, `PROMPT_LOG.md`                           | Verified | Active publish surface is composed of `docs/index.html`, linked HTML pages, `docs/styles.css`, and `docs/media/`.                        | If a framework is reintroduced later, update this claim.                |
| C-005 | The project follows a lightweight specs-driven workflow: spec -> sprint -> implementation -> QA.                                                                                    | `README.md`, `AGENTS.md`, `docs/foundation/orchestration-method.md` | Verified | The workflow is documented and corresponding folders exist in `docs/_specs/` and `docs/foundation/`.                                     | Process use should still be enforced in future work.                    |
| C-006 | Sprint docs are required for multi-surface changes and major work should be governed by specs.                                                                                      | `AGENTS.md`, `docs/_specs/`                                         | Verified | Policy is documented in `AGENTS.md`; workstream specs and sprint folders exist under `docs/_specs/`.                                     | Governance is procedural and should be checked during future changes.   |
| C-007 | Every sprint doc includes Goal, Scope, Tasks, Files to touch, Acceptance criteria, Verification checklist, and Completion evidence.                                                 | `AGENTS.md`, `docs/_specs/**/sprints/*.md`                          | Verified | Sprint docs were normalized to this format and validated.                                                                                | Recheck after future sprint edits.                                      |
| C-008 | The active museum includes a public entry/hero page, an opening gallery, chronology rooms, a publication lineage room, a people and studios room, and a collection highlights room. | `README.md`, `docs/`                                                | Verified | `docs/index.html`, `docs/home.html`, `docs/eras/`, `docs/reading-maps/`, `docs/people-and-studios.html`, and `docs/guides/` are present. | This verifies the structure, not the completeness of each room.         |
| C-009 | The visual system uses object, comic, and portrait imagery instead of abstract decorative shapes.                                                                                   | `README.md`, `AGENTS.md`, `docs/media/`                             | Verified | `docs/media/` contains comic, object, and portrait assets matching the documented approach.                                              | Recheck if new decorative assets are added later.                       |
| C-010 | The old `static-site/` directory was intentionally removed and should not be recreated as a parallel source.                                                                        | `AGENTS.md`, `PROMPT_LOG.md`                                        | Verified | Root directory no longer contains `static-site/`; removal is documented in the session log.                                              | This is a project-governance claim as well as a structural one.         |
| C-011 | The hero entry page routes visitors from `docs/index.html` into the main exhibition homepage at `docs/home.html`.                                                                   | `README.md`, `AGENTS.md`, `docs/index.html`                         | Verified | `docs/index.html` contains an `Enter Exhibit` link targeting `home.html`; documentation now describes that entry sequence.               | Recheck if the entry flow changes again.                                |
| C-012 | The hero-page collage uses locally stored media assets rather than relying on hotlinked remote images.                                                                              | `README.md`, `docs/styles.css`, `docs/media/`                       | Verified | `docs/styles.css` references hero collage images from `docs/media/`; the media directory contains downloaded comic-cover JPGs.           | Recheck after any hero-page redesign or media cleanup.                  |

## Claims That Still Need External Source Discipline

These categories should be logged here when edited in the public-facing museum content:

- Marvel publication dates
- creator biographies and roles
- studio formation timelines
- issue significance claims
- institutional or production-history claims
- interpretive statements that rely on historical chronology

For those claims, add:

- the page where the claim appears
- the source consulted
- whether the claim is direct fact, synthesis, or curatorial interpretation
- any unresolved ambiguity

## Suggested Entry Template

Use this template when adding a new claim:

| ID    | Claim                | Location           | Status                                                    | Evidence                                              | Notes                                |
| ----- | -------------------- | ------------------ | --------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------ |
| C-XXX | Exact factual claim. | File or page path. | Verified / Partially verified / Needs source / Superseded | Repository file, research source, screenshot, or URL. | Follow-up, caveats, or review notes. |
