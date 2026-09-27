# Tanasub Open — AI writing craft library

[![Repository integrity](https://github.com/The-Sangam-of-Thoughts/Tanasub-open/actions/workflows/repository-integrity.yml/badge.svg?branch=master)](https://github.com/The-Sangam-of-Thoughts/Tanasub-open/actions/workflows/repository-integrity.yml)
[![License: MIT + CC BY-SA 4.0](https://img.shields.io/badge/license-MIT%20%2B%20CC%20BY--SA%204.0-blue)](LICENSES/README.md)

**Plan, draft, and revise AI-assisted writing with guidance for structure, storytelling, voice, and editorial review.** Tanasub Open is a self-contained Markdown craft library for writers and AI agents, with 24 genre files, 8 subgenre files, and 19 optional tone cards.

Use it for fiction, screenplays, poetry, academic writing, technical documentation, blogs, and marketing copy. Load the guidance your task needs, then work through a draft and review pass. There is no application to install; bring your own chatbot or agent. No Tanasub account or hosted service is required.

[Start writing](QUICKSTART.md) · [Browse genres](genres/_index.md) · [Choose a tone](tones/_index.md) · [Platform setup](platform-adapters/_index.md) · [Contribute](CONTRIBUTING.md)

## Try it with your next draft

### In a chatbot

For a quick trial, copy the prompt block from the [generic system prompt](platform-adapters/generic-system-prompt.md) into your conversation, followed by your writing brief. For the full workflow, attach [`SKILL.md`](SKILL.md) and the files listed in the [Quick Start Guide](QUICKSTART.md). A chatbot can use only files you provide or make accessible through its tools.

For example, attach `SKILL.md`, `layers/layer0-academic.md`, `genres/fantasy-fiction.md`, `tones/elegiac.md`, `layers/layer2-humanize.md`, and `layers/layer3-qa-gate.md`, then ask:

```text
Use the attached Tanasub Open files and follow SKILL.md.
Draft a 600-word fantasy opening in an elegiac tone.
An aging cartographer discovers that a village on her map has vanished.
Build the scene around a choice she must make, with restrained worldbuilding.
Revise for voice, then report the QA findings and unresolved weaknesses.
```

This is an example brief, not a benchmark or a guarantee of output quality.

### In an AI agent

Clone the library into a directory your agent can read:

```sh
git clone https://github.com/The-Sangam-of-Thoughts/Tanasub-open.git
cd Tanasub-open
```

Tell the agent: **“Read SKILL.md first and follow its router for this writing task.”** Use the [platform adapter](platform-adapters/_index.md) for your tool to configure persistent instructions. File discovery and access depend on the tool and workspace configuration.

The stable skill identifier is `universal-writing-guide`; keep it when configuring existing integrations.

## What the library provides

| Need | Start here |
|---|---|
| Structure for academic, technical, or fiction work | [Academic structure](layers/layer0-academic.md) |
| Structure for blogs, newsletters, or marketing | [Blog structure](layers/layer0-blog.md) |
| Hooks, narrative momentum, or persuasion | [Storytelling](layers/layer1-storytelling.md) |
| Form-specific craft, from mystery to ghazal | [24 genres](genres/_index.md) and [8 subgenres](subgenres/_index.md) |
| A requested emotional attitude | [19 tones](tones/_index.md) and [combination rules](tones/_combination-rules.md) |
| Contextual voice and revision | [Humanization](layers/layer2-humanize.md) |
| Evidence, accessibility, and completion checks | [Editorial QA gate](layers/layer3-qa-gate.md) |

The genre collection includes Urdu and South Asian forms such as dastan, ghazal, katha, nataka, prakarana, and vachana, alongside contemporary fiction and screenwriting. Tone colors the voice; it does not replace the genre's emotional engine.

### A small workflow, with deeper guidance on demand

1. **Structure:** load exactly one Layer 0 file for the writing task.
2. **Craft:** add storytelling when needed, at most one genre or subgenre, and one tone only when requested.
3. **Draft and revise:** write the piece, then apply the contextual humanization pass.
4. **Review:** use the QA gate to record findings and repair weaknesses.

The router keeps unrelated files out of the working context. Actual context use depends on the selected files and model tokenizer; deeper genre and evidence files can be substantial.

The QA gate is a written review rubric, not executable validation or proof of factual accuracy. The GitHub integrity badge checks repository file types and Git modes, not writing quality. Humanization supports deliberate voice; it is not an authorship detector or a promise to evade detection. Verify sources and consequential claims yourself.

## Find your way around

| Path | Contents |
|---|---|
| [`SKILL.md`](SKILL.md) | Master router and lookup tables |
| [`layers/`](layers/) | Structure, storytelling, humanization, and QA guidance |
| [`genres/`](genres/) / [`subgenres/`](subgenres/) | Craft guidance by form |
| [`tones/`](tones/) | Optional voice-attitude cards and precedence rules |
| [`core/`](core/) | Methodology, editorial templates, and schemas |
| [`references/`](references/) | Evidence dossiers, indexes, and style catalogs |
| [`platform-adapters/`](platform-adapters/) | Setup guides for agents and chatbots |
| [`external/`](external/) | Vendored patterns and acquisition notes; see each upstream notice |

Setup guides cover ChatGPT, Claude Chat, Claude Code, Cursor, GitHub Copilot, Codex CLI, Aider, Antigravity, Grok Build, OpenCode, OpenHands, and Z.ai, plus a generic system prompt. These are configuration guides, not certification of every platform or model version.

For development context, see the [roadmap](docs/roadmap.md), [coverage ledger](docs/topic-coverage-gaps.csv), and [architecture decisions](docs/decisions/). Historical status records are not a substitute for reviewing the current content and its evidence.

## Help improve the library

Read the [contributor guide](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md). Useful first contributions include broken-link fixes, clearer setup steps, and sourced corrections to craft guidance.

- [Report a problem or ask a setup question](https://github.com/The-Sangam-of-Thoughts/Tanasub-open/issues/new/choose). Include the file, your goal, and what went wrong.
- [Suggest an improvement](https://github.com/The-Sangam-of-Thoughts/Tanasub-open/issues/new?template=improvement.md). Explain the writer's need and provide sources for substantive claims.
- [Read the security policy](.github/SECURITY.md) before reporting a vulnerability privately.

If the library helps your writing, star the repository to save it, or share a reproducible example through an issue. Do not include private drafts, credentials, or personal data.

## License and name

Project-authored material is [MIT-licensed](LICENSE) unless otherwise marked. Four humanization adaptation files are **CC BY-SA 4.0**; vendored material retains its upstream terms. Read the [license mapping](LICENSES/README.md) and [licensing scope](docs/licensing-scope.md) before redistribution. Bibliographic records do not grant rights to reproduce the works they describe.

**Tanasub** (approximately *tuh-NAA-sub*, تناسب) evokes proportion, harmony, and meaningful correspondence. The [brand foundation](docs/brand/tanasub-brand-foundation.md) explains the name and positioning.
