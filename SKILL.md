---
name: universal-writing-guide
description: Tanasub Open plans, drafts, improves, humanizes, and reviews academic, technical, creative, blog, social, and marketing writing with task-specific genre guidance.
---

# Tanasub Open

## Quick-Dispatch

If you already know your form, genre, and tone, go directly to the file paths below. No need to read the rest.

### Form → Layer 0

| Writing form | Load this file |
|---|---|
| Academic, scientific, technical, encyclopedic, schema-bound, fiction | `layers/layer0-academic.md` |
| Blog, newsletter, social, marketing, landing-page, product copy | `layers/layer0-blog.md` |

### Genre Lookup

| Genre | File |
|---|---|
| Dastan Tradition | `genres/dastan-tradition.md` |
| Detective and Mystery Fiction | `genres/detective-and-mystery-fiction.md` |
| Episodic Television Script | `genres/episodic-television-script.md` |
| Epistolary Fiction | `genres/epistolary-fiction.md` |
| Fantasy Fiction | `genres/fantasy-fiction.md` |
| Feature Screenplay | `genres/feature-screenplay.md` |
| Flash Fiction | `genres/flash-fiction.md` |
| Frame Narrative | `genres/frame-narrative.md` |
| Ghazal Sequence | `genres/ghazal-sequence.md` |
| Gothic Fiction | `genres/gothic-fiction.md` |
| Historical Fiction | `genres/historical-fiction.md` |
| Horror Fiction | `genres/horror-fiction.md` |
| Interactive Fiction | `genres/interactive-fiction.md` |
| Katha Tradition | `genres/katha-tradition.md` |
| Nataka Drama | `genres/nataka-drama.md` |
| Pastoral Literature | `genres/pastoral-literature.md` |
| Picaresque Literature | `genres/picaresque-literature.md` |
| Prakarana Drama | `genres/prakarana-drama.md` |
| Romance Fiction | `genres/romance-fiction.md` |
| Satirical Literature | `genres/satirical-literature.md` |
| Science Fiction | `genres/science-fiction.md` |
| Speculative Fiction | `genres/speculative-fiction.md` |
| Thriller Fiction | `genres/thriller-fiction.md` |
| Vachana Poetry | `genres/vachana-poetry.md` |

### Subgenre Lookup

| Subgenre | File |
|---|---|
| Bildungsroman | `subgenres/bildungsroman.md` |
| Cozy Mystery | `subgenres/cozy-mystery.md` |
| Cyberpunk | `subgenres/cyberpunk.md` |
| Psychological Fiction | `subgenres/psychological-fiction.md` |
| Psychological Thriller | `subgenres/psychological-thriller.md` |
| Solarpunk | `subgenres/solarpunk.md` |
| Space Opera | `subgenres/space-opera.md` |
| Urban Fantasy | `subgenres/urban-fantasy.md` |

### Tone Lookup

| Tone | Aliases | File |
|---|---|---|
| Comedic | funny, humorous, witty, gallows humor | `tones/comedic.md` |
| Deadpan | dry, tongue-in-cheek, wry | `tones/deadpan.md` |
| Whimsical | playful, fanciful, quirky | `tones/whimsical.md` |
| Irreverent | cheeky, impious, anti-pompous | `tones/irreverent.md` |
| Philosophical | contemplative, ideas-first, dialectical | `tones/philosophical.md` |
| Reflective | introspective, journal-like, pensive, serene, meditative | `tones/reflective.md` |
| Elegiac | mournful, lamenting, bittersweet, sad | `tones/elegiac.md` |
| Nostalgic | wistful, sepia-toned, reminiscent | `tones/nostalgic.md` |
| Inspirational | motivational, uplifting, hopeful, inspiring | `tones/inspirational.md` |
| Lyrical | poetic, musical, cadenced, beautiful prose | `tones/lyrical.md` |
| Reverent | devotional, solemn-awe, hushed, solemn | `tones/reverent.md` |
| Warm | friendly, breezy, companionable, earnest, sincere | `tones/warm.md` |
| Grim | bleak, somber, unflinching, dark mood | `tones/grim.md` |
| Cynical | sardonic, jaded, disillusioned, sarcastic | `tones/cynical.md` |
| Urgent | pressing, insistent, time-bound | `tones/urgent.md` |
| Defiant | resistant, protest-voiced, unbowed | `tones/defiant.md` |
| Intimate | confessional, vulnerable, close | `tones/intimate.md` |
| Detached | clinical, matter-of-fact, neutral | `tones/detached.md` |
| Compassionate | empathetic, consoling, tender | `tones/compassionate.md` |

---

## Pipeline

Load files in this exact order:

