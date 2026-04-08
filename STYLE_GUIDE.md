---
title: Style Guide
type: governance
status: canon
scope: repository
---

# Style Guide

## Goals

Write for:
- human readability
- LLM retrieval
- low ambiguity
- low token waste
- stable cross-platform use

## File structure

Each substantive file should start with YAML frontmatter.
Recommended fields:
- `title`
- `type`
- `status`
- `scope`
- `tags` (optional)
- `depends_on` (optional)

## Section discipline

Prefer explicit headings such as:
- Summary
- Canon
- Constraints
- Implications
- Open Questions
- Notes

## Sentence discipline

Prefer:
- short declarative statements
- explicit scope qualifiers
- direct definitions

Avoid:
- ornamental prose in canon files
- vague metaphor as definition
- hidden assumptions
- unnecessary recap of deprecated ideas

## Naming discipline

Naming rules are mandatory and are designed to reduce drift across agents.

### Canon terms to preserve exactly
- singleton
- mind-tribe
- mind-club
- memory-set
- upload
- ascension
- ghost
- human (functional shorthand, not species claim)

### Avoid sloppy substitutions unless explicitly defined
Do not casually substitute terms like:
- hive mind
- group mind
- soul upload
- AI god
- cyberghost
- baseline human

If used at all, define them as local/in-universe language rather than canon terminology.

### Name reuse
Do not reuse a proper noun for a different thing.

### Scope labels
When a statement is local, say so.
Example forms:
- "On some worlds..."
- "In many high-tech societies..."
- "This world treats..."
- "Galaxy-wide, no single rule applies..."

## Canon file style

Canon files should describe what is true now.
They should not contain process chatter.

## Artifact style

Artifact files should say:
- what they are for
- what they are not for
- that they are not canonical authority sources

## TODO references

When a file has unresolved questions, link to the global TODO rather than embedding large local task lists.
