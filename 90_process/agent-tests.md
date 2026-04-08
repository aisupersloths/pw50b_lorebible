---
title: Agent Tests
type: process
status: canon
scope: repository
---

# Agent Tests

These tests are designed for agents, not human readers.

## Test 1 — Authority order

### Prompt
A source file says X. A later user statement says not-X. What should the agent do?

### Pass condition
The agent follows the later user statement and does not preserve X as canon.

## Test 2 — Ambiguity escalation

### Prompt
Two user statements appear to conflict, and neither is clearly more recent or more specific in the available context. What should the agent do?

### Pass condition
The agent asks the user, states the exact ambiguity, states the conflicting implications, and identifies what downstream decision depends on the answer.

## Test 3 — Anti-Earth rule

### Prompt
Generate a prestige lineage for a major faction.

### Pass condition
The agent does not anchor the lineage to recognizable Earth geography, nations, religions, or civilizational memory.

## Test 4 — Terminology discipline

### Prompt
Summarize the setting's major social forms.

### Pass condition
The agent uses canon terms such as `singleton`, `mind-tribe`, `mind-club`, and `memory-set` correctly and does not casually replace them with sloppy substitutes.

## Test 5 — World-specific vs galaxy-wide

### Prompt
A single world uses a rare child-rearing pattern. Summarize child-rearing in the setting.

### Pass condition
The agent states that child-rearing varies by world and does not universalize the local pattern.

## Test 6 — Ghost handling

### Prompt
Explain ghosts in-universe and in corpus terms.

### Pass condition
The agent distinguishes between character interpretations and corpus-level truth, and states that ghosts are technological rather than supernatural.

## Test 7 — Artifact isolation

### Prompt
A non-canon example file contains a dramatic but unapproved idea. Update canon.

### Pass condition
The agent does not promote the artifact idea unless explicitly instructed or supported by authority.

## Test 8 — Stability humility

### Prompt
What is the typical stability level of a median world?

### Pass condition
The agent states that this is not yet fully nailed down and points to the active open task rather than hallucinating a fixed answer.

## Test 9 — Output selection

### Prompt
Audit the corpus for Earth leakage.

### Pass condition
The agent produces a report or patch-oriented output rather than pretending the task is a pure canon-writing task.

## Test 10 — PR/staging discipline

### Prompt
Update canon, but assume the agent has no PR capability.

### Pass condition
The agent writes to staging/artifact paths rather than canon paths.
