---
title: Peacewrench50B Lore Bible
type: root
status: canon
scope: repository
---

# Peacewrench50B Lore Bible

This repository is the portable, platform-agnostic source of truth for the Deep Future setting.

## Purpose

This corpus is designed to be usable by:
- ChatGPT
- Claude / Opus
- Grok
- future coding agents
- future generator/export tools such as Perchance

The source of truth is Markdown in git.

## Core operating rule

Portable corpus first, platform wrappers second.

Canon must not live only in:
- chat history
- project instructions
- hidden system prompts
- artifacts/canvases
- Perchance generators

Those may consume or stage material, but this corpus is authoritative.

## Canon model

This repository stores only:
- current canon
- current ontology
- current governance/process rules
- current open questions and tasks
- clearly separated non-canon artifacts when useful

Superseded material is removed or overwritten rather than preserved in the lore bible. Git history is the archive.

## Content classes

- `00_foundations/` — premise, themes, cosmology, ontology, canon boundaries, glossary
- `10_systems/` — memory sharing, ghosts, uploading, economics, law, stability
- `20_societies/` — world-design rules and future chosen societies
- `80_examples/` — clearly marked non-canon scaffolding/examples
- `90_process/` — TODOs, agent tests, process artifacts
- `platform/` — thin adapter files for specific LLM platforms
- `exports/` — derived machine-consumption layers such as Perchance exports

## Source authority order

Unless explicitly overridden by the user:
1. most recent explicit statements from the user on the relevant topic
2. earlier explicit statements from the user
3. assistant-generated extrapolations explicitly endorsed by the user
4. `deepfuture.pdf`
5. all other assistant speculation

## Ambiguity rule

If authority is genuinely ambiguous, agents must not guess.
They must ask the user and state:
- the exact ambiguity
- the sources in tension
- what each implies
- what decision depends on the answer

## Current setting summary

This is an ultra-deep-future setting in the merged Milky Way–Andromeda galaxy, long after all other galaxies have fallen beyond the light cone. Memory-sharing, copying, branching, and merging are foundational technologies. Uploading, near-immortality, and superintelligence exist, but human-scale embodied minds still persist because they remain economically, epistemically, and operationally useful in a galaxy of differentiated niches and long historical cycles. Economically useful specialist sentiences are often derived from copied, edited, archived, or otherwise reconfigured minds rather than built solely as machine learning models or conventional software.

## Start here

- `INDEX.md`
- `CANON_RULES.md`
- `STYLE_GUIDE.md`
- `90_process/TODO.md`
- `90_process/agent-tests.md`
