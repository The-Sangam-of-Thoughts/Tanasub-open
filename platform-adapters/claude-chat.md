# Claude Chat Adapter

Instructions for using Tanasub Open with Claude.ai conversations and Claude Projects.

> **Note:** Claude has a large context window, so uploading more files at once is fine. Don't worry about token budgets as much as with other platforms.

## Upload Tiers

### Tier 1 — Essential (always upload these)

| File | Purpose |
|---|---|
| `SKILL.md` | Master router — tells Claude how to use the system |
| `layers/layer0-academic.md` | Structure for academic, technical, fiction, encyclopedic work |
| **OR** `layers/layer0-blog.md` | Structure for blog, newsletter, social, marketing work |
| `layers/layer1-storytelling.md` | Hooks, narrative, persuasion, headlines *(include if writing narrative or persuasive content)* |
| `layers/layer2-humanize.md` | Contextual voice and humanization pass |
| `layers/layer3-qa-gate.md` | Automated quality validation |

### Tier 2 — Genre Pack (upload one if writing fiction or a specific form)

Upload the matching genre file from `genres/`. See `genres/_index.md` for all 24 genres, `subgenres/_index.md` for 8 subgenres.

### Tier 3 — Tone Card (optional)

Upload one matching tone file from `tones/`. See `tones/_index.md` for all 19 tones and alias mappings.

---

## Claude Projects (Recommended)

1. Create a new Project in Claude.
2. In **Project Knowledge**, upload files following the tier structure above.
3. In **Project Instructions**, paste:

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

> Since Claude Projects persist knowledge across conversations, this setup works for ongoing writing projects.

---

## One-Off Conversations

For a single conversation without a Project:

1. Start a new conversation with Claude.
2. Upload the relevant files as attachments in your first message.
3. Include this instruction at the top of your message:

```text
I'm attaching files from the Tanasub Open writing system. Read SKILL.md first, then follow its pipeline: load the appropriate Layer 0 for structure, apply the genre and tone files if attached, draft the content, then run Layer 2 (humanize) and Layer 3 (QA gate).
```

4. Follow with your writing brief.

---

## Example Conversation Starters

1. **Academic paper:** "Write a 3,000-word literature review on renewable energy policy. Use academic structure with a reflective tone."
2. **Blog post:** "Draft a blog post about productivity habits for remote workers. Make it warm and conversational with strong hooks."
3. **Genre fiction:** "Write the opening chapter of a gothic horror novella. Use an elegiac tone and build atmospheric dread."
