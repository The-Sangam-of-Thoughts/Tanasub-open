# Tone taxonomy (frozen 2026-09-24)

The frozen taxonomy for the Tanasub Open Tone Layer, recorded by
[ADR-0004](../decisions/ADR-0004-tone-layer.md). Changes after this freeze
require coordinator re-freeze and re-dispatch of affected slots only. Fleet
workers may propose changes; they may not self-serve them.

## Concept model

| Axis | Owns | Lives in |
|---|---|---|
| Genre engine | The reader's target feeling | `genres/`/`subgenres/` Ch03 + Ch09 |
| Mode | Structural attitude at genre scale | existing `axis_type: mode` files |
| Tone | The narrator's voice attitude | `tones/` |
| Register | Formality and vocabulary | Layer 2 voice brief |

Governing sentence: **Stakes belong to the genre; texture belongs to the tone;
formality belongs to the register.**

## Inclusion criteria

A tone enters the taxonomy only when it passes all five:

1. **Voice-level attitude** — describes how the narrator sounds, not what the
   reader should feel (genre engine) and not formality (register).
2. **Real brief demand** — commonly requested in actual writing briefs.
3. **Definable boundary** — a one-sentence boundary distinguishes it from each
   nearest neighbor.
4. **Cross-form validity** — operates in at least three forms (academic,
   blog/marketing, fiction, poetry, copy).
5. **Cross-cultural evidence** — at least two non-Anglophone traditions, at
   least one Indian/regional, have documented engagement with the attitude.

## The 19 tones

Families: **Humor**, **Contemplation**, **Elevation**, **Gravity**, **Candor**.

### Family: Humor

| Field | Value |
|---|---|
| ID | `tone-comedic` |
| Label | Comedic |
| Aliases | funny, humorous, witty, gallows humor (with grim tension) |
| Boundary | Humor is carried by content and structure (setup/payoff, escalation, wordplay). Differs from `tone-deadpan`, where humor lives in flat delivery, and from the `satirical-literature` mode, which critiques a specific target. Comedy needs no target. |

| Field | Value |
|---|---|
| ID | `tone-deadpan` |
| Label | Deadpan |
| Aliases | dry, tongue-in-cheek, wry |
| Boundary | The comic effect comes from expressionless delivery of absurd content. Differs from `tone-comedic` (which uses joke machinery) and `tone-detached` (which is neutral without comic intent). |

| Field | Value |
|---|---|
| ID | `tone-whimsical` |
| Label | Whimsical |
| Aliases | playful, fanciful, quirky |
| Boundary | Light, fanciful imagination that delights in its own invention. Differs from `tone-comedic` (no joke machinery required) and `tone-nostalgic` (present-facing caprice, not past-facing longing). |

| Field | Value |
|---|---|
| ID | `tone-irreverent` |
| Label | Irreverent |
| Aliases | cheeky, impious, anti-pompous |
| Boundary | Disrespect toward sacred or self-important registers without a single sustained target. Differs from `satirical-literature` (which has a target and a critique) and `tone-cynical` (which distrusts rather than teases). |

### Family: Contemplation

| Field | Value |
|---|---|
| ID | `tone-philosophical` |
| Label | Philosophical |
| Aliases | contemplative, meditative, ideas-first |
| Boundary | Ideas are the subject; the voice abstracts toward meaning, principle, and consequence. Differs from `tone-reflective`, which stays personal and inward, and from `tone-reverent`, which directs attention to a sacred object. |

| Field | Value |
|---|---|
| ID | `tone-reflective` |
| Label | Reflective |
| Aliases | introspective, journal-like, pensive |
| Boundary | The narrator turns inward on personal experience. Differs from `tone-philosophical` (abstract, outward) and `tone-nostalgic` (oriented to a specific idealized past). |

