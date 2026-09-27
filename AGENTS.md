# Tanasub Open — Repository Agent Instructions

Tanasub Open is the public, independently usable foundation of the Tanasub writing system. Preserve `universal-writing-guide` where it acts as an existing skill or platform compatibility identifier. This repository is self-contained: never imply that an external, hosted, or proprietary service is available.

## Repo Map

```
SKILL.md            → Start here. Master router and lookup tables.
layers/             → 5 pipeline stages (structure, story, humanize, QA)
genres/             → 24 genre craft files. See genres/_index.md
subgenres/          → 8 subgenre craft files. See subgenres/_index.md
tones/              → 19 tone cards. See tones/_index.md
core/               → Methodology, templates, schemas
references/         → Evidence dossiers, style catalogs
external/           → Vendored humanization patterns
platform-adapters/  → Config for 12 AI platforms
```

## Fast-Path

Already have genre + tone confirmed? Load these files in order:

1. `layers/layer0-academic.md` (fiction, academic, technical) **or** `layers/layer0-blog.md` (blog, newsletter, marketing)
2. `genres/{genre}.md` or `subgenres/{subgenre}.md` — one craft file matching the form
3. `tones/{tone}.md` — only if a tone was specified in the brief
4. Draft your content
5. `layers/layer2-humanize.md` — contextual voice and humanization pass
6. `layers/layer3-qa-gate.md` — automated validation

## Full Router

For tasks where the genre or tone still needs to be discovered, follow this complete routing sequence:

1. Load exactly one matching Layer 0 file (`layers/layer0-academic.md` or `layers/layer0-blog.md`).
2. Load `layers/layer1-storytelling.md` only when narrative, persuasion, hooks, or headlines are needed.
3. Load at most one applicable genre or subgenre file from `genres/` or `subgenres/`. Use `genres/_index.md` or `subgenres/_index.md` to choose.
4. Load one file from `tones/` only when the brief names an emotional attitude (for example philosophical, comedic, elegiac). Tone colors the voice; it never overrides the genre's emotional engine. Use `tones/_index.md` to choose.
5. Draft or revise the content.
6. Run `layers/layer2-humanize.md` for contextual voice and humanization pass.
7. Run `layers/layer3-qa-gate.md` for automated validation.
8. Open deeper references only to resolve a concrete need. Do not load the entire repository.
