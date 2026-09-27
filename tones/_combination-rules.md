# Tone combination rules

How a tone composes with a genre, a mode, a register, and the two Layer 0 forms.
Read this before applying any tone card's §6, and cite the pattern names here.

## The four axes

| Axis | Owns | Lives in |
|---|---|---|
| Genre engine | The reader's target feeling | `genres/`/`subgenres/` Ch03 + Ch09 |
| Mode | Structural attitude at genre scale | `axis_type: mode` files (satirical-literature, pastoral-literature, speculative-fiction) |
| Tone | The narrator's voice attitude | `tones/` |
| Register | Formality and vocabulary | Layer 2 voice brief |

**Dominance rule:** on stakes, the genre wins; on texture, the tone wins; on
vocabulary, the register wins. A tone may never silently override the engine the
reader was promised.

**Governing sentence:** **Stakes belong to the genre; texture belongs to the
tone; formality belongs to the register.**

## One primary tone

Route one tone. Hybrid requests resolve through the alias table in
[`_index.md`](_index.md) to a primary tone plus a named tension, then follow the
integration pattern below. Do not load two tone cards.

## Three conflict patterns

Every tone × genre pairing is handled by one of:

1. **Re-color** — the genre engine still fires; the tone adjusts voice texture.
   Example: comedic horror. Dread survives; humor lives in psychic distance and
   the narrator's phrasing, never in deflating the stakes. The engine property
   that must survive is named in the card's §6.
2. **Alternate** — tone and engine trade dominance by section or scene, joined
   by a modulation bridge that signals the shift honestly. Example: an elegiac
   opening that moves into reflective analysis.
3. **Integrate** — both hold simultaneously in a named hybrid (dark comedy,
   tragicomedy, cozy uplift, bittersweet). The card's §6 states the two
   invariants: what must stay genre-true and what must stay tone-true.

If a pairing fits none of the three, it is flagged as **high-tension** and
resolved explicitly rather than forced.

## Tonal modulation and drift

- **Modulation** is deliberate: the piece opens in one tone and lands in
  another. It requires a bridge and a reason. Without both, it reads as drift.
- **Tonal drift** is accidental: the voice wanders because the draft lost its
  brief. Diagnostic: can you name the tone of each section? If not, drift.
- **Tonal whiplash** is abrupt, unbridged switching between incompatible tones.
  Diagnostic: does the register or stakes level change without a transition?
  Fix: add the bridge or cut one tone from the piece.

## Genre families

Combination guidance is expressed per tone family against these eight genre
families plus the two Layer 0 forms. (Satirical-literature is a mode and is
handled as a cross-cutting note in each card, not as a family.)

| # | Family | Members |
|---|---|---|
| 1 | Speculative | speculative-fiction, fantasy-fiction, science-fiction; subgenres cyberpunk, solarpunk, space-opera, urban-fantasy |
| 2 | Horror | horror-fiction, gothic-fiction |
| 3 | Romance | romance-fiction |
| 4 | Thriller & Mystery | thriller-fiction, detective-and-mystery-fiction; subgenres psychological-thriller, cozy-mystery |
| 5 | Literary & Realist | historical-fiction, picaresque-literature; subgenres bildungsroman, psychological-fiction |
| 6 | Dramatic & Screen | nataka-drama, prakarana-drama, feature-screenplay, episodic-television-script |
| 7 | Poetic & Lyric | ghazal-sequence, vachana-poetry, pastoral-literature |
| 8 | Structural & Traditional | epistolary-fiction, frame-narrative, flash-fiction, interactive-fiction, dastan-tradition, katha-tradition |
| — | Layer 0 forms | academic (`layer0-academic.md`), blog/marketing (`layer0-blog.md`) |

## Matrix

Combination guidance runs per tone family against the eight genre families and
the two Layer 0 forms. Each row names one of the three patterns for every card
in the family and states the engine property that must survive. Where cards
inside one family name different patterns for the same genre family, each
card's pattern is named rather than averaged, because a card's §6 is
authoritative for its own tone: where this matrix and a card's §6 appear to
differ, the card governs. Every rule cites a card mechanism at section
granularity (`tones/<tone>.md §n`, never line numbers) or a stored claim id
(`[@clm-…]`). Flagged high-tension pairs are collected under High-tension
pairings below, each with a resolution paragraph.

Two conventions bind the rows. The three pattern names are the only pattern
names: where a card bars a tone outright over specific content
(`tones/grim.md §4`, `tones/whimsical.md §6`, `tones/reverent.md §6`,
`tones/intimate.md §4`), the row names the bounded pattern — usually
`re-color` at most — and states the prohibition in prose: the tone is not used
there and the passage runs plain. And a row names the pattern while a flag
governs content inside the same pairing: where a card's §6 gives a family
pattern and its §4 or §7 restricts content within it (compare
`tones/deadpan.md §6` with `tones/deadpan.md §7`, and `tones/elegiac.md §6`
with `tones/elegiac.md §4`), both hold — the row names the pattern, the flag
gates the content.

Satirical-literature is a mode, never a matrix row. Where a brief routes the
mode, it owns structural judgment and the tone supplies texture only, with
staging kept visible: irreverence rotates and prosecutes nothing
(`tones/irreverent.md §1`, `tones/irreverent.md §7`); the reflective voice runs
only where the brief stages it as the mode's object (`tones/reflective.md §6`);
reverence, uplift, and lyrical density stay visible as staging rather than as
the target (`tones/reverent.md §6`, `tones/inspirational.md §6`,
`tones/lyrical.md §6`); a levelled or cool surface is the vehicle while the
mode owns the judgment (`tones/detached.md §6`); satire indicting the savior is
convention, not failure (`tones/compassionate.md §7`); nostalgia keeps its
focalized frame where the mode adopts the voice (`tones/nostalgic.md §6`).
Mode-specific flags appear with the high-tension pairings.

### Humor + Gravity families

**Humor × Speculative — `integrate` (comedic, whimsical);
`re-color` (deadpan, irreverent).**
Comedic integrates mock-heroic inflation that serves the invented world and
never deflates the premise (`tones/comedic.md §6`); whimsical integrates an
invented prop that reasons *inside* the secondary world's consistency rules
rather than decorating it (`tones/whimsical.md §6`,
`[@clm-tone-whimsical-make-believe-props]`). Deadpan re-colors: the premise's
idea-question and the world's rules survive, and flatness textures narration
only (`tones/deadpan.md §6`). Irreverent re-colors: deflation levels human pomp
inside the thought experiment, never the premise itself
(`tones/irreverent.md §6`, `[@clm-tone-irreverent-hierarchy-leveling]`).

**Humor × Horror — `integrate` (comedic, dark comedy); `re-color`, strict
invariants (deadpan, irreverent); `re-color` at most, strict engine invariants
(whimsical). Flagged: *comedic × Horror*, *whimsical × Horror*,
*deadpan × Horror*, *irreverent × Horror*.**
Comedic integrates dread-first with humour living in psychic distance and
phrasing, never in deflating the stakes (`tones/comedic.md §6`,
`[@clm-tone-comedic-comic-distance]`). Deadpan re-colors: flatness may amplify
the uncanny — a haunting in case-file cadence — but must never neutralize the
danger (`tones/deadpan.md §6`, `[@clm-tone-deadpan-clinical-reportage]`).
Whimsical is `re-color` at most: the card's first option is not to use the
tone, and where it is used, whimsy lives in a safe frame *inside* the horror,
never over the threat (`tones/whimsical.md §6`,
`[@clm-tone-whimsical-tonal-clash-stakes]`). Irreverent re-colors with strict
invariants: a pompous institution inside the horror may be leveled, never the
danger or the victim's fear (`tones/irreverent.md §6`,
`tones/irreverent.md §7` mode 4 Scope — the lived-sacred line: grief and
ritual that matter to a participant are never convention).

**Humor × Romance — `integrate` (comedic, romantic comedy);
`re-color` (deadpan, whimsical, irreverent).**
Comedic integrates: the optimistic arc and its emotional risk survive, and
jokes re-color obstacles, not the bond (`tones/comedic.md §6`). Deadpan
re-colors but never lands on the confession — that beat yields to plain speech
(`tones/deadpan.md §6`; flagged: *deadpan × Romance*). Whimsical re-colors:
caprice colors obstacles, not the bond (`tones/whimsical.md §6`). Irreverent
re-colors: coloring obstacles and officious blockers only, never the confession
or the bond (`tones/irreverent.md §6`).

