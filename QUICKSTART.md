# Tanasub Open — Quick Start Guide

Get better writing from any AI chatbot in minutes. No technical knowledge required.

---

## What chatbot are you using?

```
┌─ ChatGPT (Custom GPTs or Projects) ─────→ See "Setup: ChatGPT" below
├─ Claude (claude.ai) ─────────────────→ See "Setup: Claude" below
├─ Claude Code / Cursor / Copilot ──────→ See platform-adapters/ folder
└─ Any other chatbot ──────────────────→ See "Setup: Any Chatbot" below
```

---

## What are you writing?

Use this table to pick which files to upload or paste:

| Writing type | Files to upload |
|---|---|
| **Academic paper, research, technical docs** | `layers/layer0-academic.md` + `layers/layer2-humanize.md` + `layers/layer3-qa-gate.md` |
| **Blog post, newsletter, marketing** | `layers/layer0-blog.md` + `layers/layer1-storytelling.md` + `layers/layer2-humanize.md` + `layers/layer3-qa-gate.md` |
| **Fiction (any genre)** | `layers/layer0-academic.md` + `genres/{your-genre}.md` + `layers/layer2-humanize.md` + `layers/layer3-qa-gate.md` |
| **Fiction with a specific tone** | Same as above + `tones/{your-tone}.md` |
| **Quick one-off (any chatbot)** | Just paste the system prompt from `platform-adapters/generic-system-prompt.md` |

> **Always upload `SKILL.md`** — it tells the AI how to use the other files.

---

## Setup: ChatGPT

### Using ChatGPT Projects (recommended)
1. Create a new **Project** in ChatGPT.
2. Open **Project Knowledge** and upload these files:
   - `SKILL.md`
   - The Layer 0 file matching your writing type (see table above)
   - `layers/layer1-storytelling.md` *(if writing blog/narrative content)*
   - `layers/layer2-humanize.md`
   - `layers/layer3-qa-gate.md`
   - *(Optional)* A genre file from `genres/` and/or a tone file from `tones/`
3. In **Project Instructions**, paste:
   > "You use the Tanasub Open writing system. Read SKILL.md first and follow its router."
4. Start chatting with your writing brief!

### Using Custom GPTs
1. Open **GPT Builder**.
2. Upload the same files to **Knowledge**.
3. Paste the instructions from `platform-adapters/chatgpt-custom-gpt.md` into **Instructions**.
4. Save and use your GPT.

---

## Setup: Claude

### Using Claude Projects (recommended)
1. Create a new **Project** in Claude.
2. Upload files to **Project Knowledge** (same file list as ChatGPT above).
3. In **Project Instructions**, paste:
   > "You use the Tanasub Open writing system. Read SKILL.md first and follow its router."
4. Start chatting!

> **Tip:** Claude has a large context window, so feel free to upload more files — the full genre file, tone file, and even `layers/layer1-storytelling.md` together.

### One-off conversation
1. Start a new Claude conversation.
2. Attach the relevant files to your first message.
3. Begin your message with:
   > "I'm attaching files from the Tanasub Open writing system. Read SKILL.md first, then follow its pipeline."
4. Follow with your writing brief.

---

## Setup: Any Chatbot

For Gemini, Copilot, Grok, Perplexity, local models, or any other AI:

1. Open the file `platform-adapters/generic-system-prompt.md`.
2. Copy the entire system prompt block.
3. Paste it at the very beginning of your first message to the chatbot.
4. Follow it with your writing brief.

> This gives you the core Tanasub methodology without needing file uploads. For even better results, also paste the contents of the relevant genre and tone files after the system prompt.

---

## Worked Examples

### Example 1: Academic Paper

**Goal:** Write a literature review on climate adaptation strategies.

**Files to upload:**
- `SKILL.md`
- `layers/layer0-academic.md`
- `layers/layer2-humanize.md`
- `layers/layer3-qa-gate.md`

**Prompt:** "Write a 3,000-word literature review on urban climate adaptation strategies. Focus on green infrastructure, policy frameworks, and community resilience. Use academic structure with proper evidence integration."

**What happens:** The AI uses Layer 0 for formal structure and evidence standards, drafts the review, humanizes the prose (Layer 2), and validates quality (Layer 3).

---

### Example 2: Blog Post

**Goal:** Write an engaging blog post about remote work productivity.

**Files to upload:**
- `SKILL.md`
- `layers/layer0-blog.md`
- `layers/layer1-storytelling.md`
- `layers/layer2-humanize.md`
- `layers/layer3-qa-gate.md`

**Prompt:** "Draft a 1,500-word blog post about productivity habits for remote workers. Make it warm and conversational with strong hooks and actionable tips."

**What happens:** Layer 0 provides blog structure, Layer 1 adds hooks and narrative engagement, the draft gets humanized (Layer 2), and validated (Layer 3).

---

### Example 3: Fantasy Novel Chapter with Elegiac Tone

**Goal:** Write the opening chapter of a fantasy novel with a melancholic, bittersweet mood.

**Files to upload:**
- `SKILL.md`
- `layers/layer0-academic.md` *(yes, fiction uses the academic layer for structural rigor)*
- `genres/fantasy-fiction.md`
- `tones/elegiac.md`
- `layers/layer2-humanize.md`
- `layers/layer3-qa-gate.md`

**Prompt:** "Write the opening chapter (3,000 words) of a fantasy novel. The protagonist is an aging cartographer who discovers that the lands he mapped are vanishing from reality. Use elegiac tone — bittersweet, mournful, with a sense of beautiful loss. Build the world through the character's memories and observations."

**What happens:** Layer 0 provides structural rigor, the fantasy genre file guides worldbuilding and magic systems, the elegiac tone card shapes the emotional voice, then Layer 2 and Layer 3 polish and validate.

---

## Finding the Right Files

- **Don't know which genre?** Open `genres/_index.md` — the Quick Match table maps common phrases to files.
- **Don't know which tone?** Open `tones/_index.md` — the Quick Match table maps phrases like "make it funny" to the right file.
- **Don't know which subgenre?** Open `subgenres/_index.md` for cyberpunk, space opera, cozy mystery, and more.
- **Full routing details?** Read `SKILL.md` for the complete pipeline.
