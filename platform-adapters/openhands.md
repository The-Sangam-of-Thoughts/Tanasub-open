# OpenHands adapter

## Install

Create `.openhands/microagents/repo_instructions.md` at repository root, or use `/add-skill` in the OpenHands web UI to load it.

```markdown
---
name: universal-writing-guide
type: repo
---
For writing tasks, read `SKILL.md` and follow its router. Load one matching Layer 0 file, then only task-relevant optional layers and one applicable genre or subgenre file. Open deeper references only to resolve a concrete need. Do not load the whole repository. Run Layer 3 for automated QA.
```

## Use

Start an OpenHands session in the workspace. OpenHands automatically mounts repository microagents, routing any writing or documentation task through `SKILL.md`.
