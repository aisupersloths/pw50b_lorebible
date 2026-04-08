---
title: Global TODO
type: process
status: canon
scope: repository
---

# Global TODO

This file is the main agent task backlog.

## Agent behavior rules

Agents may:
- mark tasks complete
- split tasks into subtasks
- create new tasks or subtasks
- update status and notes

Agents must:
- preserve task IDs
- preserve status values
- preserve dependencies when known
- avoid silently rewriting task intent

## Task schema

Each task should follow this structure:

```md
- [STATUS] TASK-ID Title
  - Type: canon | ontology | research | synthesis | consistency | export | test | story
  - Priority: P1 | P2 | P3
  - Scope: repository | galaxy | world | culture | system | platform | export
  - Depends on: TASK-ID, ... | none
  - Acceptance:
    - condition 1
    - condition 2
  - Notes:
    - optional note
```

## Status values

- `todo`
- `in_progress`
- `blocked`
- `done`

## Tasks

- [todo] PW50B-T001 Define stability framework
  - Type: research
  - Priority: P1
  - Scope: galaxy
  - Depends on: none
  - Acceptance:
    - define the axes of stability used by the setting
    - define what timescales count as stable
    - define a current working default for a median world
    - state major downstream consequences of stability choices

- [todo] PW50B-T002 Model world-specific population structures
  - Type: research
  - Priority: P1
  - Scope: world
  - Depends on: PW50B-T001
  - Acceptance:
    - identify what variables influence population percentages
    - identify what variables influence child-rearing percentages
    - identify key socioeconomic consequences of those percentages
    - keep results world-specific rather than falsely universal

- [todo] PW50B-T003 Build naming rules
  - Type: ontology
  - Priority: P1
  - Scope: repository
  - Depends on: none
  - Acceptance:
    - create controlled vocabulary rules
    - define forbidden sloppy substitutions
    - define proper noun reuse rules
    - define local-language vs canon-language handling

- [todo] PW50B-T004 Create initial agent benchmark suite
  - Type: test
  - Priority: P1
  - Scope: repository
  - Depends on: none
  - Acceptance:
    - benchmark canon retrieval
    - benchmark anti-Earth compliance
    - benchmark authority-order compliance
    - benchmark ambiguity escalation behavior
    - benchmark non-universalization of local examples

- [todo] PW50B-T005 Design Perchance export schema
  - Type: export
  - Priority: P2
  - Scope: export
  - Depends on: PW50B-T003
  - Acceptance:
    - define Perchance-safe exported data shapes
    - define negative constraint exports
    - define which canon files feed which export lists
    - define how generators avoid consuming irrelevant artifacts
