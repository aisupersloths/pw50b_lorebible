---
title: Canon Rules
type: governance
status: canon
scope: repository
---

# Canon Rules

## 1. Source of truth

The source of truth is the Markdown corpus in git.

Do not treat the following as canonical unless and until they are merged here:
- chats
- canvases/artifacts
- project instructions
- ad hoc summaries
- Perchance generators
- temporary staging drafts

## 2. Authority order

Unless the user explicitly says otherwise:
1. most recent explicit user statements on the relevant topic
2. earlier explicit user statements
3. assistant-generated extrapolations explicitly endorsed by the user
4. `deepfuture.pdf`
5. all other assistant speculation

## 3. Ambiguity handling

If authority is unclear:
- do not guess
- ask the user
- identify the precise ambiguity
- identify the sources in tension
- state what each source implies
- state what downstream decision depends on the answer

If the ambiguity is local and non-blocking, continue the rest of the task while bracketing the unresolved part.

If the ambiguity is foundational or blocking, stop the affected change and ask before proceeding.

## 4. Canon vs non-canon

Use these status classes:
- `canon` — settled current truth
- `tentative` — current but explicitly unresolved or incomplete
- `artifact` — derived, useful, clearly non-canon work product

Avoid adding extra status classes unless needed.

## 5. Write paths

### Agents without PR capability
- may not directly edit canon
- write to staging/artifact areas instead
- user later promotes, rejects, or rewrites material

### Agents with PR capability
- may edit canon directly
- user review occurs through pull requests

## 6. Current-lore-only rule

Do not preserve superseded ideas inside the lore bible merely for historical reference.
Git history is sufficient.

## 7. Ontology discipline

Facts and ontology are different.

A fact change adds or revises content inside the existing conceptual map.
An ontology change adds, removes, splits, or merges a core category.

Ontology changes require extra caution because they affect:
- glossary
- personhood rules
- law
- demographics
- tests
- naming rules
- story assumptions

## 8. Earth-forgetting rule

For all practical narrative purposes, nobody knows Earth.

Do not introduce:
- remembered Earth geography
- remembered Solar System geography
- remembered terrestrial nations, religions, or cultures
- prestige attached to Earth origin
- continuity myths anchored to recognizable Earth referents

Earth is true only as an objective deep past that is culturally nonexistent.

## 9. No false universalization

Do not turn world-specific arrangements into galaxy-wide defaults without explicit support.
This especially applies to:
- population percentages
- child-rearing percentages
- stability levels
- food/housing/reproduction norms
- legal structures
- economic incentives

## 10. Agent outputs allowed

Allowed outputs include:
- canon edits
- staging drafts
- contradiction/consistency reports
- benchmark/test outputs
- non-canon story scaffolds
- export artifacts

These must remain clearly separated.

## 11. Non-canon artifact isolation

Artifacts must be documented so agents do not waste context on them unless explicitly instructed.
Artifacts should:
- live outside canon areas
- be marked `status: artifact`
- say what they are for
- say they are not authority sources

## 12. Promotion rule

Nothing becomes canon just because an agent produced it.
Canon status depends on merge/review and the authority order.