| Field | Value |
|---|---|
| ID | `tone-elegiac` |
| Label | Elegiac |
| Aliases | mournful, lamenting, bittersweet (with warm/nostalgic tension) |
| Boundary | Faces loss and impermanence in the present. Differs from `tone-nostalgic` (warmer, past-facing) and `tone-grim` (bleak without mourning's tenderness). |

| Field | Value |
|---|---|
| ID | `tone-nostalgic` |
| Label | Nostalgic |
| Aliases | wistful, sepia-toned, reminiscent |
| Boundary | Idealized, bittersweet orientation to a remembered past. Differs from `tone-elegiac` (present loss) and `tone-warm` (present-facing affection). |

### Family: Elevation

| Field | Value |
|---|---|
| ID | `tone-inspirational` |
| Label | Inspirational |
| Aliases | motivational, uplifting, hopeful |
| Boundary | Forward-facing possibility and courage; the reader is moved to act or believe. Differs from `tone-reverent` (awe before something sacred) and `tone-lyrical` (beauty of language). |

| Field | Value |
|---|---|
| ID | `tone-lyrical` |
| Label | Lyrical |
| Aliases | poetic, musical, cadenced |
| Boundary | Beauty of language and rhythm is part of the meaning. Differs from `tone-reverent` (the object of awe, not the sound) and `tone-philosophical` (ideas, not music). |

| Field | Value |
|---|---|
| ID | `tone-reverent` |
| Label | Reverent |
| Aliases | devotional, solemn-awe, hushed |
| Boundary | Awe and sacred attention directed at something held holy or profound. Differs from `tone-grim` (weight without awe) and `tone-lyrical` (aesthetic rather than devotional). |

| Field | Value |
|---|---|
| ID | `tone-warm` |
| Label | Warm |
| Aliases | friendly, breezy, companionable, earnest |
| Boundary | Affiliative kindness toward the reader. Differs from `tone-compassionate` (care inside suffering) and `tone-nostalgic` (past-facing). |

### Family: Gravity

| Field | Value |
|---|---|
| ID | `tone-grim` |
| Label | Grim |
| Aliases | bleak, somber, unflinching |
| Boundary | Unflinching weight and bleakness. Differs from `tone-cynical` (distrust and bitter irony) and `tone-elegiac` (mourning with tenderness). |

| Field | Value |
|---|---|
| ID | `tone-cynical` |
| Label | Cynical |
| Aliases | sardonic, jaded, disillusioned |
| Boundary | Distrust of stated motives and ideals; bitter irony as a default posture. Differs from `satirical-literature` (a targeted critique) and `tone-grim` (bleak without the ironic edge). |

| Field | Value |
|---|---|
| ID | `tone-urgent` |
| Label | Urgent |
| Aliases | pressing, insistent, time-bound |
| Boundary | Insistence that the matter cannot wait; time and consequence press on the reader. Differs from `tone-defiant` (resistance) and `tone-inspirational` (possibility rather than deadline). |

| Field | Value |
|---|---|
| ID | `tone-defiant` |
| Label | Defiant |
| Aliases | resistant, protest-voiced, unbowed |
| Boundary | Principled resistance against a power or expectation. Differs from `tone-irreverent` (mockery rather than resistance) and `tone-urgent` (deadline rather than opposition). |

### Family: Candor

| Field | Value |
|---|---|
| ID | `tone-intimate` |
| Label | Intimate |
| Aliases | confessional, vulnerable, close |
| Boundary | Reader-closeness through disclosed interiority. Differs from `tone-reflective` (private introspection, not addressed outward) and `tone-warm` (affection without disclosure). |

| Field | Value |
|---|---|
| ID | `tone-detached` |
| Label | Detached |
| Aliases | clinical, matter-of-fact, neutral |
| Boundary | Neutral, observational distance; affect is withheld deliberately. Differs from `tone-deadpan` (flatness for comic effect) and `tone-reflective` (inward rather than outward observation). Highest AI-slop-risk tone; the structural-tells catalog applies hardest here. |

| Field | Value |
|---|---|
| ID | `tone-compassionate` |
| Label | Compassionate |
| Aliases | empathetic, consoling, tender |
| Boundary | Care expressed inside another's suffering. Differs from `tone-warm` (general kindness) and `tone-elegiac` (the narrator's own mourning). |

## Alias resolution

Briefs use loose vocabulary. Resolution is a human/agent concern via this
table; tone files stay filename-strict (D8).

| Brief vocabulary | Primary tone | Noted tension |
|---|---|---|
| motivational, uplifting, hopeful | `tone-inspirational` | toxic-positivity guard |
| playful, fanciful, quirky | `tone-whimsical` | — |
| tongue-in-cheek, wry, dry | `tone-deadpan` | ironic bend |
| sardonic, jaded, disillusioned | `tone-cynical` | deadpan delivery option |
| gallows humor, darkly comic | `tone-comedic` | grim stakes (integration) |
| bittersweet | `tone-elegiac` | warm/nostalgic secondary |
| confessional, vulnerable | `tone-intimate` | — |
| clinical, matter-of-fact | `tone-detached` | — |
| breezy, friendly, companionable | `tone-warm` | — |
| earnest, sincere | `tone-warm` | reflective secondary |
| serene, meditative | `tone-reflective` | lyrical secondary |
| solemn | `tone-reverent` | grim secondary |

## Evidence seeds

Indicative research anchors serve as research leads only and are never pre-accepted citations. Each tone's researcher verifies every anchor before use and records it in that tone's evidence silo (`references/tone-evidence/<tone>/`).

## Related

- [ADR-0004](../decisions/ADR-0004-tone-layer.md)
- [Tone index](../../tones/_index.md)
- [Combination rules](../../tones/_combination-rules.md)
