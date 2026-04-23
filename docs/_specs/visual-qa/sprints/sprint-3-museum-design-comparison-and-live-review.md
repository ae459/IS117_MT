# Sprint 3 — Museum Design Comparison And Live Review

## Goal

Compare the live Comic Book Museum against the isolated `Example/museum-layout` prototype, document the design review, and apply the approved single-page / museum-hybrid refinements without losing the curator-led exhibition logic.

## Scope

### In

- compare the live museum opening and route structure against `Example/museum-layout.html` and `Example/museum-layout.css`
- document what should be borrowed from the prototype and what should stay museum-specific
- review the live site through a Bruno Simon / Daniel Spatzek-style single-page lens while preserving the repository's curatorial rules
- implement focused spacing, hierarchy, and overlap fixes required by the comparison review
- record the resulting live-system changes in sprint evidence and repository memory docs

### Out

- replacing the museum with the placeholder example wholesale
- removing the hero-entry threshold at `docs/index.html`
- flattening the exhibition into a generic landing page with no chronology spine
- rewriting unrelated foundation docs beyond changes needed to document the sprint and its outcomes

## Tasks

1. Compare prototype and live museum.
   - read `Example/museum-layout.html`, `Example/museum-layout.css`, and the active `docs/` pages
   - identify which prototype behaviors improve immersion without weakening the museum identity
2. Document the hybrid design decision.
   - preserve `docs/index.html` as the separate threshold page
   - consolidate the rest of the museum into `docs/home.html` as a single continuous exhibition route
   - define the design rule: prototype energy in macro-composition, museum discipline in captions, objects, chronology, and interpretation
3. Apply the approved live-site refinements.
   - restructure the opening gallery into a single-page exhibition route
   - borrow scale contrast, route gestures, and object-led staging from the prototype
   - review spacing, overflow, caption fit, and overlap on the opening and wall sections
4. Record outcomes in repository memory artifacts.
   - update `PROMPT_LOG.md`
   - update `CLAIMS.md` for any new repository-state claims introduced by the sprint

## Files to touch

- `docs/home.html`
- `docs/index.html`
- `docs/styles.css`
- `docs/_specs/visual-qa/spec.md`
- `docs/_specs/README.md`
- this sprint doc
- `PROMPT_LOG.md`
- `CLAIMS.md`

## Acceptance criteria

- the comparison between prototype and live museum is documented as a bounded sprint artifact
- `docs/index.html` remains the only separate threshold page
- `docs/home.html` functions as the single long-form exhibition route for the rest of the museum
- the live design borrows immersive layout rhythm from the prototype without losing chronology-first museum logic
- opening and wall sections no longer suffer from caption/image overlap or cramped layout behavior
- repository memory docs reflect the comparison review and resulting design decisions

## Verification checklist

- [x] review `Example/museum-layout.html` and `Example/museum-layout.css` against the live museum
- [x] verify the redesign keeps the museum logic described in `AGENTS.md`
- [x] run error checks on `docs/home.html`, `docs/index.html`, and `docs/styles.css`
- [x] review the opening gallery and wall section for spacing, caption fit, and overlap problems
- [x] confirm the sprint is reflected in the spec/index/log documentation

## Completion evidence

- Repository paths: `docs/index.html`, `docs/home.html`, `docs/styles.css`, `Example/museum-layout.html`, `Example/museum-layout.css`, `docs/_specs/visual-qa/spec.md`, `docs/_specs/README.md`, `PROMPT_LOG.md`, `CLAIMS.md`
- Comparison result: the prototype remained isolated in `Example/`, while its approved layout logic informed the live hybrid museum route
- Live outcome: `docs/index.html` remains the threshold page and `docs/home.html` now carries the single-page exhibition route
- QA evidence: later spacing and overlap fixes were applied to the opening gallery and collection-wall presentations after browser review screenshots exposed caption/image collisions
- PR / commit: pending repository commit
- Progress-session feedback incorporated: the example's navigation hierarchy informed the live two-tier exhibit-map header, while the live opening retained a staged threshold object with a visibly overlapping reinvention inset on smaller screens
- Asset evidence: the live museum moved from placeholder object illustrations to real local JPEG covers, portraits, and prop imagery while preserving the prototype as an isolated sandbox
