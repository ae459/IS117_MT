# Specifications Index

This directory contains the feature specs and sprint documents that govern the Comic Book Museum. The working rule for this project is simple: spec -> sprint -> implementation -> QA. The site may be static HTML/CSS, but the planning model is still durable, bounded, and curator-driven.

For the full method, read `docs/foundation/orchestration-method.md`.

## Workstreams

| Workstream                                             | Status            | Sprints | What It Produces                                                                         |
| ------------------------------------------------------ | ----------------- | ------: | ---------------------------------------------------------------------------------------- |
| [site-exhibition](site-exhibition/spec.md)             | Active foundation |       4 | Curatorial thesis, room system, entry sequence, object surfaces, and QA baseline         |
| [curatorial-enrichment](curatorial-enrichment/spec.md) | Planned           |       3 | Stronger collection model, cast logic, room enrichment, and evidence discipline          |
| [visual-qa](visual-qa/spec.md)                         | Planned           |       3 | Card alignment standards, typography consistency, and full-site visual continuity review |

## How To Read This Folder

1. Start with the workstream `spec.md`.
2. Read the sprint docs in order.
3. Implement only one sprint-sized unit at a time.
4. Record verification and any deviations before moving on.

## Recommended Order

1. `site-exhibition` — establishes the museum's durable curatorial and process foundation
2. `curatorial-enrichment` — expands content and interpretive depth without losing the chronology spine
3. `visual-qa` — enforces the visual discipline that protects the museum's credibility

## House Shape

### Specs do this work

- define the problem clearly
- state design and curatorial goals
- describe required architecture and artifact systems
- identify scope, accuracy, and drift risks
- define verification before implementation starts
- break the feature into bounded sprints

### Sprint docs do this work

- name one narrow delivery goal
- cite the governing spec sections
- identify available assets and artifact targets
- define exact tasks and outcomes
- state the verification method
- end with a completion checklist and QA deviations section