1. **Layer 0** — Structure: `layers/layer0-academic.md` or `layers/layer0-blog.md`
2. **Layer 1** — Storytelling *(only if piece needs hooks, narrative, persuasion, or headlines)*: `layers/layer1-storytelling.md`
3. **Genre/Subgenre** — Craft file *(only if the form requires it)*: one file from `genres/` or `subgenres/`
4. **Tone** — Voice modifier *(only if brief names an emotional attitude)*: one file from `tones/`
5. **Draft** your content
6. **Layer 2** — Humanize: `layers/layer2-humanize.md`
7. **Layer 3** — QA Gate: `layers/layer3-qa-gate.md`

> **Token Budget:** Worst-case pipeline (Layer 0 + Layer 1 + genre + tone + Layer 2 + Layer 3) is approximately **~8K tokens**. Most tasks load fewer files.

---

Tanasub (approximately *tuh-NAA-sub*) is a writing system built around proportion, harmony, and meaningful connections. This repository is its open foundation. The frontmatter identifier `universal-writing-guide` is retained for compatibility with existing skill installations.

Tanasub Open must remain independently useful: everything this skill documents runs locally from files in this repository. It must not require private source files, a hosted account, a network connection, or any external service to complete its documented local workflow.

Use the smallest set of files that fully serves the request. Do not load the whole repository.

## Route the task

1. Read the request and identify audience, purpose, format, evidence needs, voice, length, and constraints.
2. Load one structural layer:
   - Academic, scientific, technical, encyclopedic, or schema-bound work: `layers/layer0-academic.md`
   - Blog, newsletter, social, marketing, landing-page, or product work: `layers/layer0-blog.md`
3. Load `layers/layer1-storytelling.md` when the piece needs an opening, narrative progression, tension, persuasion, memorability, or headline work. Skip it for tasks where those features would distract.
4. Load one file from `genres/` or `subgenres/` only when the requested form needs it. Use `genres/_index.md` or `subgenres/_index.md` to choose. Do not treat a listed gap as instruction.
5. Load one file from `tones/` only when the brief names an emotional attitude (for example philosophical, comedic, elegiac). Tone colors the voice; it never overrides the genre's emotional engine. Use `tones/_index.md` to choose.
6. Draft or revise.
7. Load `layers/layer2-humanize.md` for the contextual voice pass.
8. Run `layers/layer3-qa-gate.md`. Return only to the phase named by each failure.

## Working rules

- Preserve the user's facts, intent, supplied wording, quotations, assets, dialect, and required terminology.
- Never invent evidence, citations, experience, audience research, review, or approval.
- Match evidence effort to the claim and format. A casual caption may need no citation; a scientific claim does.
- Keep cultural and regional scope explicit. Do not present one tradition as universal.
- Prefer concrete mechanisms, examples, consequences, and actions over generic importance or praise.
- Humanization uses reflection, not banned words. Any word may remain when it is precise and fits the register.
- Treat named storytelling frameworks as optional tools. Pick one useful structure rather than stacking formulas.
- Record uncertainty when it affects correctness. Do not hide a failed check with smoother prose.

## Progressive disclosure

Load deeper material only to resolve a real need. Open the named file that answers the question; never load a directory wholesale:

- Evidence method or scoring detail: the relevant file in `core/methodology/`, usually `source-policy.md`, `report-style-guide.md`, or `quality-rubric.md`.
- A reusable document structure: one matching file in `core/templates/editorial/` or `core/templates/research-records/`.
- Structured-data validation: one schema in `core/schemas/v1/`.
- Storytelling rationale: `references/storytelling-dossier-full.md`.
- Humanization rationale or pattern lookup: `references/humanization-guide-full.md`, `references/structural-tells-catalog.md`, or `references/word-awareness-index.md`.
- A cited craft record: the specific ID under `references/evidence/claims/`, `sources/`, or `primary-works/`.
- Incomplete genre topics: filter `docs/topic-coverage-gaps.csv` for the chosen axis.
- Roadmap and decisions: `docs/roadmap.md`.
- Historical material: use `archive/` only when the request explicitly requires project history.

Minimize token use by summarizing the brief once, loading one variant at a time, and keeping optional files out of context. Token counts are optimization signals, not hard caps; retain necessary detail for correctness, accessibility, and quality.

## Quick examples

1. Academic paper: load layer0-academic → draft → layer2-humanize → layer3-qa-gate
2. Blog post: load layer0-blog + layer1-storytelling → draft → layer2-humanize → layer3-qa-gate
3. Genre fiction: load layer0-academic + genres/[genre].md → draft → layer2-humanize → layer3-qa-gate
4. Fiction with a deadpan tone: load layer0-academic + genre + tone → draft → layer2-humanize → layer3-qa-gate

## Completion

Deliver the requested artifact plus only the explanation the user needs. If the applicable QA gate fails, revise and rerun it. Keep automated checks separate from independent review or human sign-off.
