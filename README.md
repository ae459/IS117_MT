# Marvel Bauhaus Museum

Marvel Bauhaus Museum is a static HTML/CSS digital exhibition that presents Marvel history as a curated museum experience rather than a conventional fan site. The project combines Bauhaus-inspired visual order with comic-book subject matter, organizing the collection around chronology, artifacts, creators, studios, and publication lineage.

## Project Overview

This repository uses `docs/` as the single source of truth for both:

1. the live GitHub Pages exhibition
2. the curatorial, specification, and QA documentation that supports it

That structure keeps the public-facing museum and the behind-the-scenes decision-making in one place, making the project easier to maintain, review, and present.

## Exhibition Experience

The visitor-facing museum includes:

- an opening gallery at `docs/index.html`
- three chronology-based exhibition rooms in `docs/eras/`
- a publication lineage room in `docs/reading-maps/`
- a people and studios room in `docs/people-and-studios.html`
- a collection highlights room in `docs/guides/`
- custom object, comic, and portrait illustrations in `docs/media/`

## Repository Structure

- `docs/index.html` main entry point for the museum
- `docs/styles.css` shared visual system and layout rules
- `docs/eras/`, `docs/guides/`, `docs/reading-maps/`, `docs/media/` active exhibition files
- `docs/_specs/` specs and sprint documents for major workstreams
- `docs/foundation/` durable design philosophy and implementation guidance
- `docs/content/` collection-model and content-architecture notes

## Process and Documentation

The museum follows a lightweight specs-driven workflow inspired by the AI museum reference project:

- spec -> sprint -> implementation -> QA

Key documents:

- `docs/_specs/README.md`
- `docs/foundation/site-design-philosophy.md`
- `docs/foundation/site-implementation-codex.md`
- `docs/foundation/site-spec-patterns.md`
- `docs/content/collection-model.md`

## GitHub Pages Deployment

Publish the site with GitHub Pages using:

- Branch: `main`
- Folder: `/docs`

The file `docs/.nojekyll` is included so GitHub Pages will not ignore underscore-prefixed directories such as `docs/_specs/`.

## Review and QA

Because the museum is built as a static site, the main review checks are:

- HTML, CSS, and SVG validation
- internal link and media-path verification
- visual QA for alignment, spacing, caption fit, and room-to-room consistency
- exhibit coherence across chronology, artifacts, and supporting interpretation

## Purpose

This project is designed to function as both a museum exhibition and a maintainable system. The goal is not only to present Marvel material attractively, but to do so with a clear curatorial structure, consistent visual language, and documentation that supports future revision.
