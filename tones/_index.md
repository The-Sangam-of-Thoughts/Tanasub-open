# Tone Index

## Quick Match

Common user phrases mapped to tone files:

| User says… | Load this file |
|---|---|
| "make it funny" / "humorous" / "witty" / "gallows humor" | `comedic.md` |
| "dry humor" / "deadpan" / "tongue-in-cheek" / "wry" | `deadpan.md` |
| "playful" / "quirky" / "whimsical" / "fanciful" | `whimsical.md` |
| "cheeky" / "irreverent" / "impious" / "anti-pompous" | `irreverent.md` |
| "deep" / "philosophical" / "thought-provoking" / "contemplative" / "ideas-first" | `philosophical.md` |
| "introspective" / "reflective" / "pensive" / "journal-like" / "serene" / "meditative" | `reflective.md` |
| "sad" / "mournful" / "bittersweet" / "elegiac" / "lamenting" | `elegiac.md` |
| "nostalgic" / "wistful" / "sepia-toned" / "reminiscent" | `nostalgic.md` |
| "inspiring" / "motivational" / "uplifting" / "hopeful" | `inspirational.md` |
| "poetic" / "musical" / "beautiful prose" / "lyrical" / "cadenced" | `lyrical.md` |
| "devotional" / "solemn" / "reverent" / "hushed" / "solemn-awe" | `reverent.md` |
| "friendly" / "warm" / "breezy" / "earnest" / "sincere" / "companionable" | `warm.md` |
| "dark mood" / "bleak" / "somber" / "grim" / "unflinching" | `grim.md` |
| "sarcastic" / "sardonic" / "cynical" / "jaded" / "disillusioned" | `cynical.md` |
| "urgent" / "pressing" / "insistent" / "time-bound" | `urgent.md` |
| "defiant" / "resistant" / "protest" / "unbowed" | `defiant.md` |
| "confessional" / "vulnerable" / "intimate" / "close" | `intimate.md` |
| "clinical" / "matter-of-fact" / "neutral" / "detached" | `detached.md` |
| "empathetic" / "consoling" / "tender" / "compassionate" | `compassionate.md` |

---

Load only the tone file needed for the current writing task. Tone is a modifier:
it colors the voice. It never overrides the genre's emotional engine. Use the
[alias table](#alias-resolution) when a brief uses loose vocabulary.

## Tones

| Name | ID | Family | Aliases | Status | File |
|---|---|---|---|---|---|
| Comedic | `tone-comedic` | Humor | funny, humorous, witty, gallows humor | drafted | [comedic.md](comedic.md) |
| Deadpan | `tone-deadpan` | Humor | dry, tongue-in-cheek, wry | drafted | [deadpan.md](deadpan.md) |
| Whimsical | `tone-whimsical` | Humor | playful, fanciful, quirky | drafted | [whimsical.md](whimsical.md) |
| Irreverent | `tone-irreverent` | Humor | cheeky, impious, anti-pompous | drafted | [irreverent.md](irreverent.md) |
| Philosophical | `tone-philosophical` | Contemplation | contemplative, ideas-first, dialectical | drafted | [philosophical.md](philosophical.md) |
| Reflective | `tone-reflective` | Contemplation | introspective, journal-like, pensive | drafted | [reflective.md](reflective.md) |
| Elegiac | `tone-elegiac` | Contemplation | mournful, lamenting, bittersweet | drafted | [elegiac.md](elegiac.md) |
| Nostalgic | `tone-nostalgic` | Contemplation | wistful, sepia-toned, reminiscent | drafted | [nostalgic.md](nostalgic.md) |
| Inspirational | `tone-inspirational` | Elevation | motivational, uplifting, hopeful | drafted | [inspirational.md](inspirational.md) |
| Lyrical | `tone-lyrical` | Elevation | poetic, musical, cadenced | drafted | [lyrical.md](lyrical.md) |
| Reverent | `tone-reverent` | Elevation | devotional, solemn-awe, hushed | drafted | [reverent.md](reverent.md) |
| Warm | `tone-warm` | Elevation | friendly, breezy, companionable, earnest | drafted | [warm.md](warm.md) |
| Grim | `tone-grim` | Gravity | bleak, somber, unflinching | drafted | [grim.md](grim.md) |
| Cynical | `tone-cynical` | Gravity | sardonic, jaded, disillusioned | drafted | [cynical.md](cynical.md) |
| Urgent | `tone-urgent` | Gravity | pressing, insistent, time-bound | drafted | [urgent.md](urgent.md) |
| Defiant | `tone-defiant` | Gravity | resistant, protest-voiced, unbowed | drafted | [defiant.md](defiant.md) |
| Intimate | `tone-intimate` | Candor | confessional, vulnerable, close | drafted | [intimate.md](intimate.md) |
| Detached | `tone-detached` | Candor | clinical, matter-of-fact, neutral | drafted | [detached.md](detached.md) |
| Compassionate | `tone-compassionate` | Candor | empathetic, consoling, tender | drafted | [compassionate.md](compassionate.md) |

Status values: `planned` (card not yet written), `drafted` (card exists,
unreviewed), `reviewed` (findings resolved), `accepted` (coordinator-integrated).
The coordinator updates this table at integration. Tone identifiers resolve by
file existence in `tones/`; this index is the human/agent resolution layer.

## Alias resolution

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

## Combination

Tone is resolved with a genre or without one. Precedence, hybrid patterns, and
genre-family guidance live in [combination rules](_combination-rules.md).

## Related

- [Tone taxonomy](../docs/architecture/tone-taxonomy.md)
- [ADR-0004](../docs/decisions/ADR-0004-tone-layer.md)
