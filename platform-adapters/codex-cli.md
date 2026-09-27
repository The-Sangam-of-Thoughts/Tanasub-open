# OpenAI Codex CLI adapter

## Install

Place `AGENTS.md` at the project root or configure global instructions at `~/.codex/AGENTS.md`. Codex CLI supports nested per-directory `AGENTS.md` files for scoped instructions. You can run `/init` to initialize project guidelines.

```markdown
For writing tasks, read `SKILL.md` and follow its router. Load one matching Layer 0 file, then only task-relevant optional layers and one applicable genre or subgenre file. Open deeper references only to resolve a concrete need. Do not load the whole repository. Preserve user facts and keep automated QA separate from final acceptance.
```

## Use

Run `codex` from the repository root. Codex CLI automatically detects root and directory-scoped `AGENTS.md` files to route writing tasks according to `SKILL.md`.
