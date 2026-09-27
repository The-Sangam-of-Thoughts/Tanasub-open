# Claude Code adapter

## Install

Create `CLAUDE.md` at the project root or copy the block below into your existing configuration. Claude Code checks instructions in hierarchical order:
1. User settings: `~/.claude/CLAUDE.md`
2. Project settings: `<project-root>/CLAUDE.md`
3. Local overrides: `<project-root>/.claude.local.md`

```markdown
For writing tasks, read `SKILL.md` and follow its router. Load one matching Layer 0 file, then only task-relevant optional layers and one applicable genre or subgenre file. Open deeper references only to resolve a concrete need. Do not load the whole repository. Keep context minimal without dropping required constraints.
```

## Use

Run `claude` in the repository root or invoke `/init` to generate project context. Claude Code automatically ingests `CLAUDE.md` upon launch and applies the routing instructions to writing requests.
