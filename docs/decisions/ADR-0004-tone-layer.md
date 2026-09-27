# ADR-0004: Tone Layer — orthogonal voice-attitude guidance

- Status: accepted by product owner
- Date: 2026-09-24

## Decision

Tanasub Open adds a **Tone Layer**: an orthogonal, evidence-based guidance
system for the narrator's voice attitude — the emotional coloring of prose
(philosophical, comedic, elegiac, urgent, and similar attitudes) that is
distinct from genre, register, and mode. The layer ships 19 research-backed
tone cards in `tones/`, a precedence system in `tones/_combination-rules.md`,
per-tone evidence dossiers under `references/tone-evidence/`, routing guidance,
and QA integration.

The Tone Layer is a **modifier, not a pipeline stage**. It loads between genre
selection and humanization, and only when a brief names an emotional attitude.
Tone-less routing is byte-identical to today's behavior.

## Concept model

Four distinct axes govern prose, each owning a different decision:

| Axis | Owns | Lives in |
|---|---|---|
| Genre engine | The reader's target feeling (what the piece should produce) | `genres/`/`subgenres/` Ch03 + Ch09 (unchanged) |
| Mode | Structural attitude at genre scale | existing `axis_type: mode` files (satire, pastoral, speculative) |
| Tone | The narrator's voice attitude (how it sounds getting there) | `tones/` |
| Register | Formality and situation-appropriate vocabulary | Layer 2 voice brief |

Governing sentence, reused across SKILL.md, Layer 2, and the combination rules:

> **Stakes belong to the genre; texture belongs to the tone; formality belongs
> to the register.**

A tone may re-color, modulate, or sit in tension with a genre engine, but it may
never silently override the engine the reader was promised.

## Decisions

1. **D1 — Orthogonal modifier directory, not a pipeline stage.** Tone cards load
   on demand; unused tone files cost zero tokens. The pipeline becomes
   Layer 0 → [Layer 1] → [genre|subgenre] → [tone] → Layer 2 → Layer 3.
2. **D2 — One primary tone.** No tone-stacking in routing, mirroring the
   one-genre rule. Hybrids resolve through alias tension notes and the
   integration pattern in the combination rules.
3. **D3 — Genre files untouched.** All 32 axis files remain unchanged;
   combination logic lives in `tones/_combination-rules.md` and each card's §6.
   Orthogonality is the product.
4. **D4 — Dossier-first authorship.** Every card derives from a mandatory
   research dossier in a per-tone evidence silo, and every mechanism claim cites
   a silo claim ID (or an existing shared claim ID).
5. **D5 — Shared registries are coordinator-only.** `references/id-registry.json`,
   `references/indexes/master-index.json`, and everything under
   `references/evidence/` are never written by fleet agents; the coordinator
   performs all registration serially after review.
6. **D6 — Card budget 160–220 lines** (~2–2.5K tokens). The card budget is a
   template constraint enforced by the card validator. Pipeline token size is
   measured for information only — **there is no hard token cap**;
   token-saving measures may be adopted voluntarily and are never enforced
   as a gate.
7. **D7 — Family-level combination matrix + ≤90 flagged pairs.** Pairing
   guidance is expressed per tone family against genre families, never as a
   19 × 32 grid.
8. **D8 — No tool-side alias resolution.** Aliases live in `tones/_index.md` for
   human and agent resolution; tone loading stays filename-strict, consistent
   with genre routing.
9. **D9 — Restraint sections are blocking content.** Every card carries
   observable dosage thresholds, saturation signals, and context prohibitions.
   "Use sparingly" fails review.
10. **D10 — Tone QA is conditional-blocking.** Tone fidelity blocks only when a
    tone was explicitly requested; otherwise it is `not applicable` with a
    one-line reason.

## Router contract

- One optional tone identifier on the brief, or none.
- Route order: Layer 0 → [Layer 1 if `storytelling`] → [genre XOR subgenre] →
  [tone] → Layer 2 → Layer 3.
- Tone identifiers use the same hygiene as genre/subgenre: lowercase, no path
  parts, validated by file existence in `tones/`, with `_`-prefixed files
  excluded (`_index`, `_combination-rules`, templates).
- Tone is independent of genre/subgenre: either, both, or neither may be set.
- A brief without `tone` routes exactly as before.

## Compatibility

- Adding an optional `tone` field to the shared record schemas is additive; the
  record schema minor version bumps.
- Unknown-property rejection in the v1 schemas is preserved.
- The Tone Layer runs entirely from files committed in this repository. It is
  fully local and independently useful, consistent with ADR-0001's scope.

## Consequences

The system gains an explicit control for its most-requested missing craft axis:
voice attitude. Hybrid briefs ("comedic horror", "philosophical blog post")
become expressible without new genre files, and one tone card composes across
all 32 axes and both Layer 0 forms. The layer adds 19 cards, 19 dossiers,
routing, QA, and documentation work tracked across the Tone Layer program.

Expansion beyond 19 tones is a post-ship decision requiring its own evidence
packet. Taxonomy changes after the Wave 0 freeze require coordinator re-freeze
and re-dispatch of affected slots only.

## Related

- [ADR-0001](ADR-0001-tanasub-name.md) — Tanasub naming and scope
- [Tone taxonomy](../architecture/tone-taxonomy.md) — the frozen 19
