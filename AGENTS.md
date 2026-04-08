# AGENTS.md

## Purpose
This file tells repository-oriented agents how to work in this lore-bible repository.
It is procedural only. It is **not** a canon source.

## Read first
Before making changes, agents should read these files in this order:
1. `README.md`
2. `INDEX.md`
3. `CANON_RULES.md`
4. `STYLE_GUIDE.md`
5. `90_process/TODO.md`

For lore facts, then read only the canon files relevant to the task.
Do **not** load unrelated files unless needed.

## Authority order
When sources disagree, use this order:
1. Most recent explicit statements from the user on the relevant topic
2. Earlier explicit statements from the user on the relevant topic
3. Assistant-generated extrapolations the user explicitly endorsed
4. `deepfuture.pdf`
5. All other assistant speculation

If authority is clear, resolve automatically.
If authority is genuinely ambiguous, do **not** guess.
Ask the user and state:
- the exact ambiguity,
- which sources are in tension,
- what each source implies,
- and what decision depends on the answer.

If the ambiguity is local and non-blocking, continue the rest of the task while clearly bracketing the unresolved part.
If it is foundational or blocking, stop the affected change and ask first.

## Canon editing rules
If the agent can open a Git PR:
- it may edit canon files directly,
- but changes must remain reviewable and minimal.

If the agent cannot open a Git PR:
- it must write proposed canon changes to a staging area,
- and must not directly overwrite canon files.

Never preserve superseded ideas inside canon files just because they existed before.
Old versions belong in git history, not in the lore bible.

## Canon vs non-canon
Treat these classes distinctly:
- **Canon**: current authoritative lore
- **Ontology**: conceptual structure and controlled vocabulary that shape canon interpretation
- **Non-canon artifacts**: reports, test outputs, story scaffolds, staging drafts, exports

Do **not** mix non-canon artifacts into canon or ontology files.
Do **not** spend context on non-canon artifacts unless the task explicitly requires them.

## Naming discipline
Use the controlled vocabulary from the foundations and glossary files.
Do not casually invent near-synonyms for established terms.
If proposing a new ontology term or social form, treat it as a high-impact change.
Do not silently smuggle ontology changes in through prose.

## Scope discipline
Do not universalize a world-local pattern into a galaxy-wide truth.
Always preserve scope:
- galaxy
- world
- culture
- faction
- story-local

If the task concerns one world, avoid rewriting global files unless the change truly affects global canon.

## Earth rule
Do not introduce remembered Earth referents, prestige, geography, nations, religions, or continuity.
Earth ancestry may be objectively true in background ontology, but it is culturally nonexistent for practical narrative purposes.

## TODO behavior
Agents may:
- mark tasks complete,
- split tasks,
- create tasks,
- create subtasks,
- and update task status.

Use the global `90_process/TODO.md` unless instructed otherwise.
Keep tasks concrete, scoped, and machine-actionable.

## Acceptable agent outputs
Allowed outputs include:
- canon edits,
- staging drafts,
- consistency reports,
- contradiction reports,
- benchmark/test outputs,
- clearly marked story-development scaffolds,
- export artifacts.

Default to the smallest output that accomplishes the task.

## Preferred work pattern
1. Read governing files.
2. Read only relevant lore files.
3. Check for authority conflicts.
4. Decide whether the task affects canon, ontology, or non-canon artifacts.
5. Make the smallest coherent change.
6. Update `90_process/TODO.md` if appropriate.
7. If ambiguity remains, ask the user crisply.

## Do not
- Do not treat this file as canon.
- Do not revive dropped ideas from old chats just because they appear in historical materials.
- Do not browse non-canon artifacts unless needed.
- Do not expand ontology casually.
- Do not overwrite broad canon to solve a local story problem.
