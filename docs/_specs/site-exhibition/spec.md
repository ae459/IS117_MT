# Site Exhibition Specification

> **Status:** Active foundation

## Problem Statement

The Comic Book Museum currently has a strong static presentation surface, but it does not yet have a durable process layer that explains how the exhibition should evolve. Without specs, sprint docs, and curator-facing reference documents, the project is vulnerable to drift, inconsistent additions, and loss of curatorial intent across sessions.

## Design Goals

1. Preserve the chronology spine as the primary visitor route.
2. Treat companion pages as supporting rooms with clear evidence roles.
3. Keep images and objects central to interpretation.
4. Make future changes bounded, auditable, and repository-grounded.
5. Restore artifact memory through durable docs rather than chat memory.
6. Keep the process lightweight enough for a static HTML/CSS project.

## Architecture

### Primary Surfaces

The active product lives under `docs/` and currently consists of:

- public hero-entry page
- homepage / opening gallery
- three chronology rooms
- publication lineage room
- people and studios room
- collection highlights room
- shared CSS and artifact media

### Required Durable Documents

This workstream must maintain:

- `docs/foundation/site-design-philosophy.md`
- `docs/foundation/site-implementation-codex.md`
- `docs/foundation/site-spec-patterns.md`
- `docs/foundation/orchestration-method.md`
- `docs/content/collection-model.md`

### Process Artifacts

This workstream is governed by:

- `docs/_specs/README.md`
- this spec file
- sprint docs under `docs/_specs/site-exhibition/sprints/`

## Risks

### Drift Risk

The site may drift into a generic Marvel archive or ad hoc fan site if new content is added without a feature contract.

### Curatorial Dilution Risk

Pages may accumulate content without clear relation to the chronology spine or supporting-room logic.

### Visual Consistency Risk

Object cards, labels, and captions may lose alignment if changes are made without a shared verification baseline.

## Testing Strategy

### Required Validation Categories

1. repository accuracy
2. link and media reference integrity
3. HTML/CSS/SVG error checks
4. visual consistency review for cards, labels, and room hierarchy
5. spec-to-sprint traceability

## Sprint Plan

| Sprint   | Goal                                                                            |
| -------- | ------------------------------------------------------------------------------- |
| Sprint 0 | Rebuild the durable curatorial and process foundation documents                 |
| Sprint 1 | Define the room system, object model, and collection logic for future additions |
| Sprint 2 | Establish QA habits and continuity rules for docs-based museum evolution        |
| Sprint 3 | Introduce a hero-entry threshold and document the split between entry and home  |

## Future Considerations

- downstream feature workstreams such as `curatorial-enrichment` and `visual-qa`
- object accession labels and metadata tables
- room-level checklists for future page expansion
- accessibility-focused QA workstream
- docs-folder deployment and publishing workflow
