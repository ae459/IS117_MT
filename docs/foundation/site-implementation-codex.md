# Site Implementation Codex

## Purpose

This document explains where the museum's coherence lives in the current static HTML/CSS implementation so future changes can be made without improvising the architecture.

## Current Project Surface

The active product lives entirely under `docs/`.

### Route map

- `docs/index.html` -> opening gallery and route hub
- `docs/eras/golden-age.html` -> Room 1
- `docs/eras/marvel-age.html` -> Room 2
- `docs/eras/cinematic-age.html` -> Room 3
- `docs/reading-maps/publication-lineage.html` -> issue evidence room
- `docs/people-and-studios.html` -> cast and institutions room
- `docs/guides/bauhaus-marvel-language.html` -> object gallery / collection highlights

## CSS Architecture

Shared styling lives in `docs/styles.css`.

The main systems are:

- shell and navigation (`site-header`, `site-footer`, `site-nav`)
- room wrappers (`hero-panel`, `chapter-section`, `transition-block`)
- card surfaces (`content-card`, `artifact-card`, `editorial-aside`)
- image systems (`artifact-grid`, `image-strip`, `portrait-grid`, `artifact-figure`)
- theme accents (`theme-home`, `theme-golden`, `theme-marvel`, `theme-cinematic`, `theme-proof`, `theme-cast`, `theme-guide`)

## Media System

All current visuals live in `docs/media/`.

Media categories:

- issue/object cards: `marvel-comics-1.svg`, `fantastic-four-1.svg`, `amazing-fantasy-15.svg`, `infinity-gauntlet.svg`
- environment/object cards: `bullpen-desk.svg`, `mcu-helmets.svg`
- portrait cards: `martin-goodman.svg`, `jack-kirby.svg`, `stan-lee.svg`, `steve-ditko.svg`, `chris-claremont.svg`, `kevin-feige.svg`

## Navigation Model

The homepage is the orchestrator.

It introduces:

- opening objects
- the chronology spine
- companion room links
- highlight objects

Every other page should return the visitor to the main chronology or to a clearly related companion room.

## Curatorial Implementation Rules

When adding a new page or object:

1. identify whether it belongs to the chronology or a companion room
2. decide what evidence role it plays
3. use an existing card/image system before inventing a new one
4. tie the new surface back to the chronology spine
5. preserve visual consistency in border, spacing, and typography

## Verification Shape

Because the project is static HTML/CSS, verification is lightweight but still necessary.

Current baseline:

- ensure edited HTML/CSS/SVG files report no errors
- ensure referenced images and links still exist
- visually inspect alignment, spacing, and border fit in the browser preview

## Adaptation Rules

What should usually be preserved:

- chronology-first route structure
- companion-page model
- visible object/evidence surfaces
- disciplined shared CSS systems
- explicit visual hierarchy

What must change for new domains:

- the metaphor and subject matter
- artifact choices
- cast and institution groupings
- palette and imagery where appropriate
- room taxonomy if the subject does not fit a chronology spine
