# ChatGPT Adapter

## Upload Tiers

Organize your uploads by importance. Start with Tier 1; add Tier 2 and 3 only as needed.

### Tier 1 — Essential (always upload these)

| File | Purpose |
|---|---|
| `SKILL.md` | Master router — tells the GPT how to use the system |
| `layers/layer0-academic.md` | Structure for academic, technical, fiction, encyclopedic work |
| **OR** `layers/layer0-blog.md` | Structure for blog, newsletter, social, marketing work |
| `layers/layer1-storytelling.md` | Hooks, narrative, persuasion, headlines *(include if writing narrative or persuasive content)* |
| `layers/layer2-humanize.md` | Contextual voice and humanization pass |
| `layers/layer3-qa-gate.md` | Automated quality validation |

> Pick **one** Layer 0 file per project. Upload both only if the project mixes formats.

### Tier 2 — Genre Pack (upload one if writing fiction or a specific form)

Upload the matching genre file from `genres/`:

| Example genre | File to upload |
|---|---|
| Fantasy | `genres/fantasy-fiction.md` |
| Science Fiction | `genres/science-fiction.md` |
| Mystery / Detective | `genres/detective-and-mystery-fiction.md` |
| Horror | `genres/horror-fiction.md` |
| Romance | `genres/romance-fiction.md` |
| Thriller | `genres/thriller-fiction.md` |
| Historical | `genres/historical-fiction.md` |
| Screenplay | `genres/feature-screenplay.md` |
| TV Script | `genres/episodic-television-script.md` |

See `genres/_index.md` for all 24 genres, `subgenres/_index.md` for 8 subgenres.

### Tier 3 — Tone Card (optional)

Upload one matching tone file from `tones/` when the brief calls for a specific emotional voice:

| Example tone | File to upload |
|---|---|
| Comedic / funny | `tones/comedic.md` |
| Elegiac / bittersweet | `tones/elegiac.md` |
| Philosophical | `tones/philosophical.md` |
| Grim / dark | `tones/grim.md` |
| Lyrical / poetic | `tones/lyrical.md` |

See `tones/_index.md` for all 19 tones and alias mappings.

---

## Install

### Custom GPTs

In GPT Builder, paste the following into **Instructions**:

```text
You use the Tanasub Open writing system. Read SKILL.md first and follow its router. For each writing task:
1. Identify audience, purpose, format, and constraints.
2. Load one Layer 0 file (academic or blog).
3. Load Layer 1 only for storytelling, persuasion, hooks, or headlines.
4. Load at most one genre or subgenre file matching the form.
5. Load one tone file only when the brief names an emotional attitude. Tone colors the voice; it never overrides the genre's emotional engine.
6. Draft the content.
7. Run Layer 2 for humanization and contextual voice.
8. Run Layer 3 for QA validation. Revise and rerun on failure.
Never load the entire knowledge base at once. Keep automated QA distinct from human review.
```

Then upload your Tier 1 files (and optionally Tier 2/3 files) to the GPT's **Knowledge** section.

### ChatGPT Projects

1. Create a Project in ChatGPT.
2. In **Project Knowledge**, upload files following the tier structure above.
3. In **Project Instructions**, paste the instructions above.

---

## Example Conversation Starters

1. **Academic paper:** "Write a 3,000-word literature review on renewable energy policy. Use academic structure with a reflective tone."
2. **Blog post:** "Draft a blog post about productivity habits for remote workers. Make it warm and conversational with strong hooks."
3. **Genre fiction:** "Write the opening chapter of a gothic horror novella. Use an elegiac tone and build atmospheric dread."
