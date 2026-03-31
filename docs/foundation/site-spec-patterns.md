# Site Spec Patterns

## Purpose

This document explains how to derive future specs and sprints from the current static museum without losing curatorial discipline.

## Drafting Sequence

1. read `docs/foundation/site-design-philosophy.md`
2. read `docs/foundation/site-implementation-codex.md`
3. identify the feature as a curatorial problem, not only a file-edit problem
4. write a feature spec before changing pages or CSS
5. derive bounded sprint docs from real product units
6. implement and verify one sprint at a time

## What A Spec Must Cover Here

A museum feature spec should include:

- problem statement
- design / curatorial goals
- architecture and artifact model
- drift and accuracy risks
- testing / verification strategy
- sprint plan

## What A Sprint Doc Must Cover Here

A sprint doc should include:

- the goal of one bounded unit
- referenced spec sections
- available assets and current repository facts
- exact file targets
- tasks and required outcomes
- verification method
- completion checklist
- QA deviations section

## Good Workstream Candidates For This Project

Examples of features that deserve their own spec package:

- room-by-room content enrichment
- collection data model and accession labels
- image consistency and caption QA
- navigation and visitor-route improvements
- accessibility and browser polish
- collection expansion with new objects and people

## Anti-Copying Rule

Do not use the docs to justify random page creation. New work should emerge from a clear museum need: stronger evidence, clearer chronology, better cast logic, cleaner visitor path, or tighter exhibition language.
