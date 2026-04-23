# Sprint 3 — Hero Entry Sequence

## Goal

Introduce a dedicated public entry page that behaves like a museum threshold before the visitor enters the main opening gallery.

## Scope

### In

- define the entry-sequence split between `docs/index.html` and `docs/home.html`
- create a hero splash page with museum title, author credit, and `Enter Exhibit` action
- use a collage of locally stored comic-cover assets as the visual field
- establish a starfield backdrop behind the collage to strengthen arrival drama
- document the entry sequence in repository guidance so Pages behavior and file roles remain clear

### Out

- redesigning the chronology rooms or supporting rooms beyond entry-flow adjustments
- replacing the broader visual system outside hero-page needs
- adding new JavaScript-based transitions or animation systems
- changing GitHub Pages deployment away from `main` -> `/docs`

## Tasks

1. Reassign the public entry flow.

- keep `docs/index.html` as the GitHub Pages entry point
- move the main opening-gallery homepage to `docs/home.html`
- ensure the hero page routes visitors into the exhibition with a clear button action

2. Build the hero-page visual system.

- center a museum card with title and author credit
- compose the background from locally stored comic-cover images in `docs/media/`
- add a galaxy-style starfield behind the collage rather than a flat light backdrop

3. Document the new structure.

- record the entry-page behavior in repository guidance
- keep README, claims, and prompt-history references aligned with the actual implementation
- make the new sprint discoverable in the site-exhibition spec and specs index

## Files to touch

- `docs/index.html`
- `docs/home.html`
- `docs/styles.css`
- `docs/media/` hero collage assets
- `README.md`
- `AGENTS.md`
- `CLAIMS.md`
- `PROMPT_LOG.md`
- `docs/_specs/site-exhibition/spec.md`
- `docs/_specs/README.md`
- this sprint doc

## Acceptance criteria

- `docs/index.html` functions as a dedicated hero-entry page rather than the main opening gallery
- `docs/home.html` holds the primary homepage / opening-gallery content
- the hero page includes the museum title, author credit, and an `Enter Exhibit` route into `docs/home.html`
- the background collage uses local media assets rather than brittle hotlinked images
- the backdrop behind the collage reads as a starfield / galaxy field rather than a white page background
- repository documentation reflects the new entry sequence and file roles accurately

## Verification checklist

- [ ] verify `docs/index.html` links to `docs/home.html`
- [ ] verify the hero collage references assets present in `docs/media/`
- [ ] verify the CSS renders the starfield backdrop behind the collage layers
- [ ] verify `README.md`, `AGENTS.md`, `CLAIMS.md`, and `PROMPT_LOG.md` describe the entry sequence consistently
- [ ] verify the site-exhibition spec and specs index include this sprint
- [ ] verify the edited HTML/CSS/Markdown files contain no reported errors

## Completion evidence

- Repository paths: `docs/index.html`, `docs/home.html`, `docs/styles.css`, `docs/media/*.jpg`
- Repository paths: `README.md`, `AGENTS.md`, `CLAIMS.md`, `PROMPT_LOG.md`
- Repository paths: `docs/_specs/site-exhibition/spec.md`, `docs/_specs/README.md`, `docs/_specs/site-exhibition/sprints/sprint-3-hero-entry-sequence.md`
- Commit: `aa1245d` (`Created a Hero Page`)
- Follow-on progress-session evidence: the opening gallery continued to be refined after live review so the threshold object remained the dominant entry artifact while the supporting reinvention object stayed layered at smaller widths
- Follow-on live files: `docs/home.html`, `docs/styles.css`, `docs/media/marvel-comics-1.jpeg`, `docs/media/fantastic-four-1.jpeg`
