# Curatorial Enrichment — Spec

> **Status:** Planned

## Problem Statement

The Comic Book Museum now has a stable curatorial foundation and a coherent static exhibition surface, but its collection logic is still light. Objects, people, rooms, and evidence surfaces exist visually, yet the project does not fully encode why each object matters, how rooms should be enriched, or how future additions should be grouped and justified.

Without a dedicated enrichment workstream, new content risks becoming decorative rather than curatorial.

## Design Goals

1. Strengthen the museum's object logic with clearer curatorial roles.
2. Expand rooms through historically meaningful additions rather than filler.
3. Improve cast and institution logic so people pages feel interpretive, not directory-like.
4. Tie new additions back to the chronology spine.
5. Keep all enrichment bounded by the existing collection model and museum thesis.

## Architecture

### Focus Areas

This workstream is organized around three systems:

1. **Collection metadata** — stronger object fields, roles, and significance notes.
2. **Room enrichment** — adding or sharpening content inside chronology and companion rooms.
3. **Cast logic** — improving how creators, publishers, and studios are grouped and interpreted.

### Entry-Sequence Note

The public entry page should frame the visitor before they enter the chronology spine. In this repo, `docs/index.html` acts as a threshold surface, while `docs/home.html` carries the main opening-gallery content. Curatorial enrichment work should preserve that distinction: the hero page should orient, signal tone, and prepare arrival, while interpretive depth should accumulate in the opening gallery and the chronology rooms that follow.

### Primary Files In Scope

- `docs/index.html`
- `docs/home.html`
- `docs/content/collection-model.md`
- `docs/eras/*.html`
- `docs/people-and-studios.html`
- `docs/reading-maps/publication-lineage.html`
- `docs/guides/collection-highlights.html`
- `docs/media/*.svg` when new object cards are justified

## Risks

### Over-Expansion Risk

The site may accumulate too many objects or characters without improving the visitor's understanding.

### Flat Cast Risk

The people page may read like a roster instead of a historically grouped interpretive surface.

### Redundant Evidence Risk

New objects may repeat what existing rooms already prove.

## Testing Strategy

### Required Validation Categories

1. room additions map to a clear curatorial role
2. cast additions are grouped interpretively
3. object additions strengthen rather than duplicate the chronology
4. edited HTML/CSS/SVG files remain error-free
5. navigation and internal linking remain coherent

## Sprint Plan

| Sprint   | Goal                                                                    |
| -------- | ----------------------------------------------------------------------- |
| Sprint 0 | Expand the collection model with stronger object and room-role guidance |
| Sprint 1 | Enrich the cast and institutions surface with stronger grouping logic   |
| Sprint 2 | Add room-level enrichment and run a cross-room consistency pass         |

## Future Considerations

- accession-style labels and provenance notes
- curator notes for each room
- historical sources or bibliography surface
