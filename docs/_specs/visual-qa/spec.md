# Visual QA & Consistency — Spec

> **Status:** Planned

## Problem Statement

The museum depends heavily on visual credibility: aligned card borders, readable labels, consistent typography, disciplined spacing, and predictable image behavior. Small inconsistencies can make the exhibition feel improvised even when the curatorial structure is strong.

A dedicated visual QA workstream is needed so alignment and consistency are treated as governed quality work rather than informal cleanup.

## Design Goals

1. Create a repeatable alignment and typography baseline.
2. Keep object cards, portrait cards, and labels visually consistent.
3. Treat border fit, title overflow, and caption balance as real quality concerns.
4. Keep the QA process lightweight enough for a docs-folder static workflow.

## Architecture

### Focus Areas

- comic object cards
- portrait cards
- object/environment cards
- shared CSS typography and spacing
- room-to-room consistency checks

### Primary Files In Scope

- `docs/styles.css`
- `docs/media/*.svg`
- any `docs/*.html` pages whose image/caption layout needs adjustment

## Risks

### Inconsistency Risk

Visual systems may drift as new cards are added.

### Local Fix Risk

One-off fixes may solve a single card while making the broader system less consistent.

## Testing Strategy

### Required Validation Categories

1. SVG text and border fit review
2. CSS consistency review
3. HTML/CSS/SVG error checks
4. browser preview inspection across key pages
5. comparison against the shared card system rather than one-off exceptions

## Sprint Plan

| Sprint   | Goal                                                         |
| -------- | ------------------------------------------------------------ |
| Sprint 0 | Standardize comic issue cards                                |
| Sprint 1 | Standardize portrait and object cards                        |
| Sprint 2 | Perform full-site visual QA and continuity review            |
| Sprint 3 | Document design comparison and review the live hybrid museum |

## Future Considerations

- optional checklist for mobile/browser-specific review
- room-by-room visual regression checklist
- comparison-review checklist for prototype-vs-live design decisions
