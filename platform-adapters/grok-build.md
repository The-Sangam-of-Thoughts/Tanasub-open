# Grok Build adapter

## Install

Place `AGENTS.md` at the project root. Grok Build reads `AGENTS.md` natively and remains compatible with `.claude/` conventions. To configure optional MCP servers or custom tools, add `.grok/config.toml`.

```markdown
For writing tasks, read `SKILL.md` and follow its router. Load one matching Layer 0 file, then only task-relevant optional layers and one applicable genre or subgenre file. Open deeper references only to resolve a concrete need. Do not load the whole repository. Maintain voice and craft rules without hard token loss.
```

## Use

Invoke Grok Build in the workspace. The adapter is fully compatible with Grok Build's Plan Mode and Build Mode: Plan Mode maps the pipeline (`SKILL.md` routing), and Build Mode executes drafting, voice passes, and Layer 3 QA.
