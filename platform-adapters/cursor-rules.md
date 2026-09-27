# Cursor Project Rule adapter

## Install

Create `.cursor/rules/universal-writing-guide.mdc` in the target project and copy the block below into it. Cursor requires the `.mdc` extension for Project Rules and can apply a rule intelligently from its description. See [Cursor Rules](https://prod.cursor.com/docs/rules). Root `.cursorrules` is legacy and deprecated.

```mdc
---
description: Use the universal writing guide when planning, drafting, revising, humanizing, or reviewing prose, articles, creative work, social copy, or marketing copy.
alwaysApply: false
---
For writing work, read `SKILL.md` and follow its router. Load one matching Layer 0 file, then only task-relevant optional layers and one applicable genre or subgenre file. Read a reference only to resolve a concrete need. Do not load the whole repository. Treat token use as an optimization signal and use no hard token cap that removes necessary context. Keep automated QA distinct from human or platform acceptance.
```
