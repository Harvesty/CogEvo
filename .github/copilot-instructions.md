# Copilot / AI agent instructions — CogEvo

Purpose
- Help AI coding agents be immediately productive in this repository: document the repo's intent, key directories, editing conventions, and PR/commit expectations.

Big picture (short)
- This repo is a documentation-first personal lab for cognitive design (see root README). Primary content are markdown files. Most work is content authoring and small structural edits, not compile-run engineering.

Where to look (examples)
- Overview and structure: `README.md` (root).
- Philosophy patterns and contributor guidance: `Philosophy/Philosophy - Copilot.md` and `Philosophy/README.md`.
- Flashcards / translations: `Book/Thinking-Fast-Slow/Flashcard-EN.md` and `Flashcard-CN.md`.

Conventions & patterns
- Directory roles: `Prototypes/` = active experiments; `Sandbox/` = exploratory notes; `Archives/` = stable snapshots; `Context-Kits/` = scenario toolkits.
- Metadata files: add a `metadata.md` alongside new items (recommended fields: `title`, `philosophy_tags`, `status` (prototype|stable|archive), `date`, `author`).
- Tagging: use short topic tags in filenames or front-matter, e.g. `#phenomenology`, `#bayesian`, `#ethics` — these are referenced in READMEs.
- Localization: preserve original-language content. Add translations as separate files with suffix `-EN` or `-CN` rather than editing originals in-place.

Editing rules for AI agents (do this)
- Preserve tone and original Chinese passages; when adding translations, create parallel `*-EN.md` files.
- Make small, focused PRs: one logical change per PR and include a `CHANGELOG.md` entry if the change affects practices.
- When modifying structure, do not rename top-level folders without discussion — prefer adding a new folder and migrating gradually.

PR / commit message guidance
- Commit title: concise imperative + scope, e.g. `docs(Philosophy): add metadata for Hexagon case study`.
- PR description: include `关联哲学维度` or `philosophy_tags` line (e.g. `关联哲学维度: #ethics, #phenomenology`) and note affected files.

What AI should not do
- Don't bulk-rewrite long personal notes; prefer targeted improvements or additions.
- Don't assume a build/test pipeline exists; this repo is content-first (no CI scripts detected).

Quick examples
- To add a prototype: create `Prototypes/<slug>/README.md` + `Prototypes/<slug>/metadata.md` and add one-sentence summary to `Prototypes/README.md`.
- To add a translation: copy `Philosophy/SomeTopic.md` → `Philosophy/SomeTopic-EN.md` and keep a `lang:` front-matter line.

If uncertain
- Open a short PR and mark it `draft` requesting human review; include a short explanation of the change and any assumptions.

Last step
- Ask maintainers for a glossing pass on sensitive or personal notes before large stylistic edits.

— end —