**Humor × Thriller & Mystery — `re-color` (all four; strict
invariants for comedic and whimsical).**
Jeopardy and the reader's promise of resolution survive in every row: wit stays
in the narrator's phrasing, never making danger harmless (`tones/comedic.md
§6`); case-file flatness is native to the procedural but clues must stay
readable (`tones/deadpan.md §6`, `[@clm-reader-promise]`); invention stays in
the narrator's phrasing, never making danger harmless (`tones/whimsical.md §6`);
mockery of procedure may never make live danger harmless
(`tones/irreverent.md §6`).

**Humor × Literary & Realist — `integrate` (comedic, deadpan,
irreverent); `alternate` (whimsical).**
Comedic integrates with comedy arising from character and system, not
authorial commentary (`tones/comedic.md §6`). Deadpan integrates genre-true
character truth and consequence with tone-true localized flatness, the surface
never turning characters into props (`tones/deadpan.md §6`,
`tones/deadpan.md §7` target-loss mode). Irreverent integrates leveling aimed
at offices and performances the world itself supplies, never at characters as
props (`tones/irreverent.md §6`). Whimsical alternates: the realist engine and
the fanciful texture trade dominance by section, joined by a bridge, because
the play frame brackets consequence and may not run continuous over real stakes
(`tones/whimsical.md §6`, `tones/whimsical.md §4`).

**Humor × Dramatic & Screen — `re-color` (all four).**
The scene's turn and dialogue subtext survive everywhere
(`[@clm-scene-turning-points]`, `[@clm-dialogue-subtext]`): a comic line must
serve subtext, not stall the scene with talking heads (`tones/comedic.md §6`);
stage and camera supply the face natively, and prose adaptations rebuild it as
register stasis (`tones/deadpan.md §6`,
`[@clm-tone-deadpan-performance-transfer]`); an invented beat must serve the
scene's beat, not stall it (`tones/whimsical.md §6`); insolence rides role-pairs
inside the scene — kyōgen's method — and never stalls it
(`tones/irreverent.md §6`).

**Humor × Poetic & Lyric — `alternate` (all four).**
Lyric dwelling and the comic beat trade dominance by section, joined by a
bridge, in every row: humour stays concrete so it does not kill cadence
(`tones/comedic.md §6`, `tones/comedic.md §3` poetry caution); the flat beat
serves the image and never flattens it, and whole stanzas never run dead flat
(`tones/deadpan.md §6`, `tones/deadpan.md §3`); sound-play must serve the line
(`tones/whimsical.md §6`, `tones/whimsical.md §3`); one deflation trades with
dwelling by section, and where the lineage is native — bhakti and vachana verse
— leveling may hold the foreground (`tones/irreverent.md §6`,
`[@clm-tone-irreverent-indian-anticlerical-hasya]`).

**Humor × Structural & Traditional — `re-color` (all four).**
Form rules survive in every row: a comic document's form carries the joke
without breaking the form's logic (`tones/comedic.md §6`); a memo or log's form
carries the beat, and in flash the white space is the beat
(`tones/deadpan.md §6`); katha keeps its frame and *niti*, flash keeps
single-effect compression and the *volta*, and invention never adds words the
form cannot carry (`tones/whimsical.md §6`); epistle, frame, flash, dastan and
katha survive, with rule-bound insolence riding the form's own license and
expiry (`tones/irreverent.md §6`, `[@clm-tone-irreverent-licensed-frame]`).

**Humor × Academic (Layer 0) — `re-color` (all four). Flagged: *comedic ×
academic*.**
Argument, the evidence contract, and the thesis survive in every row: the joke
illustrates and never replaces the claim, and must not be promised to persuade
(`tones/comedic.md §6`, `tones/comedic.md §3`,
`[@clm-tone-comedic-superiority-limits]`); one dry illustrative sentence while
definitions, data claims, and the thesis stay literal (`tones/deadpan.md §6`,
`tones/deadpan.md §3`); the invented prop illustrates and never replaces the
claim (`tones/whimsical.md §6`, `tones/whimsical.md §3`); one deflating
illustration serves the claim while anti-pomp never touches the evidence
(`tones/irreverent.md §6`, `tones/irreverent.md §3`). L0 contract:
`layers/layer0-academic.md` requires consequential claims to be written only
when their support is available and fit for that exact claim.

**Humor × Blog / marketing (Layer 0) — `integrate` (comedic,
whimsical); `re-color` (deadpan, irreverent). Flagged: *Humor family × crisis,
bereavement, and safety/medical/legal copy*, *deadpan × blog / marketing*.**
Comedic integrates voice and promised takeaway, yielding at the CTA and at
the thesis sentence (`tones/comedic.md §6`, `tones/comedic.md §4`); whimsical
integrates voice and takeaway, yielding at the CTA
(`tones/whimsical.md §6`). Deadpan re-colors while keeping institutional nouns
from reading as actual corporate blandness (`tones/deadpan.md §6`,
`tones/deadpan.md §7` corporate-blandness mode; flagged: *deadpan × blog /
marketing*). Irreverent re-colors by deflating the category's buzzwordery,
yielding at the CTA and never mocking the reader's problem or the client's
promise (`tones/irreverent.md §6`, `tones/irreverent.md §3`). L0 contract:
`layers/layer0-blog.md` forbids inventing audience research, product
performance, testimonials, scarcity, or results, and a hook may not manufacture
fear, certainty, urgency, or a promise the body cannot deliver.

**Gravity × Speculative — `re-color` (all four).**
Estrangement and the premise's "what if?" survive everywhere: grim voices the
aftermath texture and never answers the thought experiment with mere despair
(`tones/grim.md §6`); the voice deflates human claims inside the thought
experiment, never the premise itself (`tones/cynical.md §6`); urgency voices a
concrete, locatable countdown rather than replacing world with alarm
(`tones/urgent.md §6`, `[@clm-tone-urgent-exigence-reality]`); resistance
addresses the world's power structure and never replaces its wonder
(`tones/defiant.md §6`).

**Gravity × Horror — `re-color` (all four; strict invariants where
noted). Flagged: *urgent × Horror*, *defiant × Horror*.**
The fear engine and the dread curve survive (`tones/grim.md §6`,
`[@clm-tone-grim-dread-looming]`, `[@clm-reader-promise]`); a character may
distrust the institution's reassurances, but the threat and stakes are never
deflated (`tones/cynical.md §6`); the deadline is a human clock and must not
deflate the uncanny (`tones/urgent.md §6`, `tones/urgent.md §2`
efficacy-gate; flagged: *urgent × Horror*); defiance must not promise heroism
the horror engine denies (`tones/defiant.md §6`, `tones/defiant.md §3`
vindication endings; flagged: *defiant × Horror*).

**Gravity × Romance — `alternate` (grim, urgent, defiant);
`re-color` for one character's voice only (cynical — the seeded *cynical ×
Romance* pairing).**
Grim alternates: bleak scenes and the bond trade dominance by section joined by
an honest bridge, and grim yields at the bond (`tones/grim.md §6`). Urgent
alternates: the dwelling romantic beat and urgency trade by scene with a bridge
(`tones/urgent.md §6`). Defiant alternates: a refusal against family or
expectation trades by scene with a bridge (`tones/defiant.md §6`). Cynical
re-colors for one character's voice only — the optimistic arc and the bond's
sincere beats stay untouched and the cynic is a character, not the narrative
(`tones/cynical.md §6`, `[@clm-tone-cynical-irony-echoic]`).

**Gravity × Thriller & Mystery — `re-color` (all four; urgent
restricted to the prospective present; flagged: *urgent × Thriller &
Mystery*).**
Jeopardy, the clock, and suspense's reader-state survive: grim's accelerating
threat serves the looming engine and mystery takes the bleak past as
discovered fact (`tones/grim.md §6`, `[@clm-tone-grim-dread-looming]`);
motive-reading is detection's own habit, so the texture serves the clock
(`tones/cynical.md §6`); suspense is a reader-state engine the tone may color
but never claims, and mystery's retrospective engine resists deadlines, so
urgency is reserved for the prospective present (`tones/urgent.md §6`,
`tones/urgent.md §1`, `[@clm-suspense-vs-surprise]`); defiance is a character's
voice and no deadline is manufactured (`tones/defiant.md §6`).

**Gravity × Literary & Realist — `integrate` (all four).**
The family's native prose home for both families: grim holds realist engine and
grim texture when the meaning-frame is earned by the world, not asserted by the
narrator (`tones/grim.md §6`,
`[@clm-tone-grim-meaning-making-negative-affect]`); cynical holds together when
the world supplies the record the voice reads against (`tones/cynical.md §6`,
`[@clm-tone-cynical-irony-echoic]`); urgent holds interiority and time-stakes
when the deadline is the character's own
(`tones/urgent.md §6`, `[@clm-character-desire-urgency]`); defiant holds when
the warrant is the character's own and is tested by cost
(`tones/defiant.md §6`, `[@clm-tone-defiant-moral-conviction]`).

**Gravity × Dramatic & Screen — `re-color` (grim, cynical);
`alternate` (urgent, defiant).**
Scene action and subtext survive everywhere (`[@clm-scene-turning-points]`,
`[@clm-dialogue-subtext]`): grim lives in staging and narration while
characters underplay rather than declaim (`tones/grim.md §6`); cynicism lives
in staging and delivery while characters underplay (`tones/cynical.md §6`);
act-turn pressure and scene-level dwelling trade off
(`tones/urgent.md §6`); refusal externalizes as action or subtext, never as a
speechifying pause (`tones/defiant.md §6`).

**Gravity × Poetic & Lyric — `integrate` (grim, cynical, defiant);
`alternate`, never `integrate` (urgent — the seeded *urgent × Poetic & Lyric*
pairing).**
Grim integrates the lyric's music with suggested-not-stated bleakness — karuna
and bhayanaka land through dhvani, never announcement
(`tones/grim.md §6`, `[@clm-tone-grim-rasa-karuna-bhayanaka]`,
`[@clm-dhvani-suggestion-theory]`). Cynical integrates the lyric's music with
the suggested-not-stated deflation, dhvani never announcement
(`tones/cynical.md §6`, `[@clm-dhvani-suggestion-theory]`). Defiant integrates
the chant cadence, with one sustained beat per movement keeping it from
emptying (`tones/defiant.md §6`, `tones/defiant.md §4`,
`[@clm-tone-defiant-dosage-yield]`). Urgent alternates by section and never
integrates: deadline pressure fights lyrical dwelling
(`tones/urgent.md §6`, `tones/urgent.md §3`, `[@clm-pacing-rhythm-syntax]`).

**Gravity × Structural & Traditional — `re-color` (all four).**
The form's rules survive in every row: a frame chorus may carry the dead and a
short form may end unrelieved without desensitizing (`tones/grim.md §6`); a
cynical frame figure colors the teller, never the form's promise
(`tones/cynical.md §6`); a dated entry or final line carries the clock
(`tones/urgent.md §6`, `[@clm-tone-urgent-deadline-framing]`); a letter of
refusal, a testimonial, or a final entry carries the vow
(`tones/defiant.md §6`).

**Gravity × Academic (Layer 0) — `re-color` (grim, cynical,
defiant); `re-color` only when the evidence carries time-stakes, otherwise the
tone is not used (urgent). Flagged: *urgent × academic*, *defiant ×
academic*.**
Argument, evidence, and thesis survive: grim registers only where the subject
is genuinely bleak and yields at method and definition
(`tones/grim.md §6`, `tones/grim.md §3`); cynical registers as skepticism
toward stated claims, always checked against data (`tones/cynical.md §6`,
`tones/cynical.md §3`); defiant grounds a contested claim in a named warrant
but yields to evidence at the decisive counterargument and concedes one point
(`tones/defiant.md §6`, `tones/defiant.md §7` absolutism mode,
`[@clm-controlling-idea]`); urgent is a register mismatch unless the evidence
itself carries time-stakes (`tones/urgent.md §6`, `tones/urgent.md §3`,
`[@clm-tone-urgent-time-pressure-narrows-cognition]`; flagged: *urgent ×
academic*). L0 contract: `layers/layer0-academic.md` evidence contract and
five-tier source hierarchy.

**Gravity × Blog / marketing (Layer 0) — `re-color` (grim, cynical,
urgent); `alternate` (defiant). Flagged: *urgent × blog / marketing*,
*defiant × blog / marketing*.**
Voice and the promised takeaway coexist: grim frames an honest problem and its
cost, then yields at the CTA and never runs on children-facing copy
(`tones/grim.md §6`, `tones/grim.md §4`); cynical offers candor toward the
reader's skepticism, then a plain claim and a plain CTA — it cannot be the CTA
voice (`tones/cynical.md §6`, `tones/cynical.md §3`); urgent re-colors with the
§4 three-part test as a shipping gate (`tones/urgent.md §6`,
`tones/urgent.md §4`, `[@clm-tone-urgent-manufactured-urgency-line]`; flagged:
*urgent × blog / marketing*); defiant alternates, because each post needs
power, stake, and route or it is a slogan (`tones/defiant.md §6`,
`tones/defiant.md §7` sloganeering mode, `[@clm-tone-defiant-slogan-stakes]`;
flagged: *defiant × blog / marketing*).
L0 contract: `layers/layer0-blog.md` never-invent rule (scarcity, results,
testimonials) and its evidence requirement for consequential claims.

### Contemplation + Candor families

**Contemplation × Speculative — `integrate` (philosophical); `alternate`
(reflective, nostalgic); `re-color` (elegiac).**
Philosophical integrates by arguing the idea the novum already stages, paying
every abstraction with a concrete anchor (`tones/philosophical.md §6`,
`[@clm-tone-philosophical-concreteness-grounding]`). Reflective and nostalgic
alternate because the reveal belongs to the engine: reflection owns only the
lull after the reveal and must feed the story's next why/how question
(`tones/reflective.md §6`, `[@clm-tone-reflective-causal-momentum]`), while
nostalgia owns backstory and the post-reveal lull under its two-position frame
(`tones/nostalgic.md §6`, `[@clm-tone-nostalgic-dual-time-distance]`). Elegiac
re-colors: the lament textures the cost of change and must never stall
discovery (`tones/elegiac.md §6`).

**Contemplation × Horror — `alternate` (philosophical, reflective); `re-color`
(elegiac, nostalgic), with the elegiac and nostalgic active-threat tensions
flagged (*elegiac × Horror*, *nostalgic × Horror*).**
Dread owns the scene in all four cards: philosophical may frame it in a
reflective lull or coda but never across the scare, and its periodic cadence
must break at the peak (`tones/philosophical.md §6`, `tones/philosophical.md §4`,
`[@clm-tone-philosophical-periodic-cadence]`); reflective appears in the
approach or coda only, where interiority would otherwise deflate threat
(`tones/reflective.md §6`). Elegiac may let melancholy dwell in the ruin without
defusing the scare (`tones/elegiac.md §6`), and nostalgia may let a corrupted or
lost past haunt the approach or coda (`tones/nostalgic.md §6`) — but both cards
separately flag the tone over active-threat content as high-tension (their §6
high-tension notes; see the flagged pairings below).

**Contemplation × Romance — `re-color` (philosophical, reflective);
`integrate` (elegiac, nostalgic).**
Emotional risk and the tradition's ending survive in every row. Philosophical
reflection appears only as a wide-distance narrator's thought, never at the
confession (`tones/philosophical.md §6`); reflection reviews after the
confession and never delays it (`tones/reflective.md §6`). Elegiac and nostalgic
integrate as bittersweet under two stated invariants — the union beat stays
genre-true and the loss/then stays double-valenced — with HEA-bound drafts that
would canonize one golden moment alternating instead (`tones/elegiac.md §6`
Romance row; `tones/nostalgic.md §6`, `[@clm-tone-nostalgic-bittersweet-structure]`).

**Contemplation × Thriller & Mystery — `alternate` (all four cards). Flagged:
*elegiac × Thriller & Mystery*, *nostalgic × Thriller & Mystery*.**
Jeopardy survives; the tone owns the lulls. Philosophical works in the deduction
lull and drops at the chase, per its own kinetic-promise rule — horror, thriller
and mystery are kinetic promises whose peaks the tone yields
(`tones/philosophical.md §6`); reflective must raise or answer a causal question
inside the lull (`tones/reflective.md §6`,
`[@clm-tone-reflective-causal-momentum]`); elegy owns backstory and deduction
lobs only, never the active threat (`tones/elegiac.md §6`,
`tones/elegiac.md §4`); nostalgia's return-to-hometown or cold-case reverie owns
backstory the same way (`tones/nostalgic.md §6`). Every return to stakes is
bridged by a concrete event (`tones/philosophical.md §6` modulation note); the
active-threat overhangs of elegy and nostalgia are flagged with the
high-tension pairs.

**Contemplation × Literary & Realist — `integrate` (all four cards).**
The family's native prose home. Philosophical generalises outward from
historical empathy and character interiority (`tones/philosophical.md §6`), and
the then/now evaluation is native at novel scale — the bildungsroman's
retrospective split consciousness is reflective's structure at novel scale
(`tones/reflective.md §6`, `[@clm-tone-reflective-recollected-tranquillity]`).
Elegy is at home alongside memoir while present loss stays owed
(`tones/elegiac.md §6`, `[@clm-tone-elegiac-present-loss]`), and nostalgia's
named homes are historical-fiction, bildungsroman and frame-narrative
(`tones/nostalgic.md §6`) — gated by the *nostalgic × unexamined era-praise*
flag below.

**Contemplation × Dramatic & Screen — `re-color` (all four cards).**
Scene action and blocking survive everywhere; the weight moves into subtext and
image. Philosophical weight lives in subtext and image, not in a monologue —
abstraction in monologue stalls the scene (`tones/philosophical.md §6`,
`tones/philosophical.md §3`); reflection lives in beat, subtext and image after
the action, never in a speech that stops the scene (`tones/reflective.md §6`);
grief lives in kept object and held beat, because a mourning speech at the
action peak kills urgency (`tones/elegiac.md §6`, `tones/elegiac.md §3`); the
`then` lives in prop and subtext, because a reverie speech at the action peak
kills urgency (`tones/nostalgic.md §6`, `tones/nostalgic.md §3`).

**Contemplation × Poetic & Lyric — `integrate` (all four cards).**
The lyrical image or music survives in every row. Indirection is allowed only
when tethered to an arguable idea (`tones/philosophical.md §6`,
`[@clm-tone-philosophical-dhvani-suggestion]`); reflective allows one movement
per stanza-group with a concrete anchor (`tones/reflective.md §6`,
`tones/reflective.md §4` poetry dosage); in ghazal-sequence refrain sustains
grief without closure and in pastoral the seasonal-decay field is elegy's own
heritage (`tones/elegiac.md §6`, `[@clm-tone-elegiac-ghazal-grief]`); nostalgia
allows one reverie movement per stanza-group with a present anchor
(`tones/nostalgic.md §6`). The seeded *urgent × Poetic & Lyric* pairing governs
that outside-family case.

**Contemplation × Structural & Traditional — `alternate` (all four cards).**
The form's unit — entry, letter, nested tale — survives; the tones appear in
frame commentary and interludes between units. The philosophical frame must not
replace the form's own unit (`tones/philosophical.md §6`,
`tones/philosophical.md §3`); reflective commentary sits inside the unit's frame
and the dated entry licenses longer runs (`tones/reflective.md §6`,
`[@clm-tone-reflective-dosage-yield]`); elegy keeps unit autonomy while carrying
frame elegies and interludes (`tones/elegiac.md §6`, `tones/elegiac.md §3`);
nostalgia sits in frame commentary while the unit survives
(`tones/nostalgic.md §6`).

**Contemplation × Academic (Layer 0) — `re-color` (all four cards).**
The evidence contract and the bounded conclusion survive in every row.
Provisionality lives in the reasoning, never in abandoning the answer
(`tones/philosophical.md §6`, `[@clm-tone-philosophical-essai-provisional]`,
with §4's ban on staged suggestion in evidence-bearing academic prose);
reasoning may display its testing while every consequential claim stays sourced
(`tones/reflective.md §6`); memorial framing is confined to dedication or coda,
and grief never substitutes for a claim's warrant (`tones/elegiac.md §6`,
`tones/elegiac.md §3`); nostalgia appears only as documented framing —
motivation, lineage — never as warrant (`tones/nostalgic.md §6`,
`tones/nostalgic.md §3`).

**Contemplation × Blog / marketing (Layer 0) — `re-color` (all four cards).**
The reader promise and scannable structure survive in every row. Philosophical
offers one grounded idea with a concrete payoff and a portable close, and §4
prohibits opening on an abstraction the reader has no stake in
(`tones/philosophical.md §6`, `tones/philosophical.md §4` — see
*philosophical × abstraction-first openings* below);
reflective gives one personal turn labelled as experience
(`tones/reflective.md §6`); tribute content must clear the grief-mining and
ending-posture gates (`tones/elegiac.md §6`, `tones/elegiac.md §4`,
`[@clm-tone-elegiac-restraint-vs-sentimentality]`); throwback content must clear
the §4 counts and the consumption-ethics gate (`tones/nostalgic.md §6`,
`tones/nostalgic.md §4`, `[@clm-tone-nostalgic-consumption-ethics]`).

**Candor × Speculative — `re-color` (all three cards).**
Estrangement and idea-scale survive; each tone is a human register inside the
concept. Disclosure is a human voice inside the concept
(`tones/intimate.md §6`); detachment is the observer's register inside the
concept (`tones/detached.md §6`); compassion is the narrator's regard for a
person inside the concept, never a softening of its rules
(`tones/compassionate.md §6`).

**Candor × Horror — `re-color` (all three cards), with the compassionate row
flagged high-tension (*compassionate × Horror*).**
Dread and the uncanny survive in every row: personal confession must not deflate
the uncanny (`tones/intimate.md §6`); stripped prose de-automatizes the horror,
but distance must collapse at the crisis — that is the planned modulation, not a
drift (`tones/detached.md §6`, `[@clm-tone-detached-defamiliarization]`);
compassion for a victim must not make the danger safe, and the card's own row
reads "re-color, strict invariants … flagged high-tension"
(`tones/compassionate.md §6`).

**Candor × Romance — `integrate` (intimate, compassionate); `re-color` at wide
distance for detached, governed by the seeded *detached × Romance* pairing.**
Emotional risk survives throughout. For intimate, confession *is* the risk and
both invariants hold — disclosure and the engine's optimism arc together
(`tones/intimate.md §6`); compassion colours narration and never substitutes for
earned intimacy (`tones/compassionate.md §6`,
`[@clm-character-desire-urgency]`); detachment's neutrality blocks emotional
risk, so it holds wide distance with one charged detail per beat and never at
the confession (`tones/detached.md §6` Romance row, `tones/detached.md §4` drop
rule) — that case is stated explicitly by the seeded pairing below.

**Candor × Thriller & Mystery — `re-color` (all three cards).**
Suspense owns the reader-state in every row. Intimacy stays narrator texture
(`tones/intimate.md §6`, `[@clm-suspense-vs-surprise]`); fair-play clue
reporting keeps its plain register, and external focalization suits the
retrospective puzzle (`tones/detached.md §6`); compassion stays victim texture
and never becomes suspense relief (`tones/compassionate.md §6`).

**Candor × Literary & Realist — `integrate` (all three cards; the native home
for detached and compassionate). Flagged: *detached × victim-suffering
content*.**
Interiority and social detail hold together: intimate's close first person never
lets disclosure replace the scene (`tones/intimate.md §6`,
`tones/intimate.md §4`, `[@clm-tone-intimate-self-disclosure-closeness]`);
detached withholds affect while want and cost stay legible
(`tones/detached.md §6`, `[@clm-tone-detached-restraint-vs-absence]`);
compassionate accompanies rather than replaces a character's suffering, with
historical empathy intact (`tones/compassionate.md §6`). The detached row is
qualified by the *detached × victim-suffering content* flag wherever the
material is victim-suffering content.

**Candor × Dramatic & Screen — `alternate` (intimate, detached); `integrate`
(compassionate).**
Subtext and scene carry the charge. Intimate trades dominance by beat, with
disclosure dramatised rather than declared (`tones/intimate.md §6`). Detached
trades by scene, joined by the §4 bridge pattern — one close beat, then a
procedural sentence that re-establishes the neutral register
(`tones/detached.md §6`, `tones/detached.md §4`). Compassionate integrates,
holding the scene's turn while care lives in an action or a withheld line, never
on-the-nose dialogue (`tones/compassionate.md §6`, `[@clm-dialogue-subtext]`).

**Candor × Poetic & Lyric — `integrate` (intimate, compassionate); `alternate`
(detached).**
Confessional lyric lets apostrophe serve address and musicality, with
suggestion available in place of stated confession (`tones/intimate.md §6`,
`tones/intimate.md §8`, `[@clm-tone-intimate-parasocial-address]`);
compassion shares lyric dwelling's contour and care may be suggested rather
than stated (`tones/compassionate.md §6`, `[@clm-dhvani-suggestion-theory]`);
detached alternates plain observed fact with lyrical dwelling, the image
carrying the inference (`tones/detached.md §6`, `tones/detached.md §5` shasei
operator).

**Candor × Structural & Traditional — `re-color` (all three cards).**
The frame carries the address or the register: a dated entry, letter, or final
line fixes the addressee, and in frame-narrative disclosure stays in one layer
(`tones/intimate.md §6`, epistolary note in `tones/intimate.md §6`); a report,
case file, itinerary, or dated entry carries the neutral register
(`tones/detached.md §6`); form rules survive, with a letter or testimony as
compassion's native form (`tones/compassionate.md §6`).

**Candor × Academic (Layer 0) — `alternate` (intimate, compassionate);
`integrate` (detached).**
The evidence contract survives in every row. Positionality frames the argument,
then analysis resumes at low intensity (`tones/intimate.md §6`,
`tones/intimate.md §3`); compassion frames the case and yields at the thesis
(`tones/compassionate.md §6`, `tones/compassionate.md §3`); detached integrates
argument with evidentiary plainness under one invariant — a single accountable
stance, never committee voice (`tones/detached.md §6`,
`tones/detached.md §7` manufactured-neutrality mode,
`[@clm-tone-detached-ai-slop-flatline]`).

**Candor × Blog / marketing (Layer 0) — `re-color` (all three cards).**
The reader promise survives in every row, and each card contributes a shipping
gate to the re-color: for intimate, the §4 manufactured-intimacy line — the
disclosure must cost the discloser (`tones/intimate.md §6`,
`tones/intimate.md §7`, `[@clm-tone-intimate-manufactured-authenticity]`); for
detached, coolness signals confidence only at headline or single-sentence scale
(`tones/detached.md §6`, `tones/detached.md §3`); for compassionate, the
pity-tourism and guilt-manipulation lines (`tones/compassionate.md §6`,
`tones/compassionate.md §4`) — see *compassionate × guilt-managed purchase
copy* below.

### Elevation family + Layer 0 forms

**Elevation × Speculative — `re-color` (all four cards).**
Estrangement and the novum's stakes carry the piece; Elevation contributes
texture only (`tones/inspirational.md §6`; `tones/lyrical.md §6`;
`tones/reverent.md §6`; `tones/warm.md §6`). Inspirational keeps possibility
checkable by tying every forward clause to a route and an agent, so hope inside
a speculative world reads as a novum-shaped solution rather than a wish
(`tones/inspirational.md §2`, §6; `[@clm-tone-inspirational-hope-pathways-agency]`).
Lyrical lets cadence voice the world while refusing to resolve its rules by
music (`tones/lyrical.md §6`; `[@clm-worldbuilding-rules-limits]`). Reverent
may hold an in-world object as sacred without bypassing the world's constraints
(`tones/reverent.md §6`). Warm addresses the reader as a companion while the
world's rules stay unsoftened (`tones/warm.md §6`).

**Elevation × Horror — `re-color`, strict invariants (lyrical, warm — family
default); `alternate`, narrow (reverent); `integrate`, narrow (inspirational).
Flagged: *inspirational × Horror* (seeded), *lyrical × Horror*,
*reverent × Horror*, *warm × Horror*.**
`re-color` with strict engine invariants is the family default — lyrical and
warm both mark this pairing flagged high-tension and bar ornament or
friendliness from making danger feel safe (`tones/lyrical.md §6`;
`tones/warm.md §6`; `[@clm-suspense-vs-surprise]`). **Alternate**, narrow, for
reverent: a bounded reverent passage may frame the object, after which the voice
releases back to the uncanny, and the register drops wherever threat without
fascination appears (`tones/reverent.md §2`, §4, §6;
`[@clm-tone-reverent-sacred-vs-threat-awe]`). **Integrate**, narrow, for
inspirational: uplift survives only as a coda after dread has been honoured,
never over the stakes peak or alongside disclosed harm (`tones/inspirational.md
§4`, §6; `[@clm-tone-inspirational-toxic-positivity-backfire]`). The four
cards assign three different patterns here: the split is recorded, never
averaged — each card's §6 is authoritative for its own tone — and the
card-specific routes are flagged with resolutions under High-tension pairings.

**Elevation × Romance — `integrate` (inspirational, lyrical, warm);
`re-color` (reverent).**
The optimistic arc, the emotional risk, and the bond itself survive
(`tones/inspirational.md §6`; `tones/lyrical.md §6`; `tones/warm.md §6`).
Uplift re-colors the obstacles, never the bond (`tones/inspirational.md §6`);
lyricism re-colors interiority and never substitutes cadence for earned intimacy
(`tones/lyrical.md §6`; `[@clm-character-desire-urgency]`); warmth lives in
narration and secondary voices and never replaces earned intimacy
(`tones/warm.md §6`). Re-color for reverent: reverence may consecrate the bond
but never replace the bond's work (`tones/reverent.md §6`).

**Elevation × Thriller & Mystery — `re-color` (family default: warm
throughout; resolution-only for inspirational and lyrical); `alternate`
(reverent). Flagged: *inspirational × Thriller & Mystery* (seeded), *lyrical ×
Thriller & Mystery*, *reverent × Thriller & Mystery*.**
Jeopardy and the promised resolution survive the whole run; the lift arrives
only after the danger resolves (`tones/inspirational.md §6`) and density yields
through the chase, returning only at the close (`tones/lyrical.md §6`) —
consistent with the peroration finding that the emotional peak lands after the
case is made (`tones/inspirational.md §3`;
`[@clm-tone-inspirational-peroration-late-climax]`). Warm re-colors throughout,
with the cozy variant registering warmth as its sanctioned surface
(`tones/warm.md §6`). Reverent alternates: the full register appears only in a
framed pause and then releases to the pursuit (`tones/reverent.md §6`), dropping
at stakes peaks and at any genuine deadline, which routes to `tone-urgent`
(`tones/reverent.md §3`, §4).

**Elevation × Literary & Realist — `integrate` (all four cards). Flagged:
*warm × Literary & Realist*.**
Interiority and social texture hold; Elevation enters through the situation, not
authorial decoration (`tones/inspirational.md §6`; `tones/lyrical.md §6`;
`tones/reverent.md §6`; `tones/warm.md §6`). Hope must arise from the dramatized
situation and the character's own desire rather than narratorial encouragement
(`tones/inspirational.md §6`; `[@clm-character-desire-urgency]`); lyricism stays
a local register inside the real, governed by psychic distance
(`tones/lyrical.md §6`; `[@clm-point-of-view-psychic-distance]`); the reverent
object must arise from the world rather than authorial decorum
(`tones/reverent.md §6`); companionable narration accompanies but never replaces
a character's suffering — the boundary against `tone-compassionate`
(`tones/warm.md §1`, §6).

**Elevation × Dramatic & Screen — `re-color` (all four cards).**
The scene turn is the engine (`[@clm-scene-turning-points]`;
`tones/inspirational.md §6`; `tones/lyrical.md §6`; `tones/reverent.md §6`;
`tones/warm.md §6`). Inspirational is played through a visible choice rather
than spoken encouragement (`tones/inspirational.md §6`); lyrical cadence lives
in voice-over or image and never stalls visible action (`tones/lyrical.md §6`);
reverent is played through visible gesture and addressed speech
(`tones/reverent.md §6`; `[@clm-tone-reverent-numinous-wholly-other]`); warm
lives in dialogue that carries character, not authorial friendliness
(`tones/warm.md §6`).

**Elevation × Poetic & Lyric — `integrate` (lyrical, reverent, warm);
`alternate` (inspirational).**
Form rules survive — ghazal radif, vachana ankita, pastoral tinai — and the tone
serves the form's engine rather than overriding it (`tones/lyrical.md §6`;
`[@clm-reader-promise]`; `tones/reverent.md §6`; `tones/warm.md §6`). Reverent
keeps the object concrete so cadence and suggestion coexist without flattening
it (`tones/reverent.md §6`); warmth may be suggested rather than stated
(`tones/warm.md §6`; `[@clm-dhvani-suggestion-theory]`). Alternate for
inspirational: lyric dwelling and the forward beat trade dominance by section
across a modulation bridge, because sustained uplift kills cadence unless dosed
as one bounded turn (`tones/inspirational.md §3`, §6;
`[@clm-tone-inspirational-dosage-yield]`).

**Elevation × Structural & Traditional — `re-color` (all four cards).**
Form logic — epistolary, frame, flash, interactive, dastan/katha — survives, and
each tone rides a carrier the form already provides (`tones/inspirational.md §6`;
`tones/lyrical.md §6`; `tones/reverent.md §6`; `tones/warm.md §6`): a dated
entry or closing frame carries inspirational's turn; a letter's cadence or a
frame's refrain carries lyrical's; a liturgical frame, refrain, or closing
invocation carries reverent's; the familiar letter is warm's native form
(`tones/warm.md §6`; `[@clm-tone-warm-companionable-essay-letter]`).

**Elevation × Academic (Layer 0) — `alternate` (lyrical, reverent, warm);
`re-color` (inspirational). Flagged: *inspirational × academic*, *lyrical ×
academic*, *reverent × academic*, *warm × academic*.**
Explicit academic guidance. Tone frames the opening, a key term, or the
transitions and yields at thesis, method, and evidence (`tones/lyrical.md §6`;
`tones/reverent.md §6`; `tones/warm.md §6`), consistent with the evidence
contract and five-tier source hierarchy of `layers/layer0-academic.md`. Specific
yields: lyrical's cadence may fix a key term or a closing idea but must never
make a claim sound truer than its evidence allows — rhyme-as-reason is a named
hazard (`tones/lyrical.md §3`, §4, §6; `[@clm-tone-lyrical-rhyme-truth]`);
reverent's register marks the subject's claim on attention and may not carry
evidentiary weight or the conclusion (`tones/reverent.md §3`, §6), and the
sacred register over a living tradition in a scholarly frame risks
museumification (`tones/reverent.md §4`, §7); warmth frames the opening and
transitions and yields at the thesis, never sitting over an unsupported claim,
because competence must lead under expertise-testing (`tones/warm.md §3`, §6;
`[@clm-tone-warm-warmth-without-substance]`). Pattern `re-color` for
inspirational: the argument and its evidence survive, and uplift frames a
reachable implication without substituting for proof (`tones/inspirational.md
§3`, §6), at a dosage of at most one elevation passage per section
(`tones/inspirational.md §4`; `[@clm-tone-inspirational-dosage-yield]`).

**Elevation × Blog / marketing (Layer 0) — `integrate` (inspirational, warm);
`re-color` (lyrical); `re-color` at most, otherwise not used (reverent).
Flagged: *inspirational × blog / marketing*, *lyrical × blog / marketing*,
*reverent × blog / marketing*, *warm × blog / marketing*.**
Explicit blog/marketing guidance. The reader promise and the checkable takeaway
coexist, both yielding at the call to action (`tones/inspirational.md §6`;
`tones/warm.md §6`), inside the honesty gates of `layers/layer0-blog.md` —
never invent audience research, scarcity, results, or urgency. The gates are
card-enforced: no deadline may be attached to uplift unless the material
establishes it (`tones/inspirational.md §4`;
`[@clm-tone-inspirational-urgency-not-manufactured]`) and sincerity is earned
by substance in every warm beat, never asserted (`tones/warm.md §4`, §6;
`[@clm-tone-warm-warmth-without-substance]`). Pattern `re-color` for lyrical:
music serves one memorable line, yields at the proof and the call to action,
and must never let music imply a fact (`tones/lyrical.md §3`, §6). For reverent
the pattern is `re-color` at most, and the card's default for this form is not
to use the tone at all: consecrate a shared craft or place only, never a product
benefit (`tones/reverent.md §3`, §6;
`[@clm-tone-reverent-failure-borrowed-gravity]`).

## High-tension pairings (capped at 90)

Flagged pairs receive explicit resolution paragraphs: why the pairing is
high-tension and which pattern resolves it. The seeded table below is
established and stays as written; the three tables after it complete the
layer's coverage — sixty flagged pairs against the cap of 90. Pattern cells
name one of the three patterns only. Where a card bars a tone outright over
specific content, the cell names the bounded pattern — `re-color` at most —
and the resolution states the prohibition: the tone is not used there and the
passage runs plain. Seeded rows keep their original wording, word for word;
where a seeded cell reads `avoid`, that is a **pair-level flag, not a fourth
pattern** — the default is not to combine, and any deliberate combination
still resolves through one of the three patterns above.

| Tone | Genre family | Why it is high-tension | Resolution pattern |
|---|---|---|---|
| whimsical | Horror | lightness can deflate dread | re-color with strict engine invariants, or avoid |
| inspirational | Horror | uplift contradicts the genre's promise | avoid, or integrate only in a survival-coda |
| comedic | Horror | humor can cannibalize stakes | integrate (dark comedy) with stakes invariant |
| inspirational | Thriller & Mystery | uplift competes with jeopardy | re-color only at resolution |
| reverent | Satirical-literature (mode) | awe is the mode's target | avoid unless subverting deliberately |
| detached | Romance | neutrality blocks emotional risk | re-color with wide distance only |
| cynical | Romance | distrust undercuts the optimistic arc | re-color for one character's voice only |
| urgent | Poetic & Lyric | deadline pressure fights lyrical dwelling | alternate, not integrate |
| philosophical | Comedy-adjacent Humor tones | abstraction kills timing | alternate, with the humor in the concrete |
| grim | Children-facing copy (any) | bleakness exceeds audience | avoid |

**Additional flagged pairs — Humor and Gravity**

| Tone | Genre family | Why it is high-tension | Resolution pattern |
|---|---|---|---|
| deadpan | Horror | flatness can neutralize the danger it should only frame (`tones/deadpan.md §6`) | `re-color`, strict invariants |
| irreverent | Horror | deflation can level the threat or the victim's fear (`tones/irreverent.md §6`) | `re-color`, strict invariants |
| deadpan | Romance | the flat surface converts the confession to indifference (`tones/deadpan.md §3`, §6) | `re-color` with a named drop |
| deadpan | Victim-suffering reportage (Literary & Realist scope) | flatness over unframed suffering reads as moral vacancy (`tones/deadpan.md §4`, §7) | `integrate` with a borrowed register; otherwise not used |
| whimsical | Live-grief, diagnosis, and stakes-peak content (scope) | the play frame brackets live consequence (`tones/whimsical.md §4`, §7) | `alternate` at peaks; not used over stated live harm |
| irreverent | Held-sacred and live-ritual content (scope) | deflation over a lived sacred appraises as contempt (`tones/irreverent.md §4`, §7) | `re-color` at most — barred while held unironically |
| all four Humor cards | Crisis, bereavement, safety/medical/legal copy (Layer 0 scope) | the benign/play frame cannot be established; each card's §4 prohibits it (`tones/comedic.md §4`, `tones/deadpan.md §4`, `tones/whimsical.md §4`, `tones/irreverent.md §4`) | `re-color` at most — barred outright; these registers run plain |
| deadpan | Blog / marketing (Layer 0) | the tone's surface is indistinguishable from corporate blandness (`tones/deadpan.md §7`) | `re-color` with a load-gate |
| comedic | Academic (Layer 0) | a joke at thesis or definition costs precision and cannot carry the claim (`tones/comedic.md §3`, §6) | `re-color` with hard yields |
| grim, cynical, defiant | Live-grief, memorial, sacred/ritual content (scope) | comfort, irony over pain, and grief-as-subject each break the tone (`tones/grim.md §4`, `tones/cynical.md §4`, `tones/defiant.md §4`) | `re-color` at most for real address — barred; `alternate` for scene content |
| urgent | Horror | alarm without a feasible response converts to avoidance; the clock must not deflate the uncanny (`tones/urgent.md §2`, §6) | `re-color`, strict invariants |
| defiant | Horror | vow-and-vindication endings promise heroism the engine may deny (`tones/defiant.md §3`, §6) | `re-color`, strict invariants |
| urgent | Thriller & Mystery | mystery's retrospective engine resists deadlines (`tones/urgent.md §1`, §6) | `re-color`, prospective present only |
| urgent | Academic (Layer 0) | time-pressure narrows judgment where scholarship models considered judgment (`tones/urgent.md §3`, §6) | `re-color` only where the evidence carries time-stakes; otherwise the deadline claim is not made |
| urgent | Blog / marketing (Layer 0) | the tone's arch-failure meets the layer's never-invent-scarcity rule (`tones/urgent.md §4`, §7) | `re-color` behind the three-part test |
| defiant | Academic (Layer 0) | sustained moral-mandate framing narrows tolerance of counterevidence (`tones/defiant.md §4`, §7) | `re-color` with hard yields and one concession |
| defiant | Blog / marketing (Layer 0) | protest voice on a conversion surface degenerates to slogan (`tones/defiant.md §7`) | `alternate` per post unit |
| comedic × grim | Hybrid briefs ("gallows humor", "darkly comic") | comic distance needs an unpanicked narrator; grim holds affect the surface refuses to name (`tones/comedic.md §2`, `tones/grim.md §1`) | route one primary; `integrate` as dark comedy, `alternate` at peaks |
| irreverent × cynical | Hybrid briefs and neighbor-drift | teasing that never returns to benevolence curdles into distrust (`tones/irreverent.md §1`, §7) | route one primary; `alternate`, never `integrate` |
| urgent × defiant | Hybrid briefs (clockless pressure) | urgency needs a clock; defiance needs an opponent — bolted-on deadlines are drift (`tones/urgent.md §7`, `tones/defiant.md §1`) | route one primary; `alternate`, never a fabricated clock |
| irreverent | Satirical-literature (mode) | rotation supplies no prosecutable case; prosecution leaves the tone (`tones/irreverent.md §1`, §7) | `re-color` under the mode with rotation intact; otherwise the tone is rerouted |

**Additional flagged pairs — Contemplation and Candor**

| Tone | Genre family | Why it is high-tension | Resolution pattern |
|---|---|---|---|
| elegiac | Horror — active-threat scenes | mourning across an active threat kills the promised dread (`tones/elegiac.md §4`, §6) | `alternate` — grief at rest points only; not used where no rest point exists |
| elegiac | Thriller & Mystery — active-threat scenes | a deadline engine and a lament compete for the same clock (`tones/elegiac.md §4`, §6) | `alternate` — backstory and deduction lulls only; not used if the structure never leaves the threat |
| nostalgic | Horror — active-threat scenes | two-position reverie over an active threat kills urgency and can soften dread (`tones/nostalgic.md §4`, §6) | `alternate` — one flight at rest points under the §4 counts; otherwise not used |
| nostalgic | Thriller & Mystery — active-threat scenes | cold-case reverie competes with jeopardy over the active threat (`tones/nostalgic.md §4`, §6) | `alternate` — lulls only, every flight bridged; not used if the act has no lull |
| compassionate | Horror | care for a victim can make the danger feel safe and cannibalize dread (`tones/compassionate.md §6`) | `re-color`, strict invariants; not used if the victim must be made safe |
| reflective | Satirical-literature (mode) | the reflective voice becomes the joke's straight man and the mode takes the mic (`tones/reflective.md §4`, §6) | `re-color` at most — not used unless the brief stages the voice as the mode's object |
| reflective | Safety-critical, instructional, and legal/medical-certainty copy (Layer 0 scope) | provisional modality reads as unreliability exactly where certainty is owed (`tones/reflective.md §4`, §5) | `re-color` at most — barred where certainty is owed |
| nostalgic | Safety, legal, and medical copy (Layer 0 scope) | a looking-back voice reads as unreliability in these registers (`tones/nostalgic.md §4`) | `re-color` at most — barred; the present fact runs plain |
| intimate | Adjudicative, clinical, and authority contexts (scope) | disclosure contradicts the speaker's expected role and refuses the listening intimacy needs (`tones/intimate.md §3`, §4) | `re-color` at most — outright prohibition; not used |
| philosophical | Abstraction-first openings in blog / marketing (Layer 0) | vague-but-impressive abstraction reads as profundity, then as spin (`tones/philosophical.md §4`) | `re-color` from a concrete open; the abstraction-first open is not used |
| detached | Victim-suffering content (atrocity, disaster, reportage scope) | a level voice over suffering can hide an unstated stance (`tones/detached.md §4`, §7) | `integrate` only where the accountable stance is legible; otherwise not used |
| compassionate | Guilt-managed purchase copy (Layer 0 scope) | care performed to move a purchase is pity tourism (`tones/compassionate.md §3`, §4) | `re-color` at most — barred outright; the §4 lines are shipping gates |
| elegiac | Real-bereavement service and condolence messages (scope) | consoling a real person is not this tone's job (`tones/elegiac.md §3`, §4) | `re-color` at most — not used for real address; the card routes condolence to `tone-compassionate` |
| intimate × reflective | Hybrid or confessional-drift requests (tone × tone) | the addressee can silently vanish and the passage changes tone (`tones/intimate.md §7`, `tones/reflective.md §1`) | route one primary; `alternate`, never `integrate` |
| nostalgic | Unexamined era-praise in historical or political material (Literary & Realist scope) | focalized memory drifting into unmarked fact becomes propaganda for an era that never was (`tones/nostalgic.md §4`, §7) | `integrate` with strict invariants; not used where era-praise must stand as narration's fact |

**Additional flagged pairs — Elevation**

| Tone | Genre family | Why it is high-tension | Resolution pattern |
|---|---|---|---|
| inspirational | Academic (Layer 0) | uplift pressures the evidence contract (`tones/inspirational.md §3`, §6) | `re-color` |
| inspirational | Blog / marketing (Layer 0) | forward vector pressures the no-manufactured-urgency rule (`tones/inspirational.md §4`) | `integrate` |
| lyrical | Horror | ornament can make danger feel safe; the card self-flags (`tones/lyrical.md §6`) | `re-color`, strict invariants |
| lyrical | Thriller & Mystery | foregrounded density fights pace (`tones/lyrical.md §2`, §6) | `re-color`, resolution only |
| lyrical | Academic (Layer 0) | cadence can imply facts the evidence has not earned (`tones/lyrical.md §4`) | `alternate` |
| lyrical | Blog / marketing (Layer 0) | music must not imply a fact over evidence-gated claims (`tones/lyrical.md §3`) | `re-color` |
| reverent | Horror | fascination competes with threat; narrow route only (`tones/reverent.md §2`, §6) | `alternate`, narrow |
| reverent | Thriller & Mystery | sacred dwelling competes with jeopardy's clock (`tones/reverent.md §3`, §6) | `alternate` |
| reverent | Academic (Layer 0) | awe cannot carry an argument; museumification risk (`tones/reverent.md §3`, §4) | `alternate` |
| reverent | Blog / marketing (Layer 0) | borrowed gravity over a product — the tone's arch-failure (`tones/reverent.md §4`, §6) | `re-color` at most, otherwise not used |
| warm | Horror | affiliative closeness deflates the uncanny; the card self-flags (`tones/warm.md §6`) | `re-color`, strict invariants |
| warm | Literary & Realist | warmth collapses over a character's real suffering (`tones/warm.md §1`, §7) | `integrate` with a named drop |
| warm | Academic (Layer 0) | warmth without substance reads as pity under scrutiny (`tones/warm.md §2`, §3) | `alternate` |
| warm | Blog / marketing (Layer 0) | brand-voice smarm concentrates exactly at proof and CTA (`tones/warm.md §4`) | `integrate` |

### Resolution paragraphs

**1 · whimsical × Horror — extension of a seeded row.** High-tension because
lightness can deflate the dread the reader was promised, which is why the seed
carries the pair. The seeded options stand, restated in the card's own order —
the tone is not used, else `re-color` with strict engine invariants
(`tones/whimsical.md §6`; the card phrases the bar first, the seed phrases
re-coloring first; the options are identical). The extension adds the placement
rule: whimsy lives only in a safe frame *inside* the horror, never over the
threat (`tones/whimsical.md §6`), and the stakes-trivializing diagnostic decides
it — if the whimsy would tell a person in real distress that their situation is
"just a game," cut the fanciful beat and substitute one concrete, literal
sentence (`tones/whimsical.md §7`,
`[@clm-tone-whimsical-tonal-clash-stakes]`, `tones/whimsical.md §4`).

**2 · inspirational × Horror — extension of a seeded row.** High-tension
because uplift and dread pull the reader's target feeling in opposite
directions, which is why the seed carries the pair. The seeded resolution
stands — `integrate`, narrow: a survival coda after dread has been honoured,
never as a defence against it (`tones/inspirational.md §6`). The extension adds
the card's restraint mechanics: no uplift may run over disclosed harm while the
threat is live (`tones/inspirational.md §4`;
`[@clm-tone-inspirational-toxic-positivity-backfire]`), and any closing lift
still needs a route or a named model rather than a slogan
(`tones/inspirational.md §2`;
`[@clm-tone-inspirational-hope-pathways-agency]`). If those conditions cannot be
met, the seed's alternative stands: the tone is not used.

**3 · comedic × Horror — extension of a seeded row.** High-tension because
humour can cannibalize the stakes the genre promised, which is why the seed
carries the pair. The seeded pattern stands — `integrate` (dark comedy) with a
stakes invariant — and the extension adds the card's mechanics: dread survives
while humour lives only in psychic distance and phrasing (`tones/comedic.md §6`,
`[@clm-tone-comedic-comic-distance]`); at a stakes peak the draft must pass the
bathos diagnostic — does the comic beat release tension prematurely, and does
the piece re-earn the emotion afterward — moving the beat earlier or letting the
serious line stand (`tones/comedic.md §7` bathos mode); and over live harm the
§4 context prohibitions bind absolutely (`tones/comedic.md §4`).

**4 · inspirational × Thriller & Mystery — extension of a seeded row.**
High-tension because uplift competes with jeopardy, which is why the seed
carries the pair. The seeded pattern stands — `re-color`, resolution only:
jeopardy and the promise of resolution survive the entire run, and the lift
arrives after the danger resolves (`tones/inspirational.md §6`). The extension
adds placement and clock discipline: the emotional peak belongs to the
peroration, after the case is made (`tones/inspirational.md §3`;
`[@clm-tone-inspirational-peroration-late-climax]`), and no deadline may
intensify the jeopardy unless the material independently establishes it — a real
clock routes to `tone-urgent` (`tones/inspirational.md §4`;
`[@clm-tone-inspirational-urgency-not-manufactured]`).

**5 · reverent × Satirical-literature (mode) — extension of a seeded row.**
High-tension stands as seeded: awe is the mode's target, so reverence and
critique compete for the same surface. The seeded resolution — the tone is not
used unless the brief subverts deliberately — carries the staging-visible
invariant added here: uplift may be the satire's target but must stay visible as
staging (`tones/inspirational.md §6`); lyrical density may be the object of the
satire, staging staying visible (`tones/lyrical.md §6`); and deliberate parody
stages borrowed gravity visibly, which the card treats as convention rather than
failure (`tones/reverent.md §7`).

**6 · detached × Romance — seeded row.** High-tension because a level neutral
voice blocks the emotional risk the genre exists for: the card's Romance row
holds wide distance with one charged detail per beat reported from outside the
feeling, and never sustains neutrality at the confession, where the emotional
risk must land (`tones/detached.md §6`). Resolution: `re-color` with wide
distance only, as seeded — flatness textures observation and narration, one
charged detail carries each beat, and at the confession the flat beat drops to
plain register under the §4 drop rule (`tones/detached.md §4`).

**7 · cynical × Romance — extension of a seeded row.** High-tension because
distrust undercuts the optimistic arc, which is why the seed carries the pair.
The seeded pattern stands — `re-color` for one character's voice only — and the
card's §6 row states the same rule with its invariant: the bond's sincere beats
stay untouched and the cynic is a character, not the narrative
(`tones/cynical.md §6`). The extension adds the mechanism that makes the
restriction work: every deflating line needs a recoverable prior in the text, so
the arc's sincere claims must survive undeflated
(`[@clm-tone-cynical-irony-echoic]`), and at least one stated motive survives
undeflated per movement (`tones/cynical.md §4`,
`[@clm-tone-cynical-dosage-saturation]`).

**8 · urgent × Poetic & Lyric — extension of a seeded row.** High-tension
because deadline pressure fights the lyric's dwelling, which is why the seed
carries the pair. The seeded pattern stands — `alternate`, never `integrate` —
and the card's §6 row is explicit: resolved by section, never integrated
(`tones/urgent.md §6`, `[@clm-pacing-rhythm-syntax]`). The extension adds
dosage placement: the urgent spike is bounded — at most one spike per ~1,200
words with the strongest markers at a single decision point — so the lyric
movement owns everything around it (`tones/urgent.md §4`,
`tones/urgent.md §3`), and the bridge must be a concrete event, not a mood
shift (modulation rules above).

**9 · philosophical × comedy-adjacent Humor tones — extension of a seeded
row.** High-tension because abstraction kills timing, which is why the seed
carries the pair; its resolution stands — `alternate`, with the humor in the
concrete — and the extension adds the Humor side's own anchors. Each Humor card
supplies the concrete floor the alternation needs: comedic stages low-register
concrete images against high subjects so setup and turn stay picturable
(`tones/comedic.md §5`); deadpan needs loaded *content* for the flat surface to
contradict — abstraction opens no gap (`tones/deadpan.md §1`,
`[@clm-tone-deadpan-flatness-failure]`); whimsical requires at least one
ordinary, true, or concrete element per fanciful flight (`tones/whimsical.md §4`,
`[@clm-tone-whimsical-nonsense-sense-tension]`); irreverent must name the
elevated register each beat knocks down in one noun phrase — abstraction offers
no ceremony to collapse (`tones/irreverent.md §1` recognition test,
`tones/irreverent.md §5`).

**10 · grim, with cynical added, × children-facing copy — extension of a
seeded row.** High-tension because bleakness exceeds the audience; the seed's
resolution stands — the tone is not used, and the card reinforces it twice:
children-facing copy of any kind is a §4 context prohibition
(`tones/grim.md §4`), and the §6 cross-cutting note bars re-coloring the pairing
at all (`tones/grim.md §6`). The extension adds a second tone to the seeded
surface: cynical's §4 context prohibitions independently bar children-facing
copy (`tones/cynical.md §4`), so the row now covers both Gravity cards that
prohibit it. Precision note: this flag does not generalize across families —
whimsical explicitly permits children-facing copy at high cute-surface density
because illustrations supply the prop (`tones/whimsical.md §7`).

**11 · deadpan × Horror.** High-tension because the same flat surface that can
amplify the uncanny can also neutralize the danger it should only frame — the
card's Horror row demands dread, threat, and the payoff survive and forbids
neutralizing the danger (`tones/deadpan.md §6`). Over horror's atrocity beats
the tension sharpens: recording suffering without a borrowed institutional
frame reads as moral vacancy (`tones/deadpan.md §4` ethical bounds,
`tones/deadpan.md §7` target-loss mode). Resolution: `re-color` with strict
invariants — flatness is anchored to a named register (case file, memo,
dispatch) so the echo does the indicting work
(`[@clm-tone-deadpan-clinical-reportage]`), one early incongruity keys the
frame (`tones/deadpan.md §4`,
`[@clm-tone-deadpan-literal-read-failure]`), and the beat drops at any stakes
peak where the reader needs a stated reaction (`tones/deadpan.md §4`).

**12 · irreverent × Horror.** High-tension because the leveling texture can
land on the danger or on the victim's fear instead of the pomp — the card's
own Horror row is strict: a pompous institution inside the horror may be
leveled, never the danger or the victim's fear (`tones/irreverent.md §6`). Over
live dread the license is fragile: where the benign frame cannot be built,
deflation registers as contempt, and negativity dominance magnifies the failed
reading (`tones/irreverent.md §4`,
`[@clm-tone-irreverent-benign-violation-register]`). Resolution: `re-color`
with strict invariants — the engine's dread, threat, and payoff survive
(`[@clm-reader-promise]`); targets are in-world offices and ceremonies only;
and at the stakes peak the tone yields to one plain, literal line before any
resumption (`tones/irreverent.md §4`,
`[@clm-tone-irreverent-licensed-frame]`).

**13 · deadpan × Romance.** High-tension because the flat surface converts the
beat the genre exists for into indifference: deadpan never lands on the
confession — that beat yields to plain speech (`tones/deadpan.md §6`) — and
"incompatible at the emotional peak; the flat surface converts grief into
indifference" is the card's own purpose rule (`tones/deadpan.md §3`). Distinct
from the seeded *detached × Romance* pairing — a different card with a
different mechanism (neutral observation vs the loaded-content gap).
Resolution: `re-color` with a named drop — flatness textures obstacles,
procedure, and narration, while the confession beat and the bond's emotional
risk run plain (`tones/deadpan.md §6`, `tones/deadpan.md §4` drop rule), or the
moment becomes the piece's single frame break and the flat surface resumes
afterward (`tones/deadpan.md §4`).

**14 · deadpan × victim-suffering reportage (Literary & Realist scope).**
High-tension because suffering recorded without an institutional or absurd
frame replicates the atrocity instead of indicting it — flatness reads as moral
vacancy, the card's target-loss failure (`tones/deadpan.md §7`), with the §4
ethical bound stating the same rule for documentary, disaster, and conflict
material. Resolution: `integrate` only where the flatness is anchored to a
named borrowed register so the echo does the satiric work
(`tones/deadpan.md §5` reportage attribution,
`[@clm-tone-deadpan-clinical-reportage]`), with the real term always recoverable
(`tones/deadpan.md §5`); otherwise the tone is not used. Sustained unframed
flatness across the suffering is never the resolution. Related, not duplicated:
*detached × victim-suffering content* governs `tone-detached` over the same
content by a different mechanism.

**15 · whimsical × live-grief, diagnosis, and stakes-peak content (scope).**
High-tension because the play frame brackets consequence, and applied to genuine
stakes it reads as denial or emotion invalidation — the card's
stakes-trivializing failure, with the rhetorical cousin of toxic positivity
named (`tones/whimsical.md §7`,
`[@clm-tone-whimsical-tonal-clash-stakes]`), and the §4 context prohibitions
bar the tone outright over death, bereavement, live grief, crisis messages, and
any harm the reader is presently suffering. Resolution: the tone is not used
wherever the text states a live harm directly; inside fiction with stakes peaks,
`alternate` — drop to a plain or concrete register at the peak and let the
fanciful texture return only after the bridge (`tones/whimsical.md §4`,
`tones/whimsical.md §9` exercise 3). The §6 Literary `alternate` row still
governs texture elsewhere; it never licenses play over the peak.

**16 · irreverent × held-sacred and live-ritual content (scope).**
High-tension because where the subject is someone's lived sacred — grief, a
ritual that matters to a participant — deflation appraises as real contempt
rather than teasing, and the benign frame cannot be built
(`tones/irreverent.md §7` mode 4 Scope, the
lived-sacred line, `tones/irreverent.md §4`,
`[@clm-tone-irreverent-benign-violation-register]`); one failed breach sticks
because negativity asymmetry magnifies the contempt reading
(`tones/irreverent.md §7`,
`[@clm-tone-irreverent-licensed-frame]`). Resolution: `re-color` at most — the
tone is not used while a person in-scene holds the sacred without irony; the
beat runs plain, then the leveling resumes only after the scene re-licenses it
(`tones/irreverent.md §4` substitutions); alternatively rotate the target to an
elevated register the scene itself puts on ceremony (`tones/irreverent.md §5`,
`[@clm-tone-irreverent-no-sustained-target]`).

**17 · Humor family × crisis, bereavement, and safety/medical/legal copy
(Layer 0 scope).** High-tension because all four cards independently prohibit
these contexts by the same mechanism: the benign or play frame cannot be
established there, so the tone converts to harm — comedic over death,
bereavement, live grief, crisis, and instruction the reader must act on
literally (`tones/comedic.md §4`); deadpan over crisis, safety, medical, legal,
bereavement, and live-harm content (`tones/deadpan.md §4`); whimsical where the
play frame cannot be made safe and converts to trivialization
(`tones/whimsical.md §4`, `[@clm-tone-whimsical-tonal-clash-stakes]`);
irreverent where deflation without a benign frame registers as contempt
(`tones/irreverent.md §4`,
`[@clm-tone-irreverent-benign-violation-register]`). Resolution: `re-color` at
most — barred outright; these registers run plain. This is a surface
prohibition, not a softer pattern. Scope note: the *reflective × safety-critical*
and *nostalgic × safety, legal, and medical copy* entries flag the same surfaces
for other families; no tone overlaps this entry.

**18 · deadpan × blog / marketing (Layer 0).** High-tension because the tone's
required surface — neutral, hedged, institutional prose — is exactly the
surface the form rejects when it is not loaded: adopting deadpan's surface with
no absurdist content produces lifeless marketing copy, the card's
corporate-blandness failure (`tones/deadpan.md §7`,
`tones/deadpan.md §6`), an entry the card marks tier 4–5 in basis and never
sole support. Resolution: `re-color` behind a load-gate — every flat beat sits
on loaded content, with one unmistakable incongruity early so single-pass
readers infer the frame (`tones/deadpan.md §4`,
`[@clm-tone-deadpan-literal-read-failure]`), yield at the CTA and the promised
takeaway (`tones/deadpan.md §6`), and where the content will not load, switch
deliberately to plain exposition rather than running flat
(`tones/deadpan.md §7`).

**19 · comedic × academic (Layer 0).** High-tension because a joke placed at
the load-bearing points buys attention and costs precision — yield at the
thesis and at definitions (`tones/comedic.md §3`) — and comedy's persuasive
effect is small and condition-dependent, so the tone may never be promised to
carry the argument (`tones/comedic.md §6`,
`[@clm-tone-comedic-superiority-limits]`); over-dense comic detail further
depresses comprehension and transfer even when readers enjoy it
(`tones/comedic.md §4`,
`[@clm-tone-comedic-density-saturation]`). Resolution: `re-color` with hard
yields — the argument, evidence contract, and thesis survive; one sustained
comic passage sits inside the 900–1,500-word band away from the thesis
(`tones/comedic.md §4`); the joke illustrates the claim and never substitutes
for it or for the proof (`tones/comedic.md §6`,
`layers/layer0-academic.md` evidence contract).

**20 · grim, cynical, and defiant × live-grief, memorial, sacred/ritual
content (scope).** High-tension because each card independently breaks over
this content: grim over comfort is cruelty and over the sacred is desecration,
with §4 barring direct address of a reader's fresh grief and sacred or ritual
moments (`tones/grim.md §4`); cynical's bitter irony over real pain reads as
cruelty, and memorials, elegies, and sacred or ritual moments are §4 context
prohibitions (`tones/cynical.md §4`); defiant may never run where the subject
is one's own grief and where the only constraint is a clock rather than a
power (`tones/defiant.md §4`). Resolution: `re-color` at most where the piece
must address real grief or a real memorial service — barred there, the passage
runs plain — and `alternate` where grief or ritual appears as *scene content*
inside a piece routed to one of these tones: by section with a bridge, the
yield beat runs plain (concrete consequence, plain fact, named witness:
`tones/grim.md §4` substitutions; the institution's own record or one unironic
line: `tones/cynical.md §4` substitutions; evidence, concession, or appeal:
`tones/defiant.md §4` substitutions), not a second tone card. Distinct from
*elegiac × real-bereavement and condolence messages*: different tones,
different mechanisms.

**21 · urgent × Horror.** High-tension because the two mechanisms conflict at
the root: horror's engine withholds control, while urgent's alarm motivates
protective action only when the reader perceives an effective, feasible
response — without one the same alarm yields defensive avoidance or denial
(`tones/urgent.md §2`,
`[@clm-tone-urgent-efficacy-gate]`) — and the row's own invariant says the
deadline is a human clock that must not deflate the uncanny
(`tones/urgent.md §6`, `[@clm-suspense-vs-surprise]`). Resolution: `re-color`
with strict invariants: the dread curve and the threat own the reader-state;
the clock exists only as a character-level countdown inside the fiction, never
as alarm-narration addressed over the uncanny (`tones/urgent.md §6`); where the
horror structurally offers no feasible action, the urgent voice drops for plain
consequence (`tones/urgent.md §4` substitutions) rather than converting to
avoidance (`tones/urgent.md §7` efficacy mode).

**22 · defiant × Horror.** High-tension because defiance's own machinery
promises what horror may deny: endings close on vow, pledge, or anticipated
vindication (`tones/defiant.md §3`), and reactance craft asks for a freedom
voiced and restored (`[@clm-tone-defiant-reactance-restoration]`), while the
card's Horror row forbids promising heroism the horror engine denies or
deflating the uncanny (`tones/defiant.md §6`). Resolution: `re-color` with
strict invariants — resistance textures a character's voice against a named
power, the warrant is tested by cost so the piece can end unvindicated
(`tones/defiant.md §6` Literary invariant, `tones/defiant.md §4`), and the
defiant beat drops at the stakes peak to unadorned fact or the engine's own
dread (`tones/defiant.md §4` substitutions). If the piece needs the defiance to
*win*, the structure is not horror — route the engine, not the tone.

**23 · urgent × Thriller & Mystery.** High-tension because suspense is a
reader-state engine produced by asymmetric information that the tone may color
but never claims, while mystery's retrospective engine resists deadlines
outright (`tones/urgent.md §1`, `tones/urgent.md §6`,
`[@clm-suspense-vs-surprise]`); a bolted-on clock also risks the card's
genre-overlap drift, where the reader is promised one feeling and delivered
another (`tones/urgent.md §7`). Resolution: `re-color`, prospective present
only — urgency voices the human clock where the danger is still ahead
(`tones/urgent.md §6`), suspense owns the reader-state throughout
(`tones/urgent.md §1`), and the retrospective deduction beats run plain with
no manufactured deadline (`tones/urgent.md §6`,
`[@clm-tone-urgent-manufactured-urgency-line]`). Contrasting invariant:
grim's `re-color` in the same row serves the looming engine rather than
fighting it (`tones/grim.md §6`, `[@clm-tone-grim-dread-looming]`).

**24 · urgent × academic (Layer 0).** High-tension because the card itself
calls it a register mismatch: the tone registers only when the evidence
carries time-stakes (`tones/urgent.md §6`, `tones/urgent.md §3`), and the
mechanism it runs on — time pressure narrowing attention and hastening
commitment to an early judgment — works against the considered judgment an
academic argument models (`[@clm-tone-urgent-time-pressure-narrows-cognition]`)
while the L0 evidence contract requires consequential claims narrowed to
available support (`layers/layer0-academic.md`). Resolution: `re-color` only
where the evidence itself carries a named, non-resetting time-bound gap and
the cost of delay is verifiable (`tones/urgent.md §6`,
`tones/urgent.md §4` three-part test); otherwise the deadline claim simply is
not made, and the argument runs plain.

**25 · urgent × blog / marketing (Layer 0).** High-tension because this
surface concentrates the tone's arch-failure: fabricated deadlines, inflated
consequences, and pressure with no real action — manufactured urgency — against
a form that forbids inventing scarcity and forbids hooks that manufacture
urgency the body cannot deliver (`tones/urgent.md §4`,
`tones/urgent.md §7` manufactured-urgency mode,
`[@clm-tone-urgent-manufactured-urgency-line]`, `layers/layer0-blog.md`
never-invent rule). Resolution: `re-color` behind the §4 three-part test as
a shipping gate — a real, non-resetting deadline; a verifiable,
non-inflated consequence; and a feasible action (`tones/urgent.md §4`), with
the alarm paired with efficacy or dropped (`[@clm-tone-urgent-efficacy-gate]`)
and the promised takeaway stated plainly after the spike
(`tones/urgent.md §6`). Adjacent, not duplicated: *inspirational × blog /
marketing* governs inspirational's forward vector on the same surface by a
different card mechanism.

**26 · defiant × academic (Layer 0).** High-tension because sustained
moral-mandate framing narrows tolerance of dissenters and trust in authorities
(`[@clm-tone-defiant-moral-conviction]`), and the card forbids running the
defiant register over the decisive counterargument when addressing the
undecided — argument addressed to the undecided may not sustain absolutism
(`tones/defiant.md §4`, `tones/defiant.md §7` absolutism mode), precisely the
reader an academic argument addresses. Resolution: `re-color` with hard
yields — the claim stays grounded in a named warrant while method, evidence,
and counterevidence run plain (`tones/defiant.md §6`,
`layers/layer0-academic.md`), and after every defiant beat the draft returns to
evidence and inserts one concession (`tones/defiant.md §4` dosage rule,
`[@clm-tone-defiant-dosage-yield]`, `[@clm-controlling-idea]`). Sloganeering
substitutions never carry a claim (`tones/defiant.md §3`).

**27 · defiant × blog / marketing (Layer 0).** High-tension because protest
voice on a conversion surface degenerates exactly where the form is judged:
injustice framing without efficacy, route, or a concrete "we" leaves the reader
angry and inert — a slogan, not rhetoric (`tones/defiant.md §7` sloganeering
mode, `[@clm-tone-defiant-slogan-stakes]`) — and controlling imperatives turn
the reader's reactance back on the writer
(`[@clm-tone-defiant-dosage-yield]`), while `layers/layer0-blog.md` requires
the hook to lead honestly and consequential claims to carry evidence.
Resolution: `alternate` per post unit (the card's own §6 pattern): each
unit names power, stake, and one feasible route, then the piece returns to the
plain promise and literal CTA (`tones/defiant.md §6`,
`tones/defiant.md §4`), at most one sustained defiant beat per section and no
reader-commanding imperatives outside quoted speech (`tones/defiant.md §4`,
`tones/defiant.md §7`).

**28 · comedic × grim — hybrid briefs ("gallows humor", "darkly comic").**
High-tension because the alias table routes these briefs to comedic with a
"grim stakes (integration)" tension (`tones/_index.md` alias resolution), yet
the two cards' mechanisms pull opposite: comic distance requires the narrator
unpanicked, emotion in the narrator being laughter's enemy
(`tones/comedic.md §2`,
`[@clm-tone-comedic-comic-distance]`), while grim carries affect *held* — a
pressure the surface refuses to name, weight with no ironic edge
(`tones/grim.md §1`). Resolution: route one primary under the one-primary-tone
rule (the alias table resolves to comedic plus a named tension), then
`integrate` as dark comedy under comedic's Horror-row invariants — dread and
stakes survive, humour lives in distance and phrasing (`tones/comedic.md §6`)
— and `alternate` at stakes peaks, where the comic beat yields and grim weight
stands unqualified (`tones/comedic.md §4` yield rule, `tones/grim.md §4`
interlude rule). Never two tone cards loaded (one-primary-tone rule above).

**29 · irreverent × cynical — hybrid briefs and neighbor-drift.**
High-tension because the two voices differ by one observable the draft can
silently lose: irreverence teases from inside a shared frame and still likes
what it levels, while cynical distrusts and never returns to benevolence
(`tones/irreverent.md §1`), and the card names the exact drift — distance that
never returns to benevolence *becomes* `tone-cynical`
(`tones/irreverent.md §7` neighbor-drift mode,
`[@clm-tone-irreverent-no-sustained-target]`,
`[@clm-tone-irreverent-co-conspirator-distance]`). Resolution: route one
primary through the alias table (cheeky/impious → irreverent; sardonic,
bitter, jaded → cynical; `tones/_index.md` alias resolution) — where both
appear across a piece, `alternate` by section with a bridge and a reason,
never `integrate`: the drift diagnostic is whether the voice still likes
anything (`tones/irreverent.md §7`), and the cynic's own diagnostic is whether
a stated claim survives undeflated (`tones/cynical.md §1`).

**30 · urgent × defiant — hybrid briefs (clockless pressure).**
High-tension because the two are separated by one observable: urgency is
bounded by a clock and defiance is bounded by an opponent — if the pressure
survives with no deadline attached, the piece has written defiance, and where
the constraint really is time, the route is urgent (`tones/defiant.md §1`,
`tones/urgent.md §1`). The card documents the failure directly: urgency
standing in for a clockless opposition — a defiant manifesto with a fake
midnight deadline bolted on — reads as drift, not modulation
(`tones/urgent.md §7` genre-overlap mode). Resolution: route one primary
by whether a real clock exists, the urgent route then passing the §4
three-part test (`[@clm-tone-urgent-manufactured-urgency-line]`); where both
genuinely appear across a piece, `alternate` by section with a bridge —
never `integrate`, and never a fabricated deadline to fake the clock
(`tones/urgent.md §4`, `tones/defiant.md §4`).

**31 · irreverent × Satirical-literature (mode).** High-tension because the
mode and the tone want incompatible things from the same surface: satire fixes
a target and prosecutes it through structure and critique, while irreverence
levels whatever register is elevated *here*, rotating so no case accumulates,
and supplies no program (`tones/irreverent.md §1`,
`[@clm-tone-irreverent-no-sustained-target]`); when one fixed target plus an
accumulating argument takes over, the piece has left the tone for the mode —
the card's satire-creep drift (`tones/irreverent.md §7`). Resolution:
`re-color` where the mode owns the structural critique and irreverence
supplies only texture with rotation intact (`tones/irreverent.md §6`
cross-cutting note); otherwise the tone is rerouted — the voice leaves
irreverence wherever the narrator must prosecute the same target beat by beat
(`tones/irreverent.md §1` recognition test). This is a mode row following the
seed table's mode-row convention; satirical-literature is not a family.
Distinct from the seeded *reverent × Satirical-literature* pairing, which
carries its own extension.

**32 · elegiac × Horror — active-threat scenes.** High-tension because
mourning running across an active threat kills the dread the reader was
promised — the card states it directly: do not run this tone over
active-threat content, it kills urgency (`tones/elegiac.md §4`), and its §6
high-tension note flags the pairing itself (`tones/elegiac.md §6`). Resolution:
`alternate` — grief at rest points only (approach, coda, the counter-register
recesses required by `[@clm-tone-elegiac-oscillation-dosage]`), with the scare
owning every peak — and the tone is not used where the structure offers the
lament no rest point. The §6 Horror `re-color` row still governs texture in
the ruin; it never licenses a lament across the scare.

**33 · elegiac × Thriller & Mystery — active-threat scenes.** High-tension
because a deadline engine and a lament in the same beat compete for the same
clock; elegy over active-threat or urgent-action content is flagged in the
card (`tones/elegiac.md §6` high-tension note, `tones/elegiac.md §4`).
Resolution: `alternate` — elegy owns backstory and deduction lulls only
(`tones/elegiac.md §6` Thriller row), with a concrete-event bridge back to
jeopardy; not used if the structure never leaves the threat.

**34 · nostalgic × Horror — active-threat scenes.** High-tension because a
two-position reverie over an active threat both kills urgency and can soften
dread with a familiar, corrupted past; the card flags nostalgic ×
active-threat content as high-tension (`tones/nostalgic.md §6`,
`tones/nostalgic.md §4`). Resolution: `alternate` — one flight at rest points
only under the §4 counts (one dominating passage, counter-register within the
page, `[@clm-tone-nostalgic-mixed-valence-dailylife]`) — and the tone is not
used where the threat never rests. The §6 `re-color` (a lost past haunting the
approach or coda) applies only where no threat is active.

**35 · nostalgic × Thriller & Mystery — active-threat scenes.** High-tension
because the return-to-hometown or cold-case reverie competes with jeopardy the
moment it runs over the active threat; flagged in the card
(`tones/nostalgic.md §6` high-tension note, `tones/nostalgic.md §4`).
Resolution: `alternate` — backstory and deduction lulls only
(`tones/nostalgic.md §6` Thriller row), every flight entered through a
concrete scene-level cue (`tones/nostalgic.md §5`) and bridged back; not used
if the act has no lull.

**36 · compassionate × Horror.** High-tension because care for a victim can
make the danger feel safe and cannibalize dread — the card's own row reads
"re-color, strict invariants … flagged high-tension" (`tones/compassionate.md
§6`). Resolution: `re-color` with strict invariants — dread and the uncanny
survive, the victim's suffering never softens the threat's plausibility, and
the tone drops to the engine at the stakes peak (`tones/compassionate.md §4`;
the front-matter engine note forbids manufacturing redemption). If the piece
needs the victim made safe, the tone is not used instead.

**37 · reflective × Satirical-literature (mode).** High-tension because when
the engine is comedy about introspection itself, the reflective voice becomes
the joke's straight man and the mode takes the mic (`tones/reflective.md §6`
mode note; `tones/reflective.md §4` peaks-and-modes prohibition). Resolution:
`re-color` at most — the reflective voice is not used unless the brief
deliberately stages the voice as the mode's object. This is a mode row,
following the seed table's mode-row convention; satirical mode is not a family.

**38 · reflective × safety-critical, instructional, and legal/medical-certainty
copy (Layer 0 scope).** High-tension because provisional modality — "perhaps,"
"it seemed" — reads as unreliability exactly where certainty is owed
(`tones/reflective.md §4` context prohibitions; the provisional-modality
operator of `tones/reflective.md §5`). Resolution: `re-color` at most — the
tone is not used where certainty is owed; the card routes the passage to
`tone-detached` when the reader needs observation rather than interiority
(`tones/reflective.md §4`).

**39 · nostalgic × safety, legal, and medical copy (Layer 0 scope).**
High-tension because a looking-back voice reads as unreliability in precisely
these registers (`tones/nostalgic.md §4` context prohibitions). Resolution:
`re-color` at most — the tone is not used in these registers; the present fact
runs plain and the then/now shuttle has no licence there.

**40 · intimate × adjudicative, clinical, and authority contexts (scope).**
High-tension because disclosure that contradicts the speaker's expected role
loses the audience, and the card states an outright prohibition — never in
adjudicative, clinical, or authority contexts (`tones/intimate.md §4`,
`[@clm-tone-intimate-disclosure-risk-boundaries]`); a reader primed to
adjudicate also refuses the listening role that intimacy requires
(`tones/intimate.md §3`). Resolution: `re-color` at most — the tone is not
used in these contexts.

**41 · philosophical × abstraction-first openings in blog / marketing copy
(Layer 0 scope).** High-tension because vague but impressive abstraction is
read as profundity whether or not an idea is present, and depth performance
then reads as spin (`tones/philosophical.md §4`,
`[@clm-tone-philosophical-pseudo-profundity]`); the card prohibits opening
copy or a platform post on an abstraction the reader has no stake in
(`tones/philosophical.md §4`). Resolution: `re-color` from a concrete start —
the abstraction-first open is not used; start from a concrete instance (the
concrete-then-fade floor, `tones/philosophical.md §4`) and then re-color per
§6 with one grounded idea and a portable close.

**42 · detached × victim-suffering content (atrocity, disaster, reportage
scope).** High-tension because a perfectly level voice over someone's suffering
can hide an unstated stance — manufactured neutrality — and the card prohibits
rendering a victim's suffering without an inferable moral footing
(`tones/detached.md §4`; accountability test in `tones/detached.md §7`).
Resolution: `integrate` only where the accountable stance is legible in event
order, consequence, want and cost (`tones/detached.md §6` Literary row,
`[@clm-tone-detached-restraint-vs-absence]`); otherwise the tone is not used.
Sustained flatness across the suffering is never the resolution. Related, not
duplicated: *deadpan × victim-suffering reportage* governs `tone-deadpan` over
the same content by a different mechanism.

**43 · compassionate × guilt-managed purchase copy (Layer 0 scope).**
High-tension because care performed to move a purchase is pity tourism wearing
craft's clothes; the card prohibits managing a purchase through guilt and bars
performing care to move a sale (`tones/compassionate.md §4` context
prohibitions, `tones/compassionate.md §3` blog row,
`[@clm-tone-compassionate-saviorism-witness-ethics]`). Resolution: `re-color`
at most — the tone is not used: the §6 Blog row's pity-tourism and
guilt-manipulation lines are shipping gates, not a softer pattern.

**44 · elegiac × real-bereavement service and condolence messages (scope).**
High-tension because consoling a real person is not this tone's job — the card
routes condolence to `tone-compassionate` as primary and flags service-message
use of elegy (`tones/elegiac.md §4` context prohibitions,
`tones/elegiac.md §3` blog row). Resolution: `re-color` at most — the tone is
not used for real address; only when the brief explicitly asks for
condolence-as-lament does elegiac stand, and then the §4 ending-posture gate
still binds.

**45 · intimate × reflective — hybrid or confessional-drift requests (tone ×
tone).** High-tension because the two voices are separated by one observable —
the addressee — and a piece can silently lose it: if the addressee vanishes the
passage is reflective, not intimate (`tones/intimate.md §7`
confessional-drift diagnostic), and reflective flags the same crossing as a
watch line — disclosure-for-relationship versus a question being worked
(`tones/reflective.md §1`). Resolution: `alternate`, never `integrate` — route
one primary tone under the one-primary-tone rule ("confessional, vulnerable"
→ intimate; "introspective, journal-like" → reflective, alias rows in
`tones/_index.md`), and where both appear across a piece, alternate by
section with a bridge and a reason: intimate sections keep the addressee,
reflective sections work the question (`tones/intimate.md §7` scope line).

**46 · nostalgic × unexamined era-praise in historical or political material
(Literary & Realist scope).** High-tension because idealization that drifts
from focalized memory into unmarked fact becomes propaganda for an era that
never was — sepia-wash at sentence level, restorative hardening at program
level (`tones/nostalgic.md §7`,
`[@clm-tone-nostalgic-rosey-retrospection]`,
`[@clm-tone-nostalgic-restorative-reflective]`). Resolution: `integrate` with
strict invariants — focalized idealization ("I thought then") plus at least one
puncture complicating the golden then per sustained passage
(`tones/nostalgic.md §4` puncture rule) — and the tone is not used wherever
era-praise must stand as narration's fact.

**47 · inspirational × academic (Layer 0).** High-tension because uplift
pressures the evidence contract of `layers/layer0-academic.md`, where
consequential claims are narrowed to available support, while the tone's
register asserts possibility. It resolves by `re-color`: the argument and its
evidence survive, and the tone frames a reachable implication without
substituting for proof (`tones/inspirational.md §3`, §6), held to at most one
elevation passage per section (`tones/inspirational.md §4`;
`[@clm-tone-inspirational-dosage-yield]`).

**48 · inspirational × blog / marketing (Layer 0).** High-tension because the
forward vector and the call to action pull toward invented scarcity and
deadlines, which `layers/layer0-blog.md` forbids outright (never invent
audience research, product performance, scarcity, or results; avoid deceptive
urgency). It resolves by `integrate`: the reader promise and the checkable
takeaway coexist, the tone yields at the CTA, and any deadline must be
established by the material (`tones/inspirational.md §4`, §6;
`[@clm-tone-inspirational-urgency-not-manufactured]`). Over a reader in acute
distress the uplift drops entirely (`tones/inspirational.md §4`;
`[@clm-tone-inspirational-toxic-positivity-backfire]`).

**49 · lyrical × Horror.** High-tension because foregrounded ornament and
cadence can make danger feel safe and can move attention from the threat to the
language — the card itself marks the pairing flagged (`tones/lyrical.md §6`;
purple test `[@clm-tone-lyrical-purple-prose-failure]`). It resolves by
`re-color` with strict invariants: dread survives; cadence may mount the
uncanny, but density yields at the scare itself — bracket the peak, do not
occupy it (`tones/lyrical.md §4`, §6; `[@clm-suspense-vs-surprise]`).

**50 · lyrical × Thriller & Mystery.** High-tension because foregrounding
deliberately slows reading (`tones/lyrical.md §2`;
`[@clm-tone-lyrical-foregrounding-affect]`) while jeopardy depends on pace. It
resolves by `re-color`, resolution only: density yields through the chase and
may return at the close (`tones/lyrical.md §6`), after the action and
informational peaks where the card directs the tone to be dropped
(`tones/lyrical.md §4`).

**51 · lyrical × academic (Layer 0).** High-tension because patterned sound
raises perceived truth independent of evidence — rhyme-as-reason, a named hazard
in the card (`tones/lyrical.md §4`; `[@clm-tone-lyrical-rhyme-truth]`) — which
is exactly what `layers/layer0-academic.md`'s evidence contract prohibits. It
resolves by `alternate`: cadence frames an opening or a close and yields at
thesis, method, and data (`tones/lyrical.md §3`, §6). A cadenced line may fix a
key term in memory; it may never carry a claim.

**52 · lyrical × blog / marketing (Layer 0).** High-tension because
`layers/layer0-blog.md` requires direct, suitable evidence for claims affecting
money, health, reputation, rights, or purchase, while music can make a line
feel proven. It resolves by `re-color`: music serves one memorable line, yields
at the proof and the call to action, and must never let music imply a fact
(`tones/lyrical.md §3`, §6; rhyme-as-reason guard
`[@clm-tone-lyrical-rhyme-truth]`).

**53 · reverent × Horror.** High-tension because fascination with the object
and the genre's threat engine pull in opposite directions: threat-based awe is
not reliably prosocial, and submission without fascination is the boundary
signal where the voice slides toward grim or horror (`tones/reverent.md §2`,
§4; `[@clm-tone-reverent-sacred-vs-threat-awe]`). It resolves by `alternate`,
narrow — a framed reverent passage around the object, then release back to the
uncanny (`tones/reverent.md §6`) — with the register dropped wherever danger or
loss must be felt unadorned (`tones/reverent.md §4`).

**54 · reverent × Thriller & Mystery.** High-tension because sacred dwelling
competes with jeopardy's clock, and the card routes real deadlines to
`tone-urgent` rather than to awe (`tones/reverent.md §3`). It resolves by
`alternate`: the full register appears only in a framed pause, then releases
to the pursuit (`tones/reverent.md §6`), and it drops at stakes peaks and at
any genuine deadline (`tones/reverent.md §4`), dosed to a bounded reverent
passage per section (`tones/reverent.md §4`;
`[@clm-tone-reverent-dosage-yield]`).

**55 · reverent × academic (Layer 0).** High-tension because awe cannot carry
an argument's evidentiary burden — the academic row of the card bars the tone
from doing the work of proof (`tones/reverent.md §3`) — and elevated register
over a living tradition in a scholarly frame risks museumification
(`tones/reverent.md §4`, §7). It resolves by `alternate`: the register marks
the subject's claim on attention and never the conclusion (`tones/reverent.md
§6`); method, evidence, and counterevidence run plain per
`layers/layer0-academic.md`.

**56 · reverent × blog / marketing (Layer 0).** High-tension because this
pairing concentrates the tone's arch-failure: devotion's register imported over
a product, brand, or conversion goal (`tones/reverent.md §4`;
`[@clm-tone-reverent-failure-borrowed-gravity]`) — named the cardinal failure
for this form in the card's form table (`tones/reverent.md §3`). It resolves by
`re-color` at most, with the card's default being not to use the tone in this
form: consecrate a shared craft or place only, never a product benefit
(`tones/reverent.md §6`); if the object cannot justify sacred attention, strip
the register to plain description (`tones/reverent.md §4`).

**57 · warm × Horror.** High-tension because affiliative closeness deflates
the uncanny and makes danger feel safe; the card itself marks the pairing
flagged high-tension (`tones/warm.md §6`; `[@clm-suspense-vs-surprise]`), and
warm's benign frame fails in crisis contexts (`tones/warm.md §4`). It resolves
by `re-color` with strict invariants: dread survives; warmth lives in a
character's voice or a brief narrator aside away from the threat, and yields at
the stakes peak to an unadorned declarative (`tones/warm.md §4`, §6).

**58 · warm × Literary & Realist.** High-tension because realism's engine
includes unaffiliated suffering, over which affiliative warmth reads as
invalidation and the promised feeling never fires — the card's tonal-collapse
failure (`tones/warm.md §7`) and its boundary against `tone-compassionate`
(`tones/warm.md §1`). It resolves by `integrate` with a named drop:
companionable narration accompanies the texture of ordinary life
(`tones/warm.md §6`) but yields at any passage naming a harm the reader now
suffers, substituting unadorned or compassionate register, and returns only
across a bridge — modulation, not drift (`tones/warm.md §4`; rules above).

**59 · warm × academic (Layer 0).** High-tension because expertise-testing
readers require competence to lead, and high warmth without substance draws
pity rather than trust (`tones/warm.md §2`;
`[@clm-tone-warm-warmth-without-substance]`); the card forbids warmth over an
unsupported claim in this form (`tones/warm.md §3`). It resolves by
`alternate`: warmth frames the opening and transitions and yields at the
thesis (`tones/warm.md §6`), dosed to one sustained beat between runs of
substance (`tones/warm.md §4`; `[@clm-tone-warm-dosage-yield]`).

**60 · warm × blog / marketing (Layer 0).** High-tension because the tone's
native marketing surface is also where its arch-failure concentrates — stock
friendliness and brand-voice smarm over claims — against
`layers/layer0-blog.md`'s requirement that consequential claims carry direct,
suitable evidence (`tones/warm.md §4`;
`[@clm-tone-warm-warmth-without-substance]`). It resolves by `integrate`: voice
and takeaway coexist, every warm beat carries a concrete fact, and warmth yields
at the proof and the CTA, where sincerity must be earned by substance
(`tones/warm.md §4`, §6; `[@clm-tone-warm-dosage-yield]`).

## Related

- [Tone index](_index.md)
- [Tone taxonomy](../docs/architecture/tone-taxonomy.md)
- [ADR-0004](../docs/decisions/ADR-0004-tone-layer.md)
