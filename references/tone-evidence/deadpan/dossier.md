# Tone Evidence Dossier — Deadpan

- **Tone ID:** `tone-deadpan`
- **Family:** Humor
- **Taxonomy row:** `docs/architecture/tone-taxonomy.md` (deadpan row and its neighbor sentences)
- **Researched:** 2026-09-24
- **Evidence status:** complete (sub-items flagged evidence-incomplete, see §H and §I)
- **Boundary under test:** deadpan is the comedic effect produced when absurd, incongruous, or loaded *content* meets a deliberately expressionless, literal, register-stable *surface*. The humor lives in the gap between the two; the surface itself claims nothing. This dossier tests that boundary against three neighbors: **`tone-comedic`** (same Humor family — but builds visible joke machinery: setup, timing, comic framing; deadpan *withholds* the play signal so the reader must infer it), **`tone-detached`** (neutral observation with no comic intent — deadpan is detached's *surface with absurdist content loaded into it*), and **the satirical mode `satirical-literature`** (targets and prescribes — deadpan often targets by simply *recording*; this is a genre-mode neighbor, not a tone id). Where evidence blurs a boundary, it is noted rather than resolved.

---

## A. Claims matrix

| claim_id | claim | tier | locator | scope | confidence |
|---|---|---|---|---|---|
| clm-tone-deadpan-incongruity-gap | Incongruity gap: absurd or loaded content against an expressionless, register-stable surface is the core comic engine — the surface denies the joke, the content supplies it, and the reader's resolution of the mismatch is the laugh. | 1 | `src-deadpan-modest-proposal-1729` — full text (Project Gutenberg eBook #1080); `src-deadpan-suls-joke-model-1972` — ch. 4 (pages vary by catalog: 81–97 / 81–100) | Written prose (narrative, essay, satiric reportage) where the surface is authored narration rather than a live performer's face; cross-linguistic instances in French, Urdu/Hindi (Manto, Parsai), Russian (Kharms). | strong |
| clm-tone-deadpan-withheld-play-frame | The play frame must be inferred, not announced: withholding the play signal makes the reader infer that play is active, and removing that inference converts comedy into literal statement. | 2 | `src-deadpan-bateson-play-frame-1955` — in Bateson (ed.), *A Theory of Play and Fantasy*, pp. 31–56; `src-deadpan-goffman-frame-analysis-1974` — ch. 3 and part VI | Written contexts where no performer is present to signal with face or timing; holds for narration, essay, and dialogue; in stage/film some signals are present but minimal. | moderate |
| clm-tone-deadpan-echoic-dissociation | Echoic mention / dissociation: the narration repeats an institutional formula while dissociating from it, and the dissociation is signalled only by the absurdity of what is echoed — never by a change of voice. | 2 | `src-deadpan-wilson-sperber-verbal-irony-1992` — pp. 56–74; `src-deadpan-sperber-wilson-mention-1981` — pp. 283–292 | Applies when the surface borrows a recognizable register (case file, memo, news report, budget) as echo target; purely personal first-person flatness without a borrowed register edges toward `tone-detached`. | strong |
| clm-tone-deadpan-understatement-operators | Understatement operators — litotes, meiosis, hedged negatives, institutional euphemism — grammatically suppress emphasis so that the content, not the voice, carries the shock. | 1 | `src-anandavardhana-dhvanyaloka-1990` — sections on suggestion (*dhvani*) and the surface meaning; `src-deadpan-booth-irony-1974` — discussion of irony as understatement and the 'stable' ironic voice | Prose in any register; the operators are documented across the surveyed traditions; most at home in institutional, clinical, or fiscal registers. | strong |
| clm-tone-deadpan-literal-read-failure | Because the literal reading is accessed first, a deadpan passage with no key reads as sincere statement or as incompetence before it reads as comedy; the writer must plant at least one unmistakable incongruity so the reader can reframe. | 2 | `src-deadpan-giora-graded-salience-1997` — pp. 183–206; `src-deadpan-winner-point-of-words-1988` — ch. 4, pp. 104–142 | Written prose addressed to a general readership; strongest in generated or unfamiliar writing where the reader has no author-level prior. | strong |
| clm-tone-deadpan-clinical-reportage | The prose substitute for the straight face is the clinical or bureaucratic register: horror, scandal, or absurdity reported in case-file cadence — attributed, dated, itemized — so the narrator's neutrality is structural rather than performed. | 2 | `src-deadpan-jalal-pity-partition-2013` — historical framing of partition testimony and documentation; `src-deadpan-manto-selected-stories-2008` — partition stories (clinical tone attested at genres/satirical-literature.md lines 115, 321, 371, 385, 499) | Narrative fiction, reportage-parody, and satiric essay; particular to traditions with a strong bureaucratic written register; not required for stage or aphoristic deadpan (Kharms, Keaton). | moderate |
| clm-tone-deadpan-performance-transfer | The deadpan *face* does not transfer losslessly to prose: the origin is the expressionless face of performance, so the writer must substitute register-stasis and withheld reaction, with an acknowledged loss of the performer's physical timing. | 3 | `src-deadpan-curtis-keaton-2022` — biographical/critical discussion of Keaton's screen persona (evidence-incomplete bibliographic record) | Any adaptation of deadpan from visual or performed media into prose; in native prose the claim is analogical — prose builds its own flat surface rather than inheriting one. | moderate |
| clm-tone-deadpan-saturation-dosage | Deadpan decays under repetition: each recurrence of the same flat-surface move reduces novelty and invites the reader to pre-cue the joke, after which the construction lands literally — so a piece should escalate rather than repeat. | 2 | `src-deadpan-berlyne-aesthetics-1971` — book-level only (Appleton-Century-Crofts, 1971; xiv+336 pp.; page locator not verified); `src-deadpan-clark-gerrig-pretense-1984` — pp. 121–126 (obviousness/pre-cueing discussion) | Sustained pieces (essay, story, chapter) using deadpan as the dominant tone; not a concern in single-sentence or headline uses; dosage thresholds are bounded writer-inference, not measured constants. | moderate |
| clm-tone-deadpan-flatness-failure | Flatness without absurdity fails: expressionless delivery of content that is itself unremarkable produces confusion or blandness instead of comedy — the gap closes from the content side. | 2 | `src-deadpan-giora-graded-salience-1997` — pp. 183–206; `src-deadpan-wilson-sperber-verbal-irony-1992` — pp. 56–74 | All deadpan prose; the check applies before any use of the tone; distinct from failure mode 2 (missing key) — here the key may exist but points at nothing. | moderate |

Nine claim records are written to `claims/`, one per row, with locators, counterevidence, scope, exceptions, confidence, report anchors, and inference labels.

---

## B. Cognitive and psychological foundations

1. **Incongruity and resolution (Suls, 1972).** Suls's two-stage model — perceive an incongruity, then find the rule that resolves it — describes the deadpan read precisely: the flat surface *creates* the incongruity (nothing in the delivery signals a joke), and the reader supplies the rule (this must be a joke; the surface is lying). Locator: ch. 4, page range varies across catalogs (81–97 / 81–100); the comedic silo records pp. 81–100. Tier 2.
2. **Echoic-mention and dissociation (Wilson & Sperber, 1992; Sperber & Wilson, 1981).** Verbal irony echoes an attitude the speaker dissociates from; the deadpan surface is the *maximally quiet* way to produce that echo — the voice never rises, so the dissociation must be inferred from content alone. Locators: E-Language and Literature 17(1), 56–74; *Poetics* 10, 283–292. Tier 2.
3. **Pretense (Clark & Gerrig, 1984).** Irony as apparent communication of an attitude the speaker does not hold; their "obviousness" dimension maps deadpan as *least obvious* pretense — the poker face hides the pretense itself. Locator: *JEP: General* 113(1), 121–126. DOI 10.1037/0096-3445.113.1.121. Tier 2.
4. **Salience-graded literals (Giora, 1997).** The literal interpretation is accessed first when salient; deadpan *weaponizes* this by making the literal reading available and wrong simultaneously — the source of both the laugh and the failure mode. Locator: *Cognitive Linguistics* 8(3), 183–206. DOI 10.1515/cogl.1997.8.3.183. Tier 2.
5. **Play frame and signaling (Bateson, 1955; Goffman, 1974).** Bateson's play signal ("these are not the signals that they would be") is exactly what deadpan *removes*; Goffman's frame analysis explains the reader's work of re-framing a neutral surface as play. Locators: in Bateson, ed., *A Theory of Play and Fantasy*, pp. 31–56; Goffman ch. 3 ("Frame Analysis") and part VI. Tier 2.
6. **Developmental recognition (Winner, 1988).** Winner's account of how children learn that "the point of words" can diverge from their literal force explains why deadpan is a learned competence — and why unprepared readers fail it. Locator: ch. 4, pp. 104–142. Tier 2.
7. **Arousal and novelty (Berlyne, 1971).** Collative variables — novelty, surprise, complexity — drive arousal; deadpan's surprise is *deferred* (the reveal comes at the second reading), which predicts its decay under repetition. Locator: book-level only (Appleton-Century-Crofts, 1971; xiv+336 pp.; TOC and page-level locators not verified — evidence-incomplete). Tier 2.
8. **Null / not claimed here.** No deadpan-specific fMRI or psychophysiological study is claimed; no facial-coding study of the deadpan expression is claimed.
   - Keaton's face is documented as *lexical and biographical record* (tier 5 and secondary tier 3), not as experimental evidence.
   - Stated as null rather than padded (evidence rule).

---

## C. Rhetorical and literary tradition

The tradition runs on one move: **say the unbearable thing in the voice of a record-keeper.**

- **Classical root — litotes and meiosis.** Understatement by negation of the opposite (litotes) and deliberate minimizing (meiosis) are the grammatical ancestors of the flat surface. The repo's shared Sanskrit source, *Dhvanyaloka* (`references/evidence/sources/src-anandavardhana-dhvanyaloka-1990.json`), supplies the Indian theoretical counterpart: suggestion (*dhvani*) works when the surface says less than the meaning requires — deadpan is *dhvani with the emotional signal removed*. Cross-linked, not claimed as a translation.
- **Early modern English — the mock-serious register.** Swift's *A Modest Proposal* (1729) is the canonical printed deadpan: fiscal-bureaucratic prose cataloguing the pricing of children, with zero tonal break. Wikipedia's article on the essay itself notes the phrase "conventionally an allusion to this style of deadpan satire" (tier 5, corroborating only).
- **Colonial and modern Urdu/Hindi — the clinical witness.** Manto's partition stories report atrocity in case-file cadence; Parsai's *Inspector Matadeen* runs bureaucratic Hindi through satiric situations. The repo's `genres/satirical-literature.md` documents both (Manto's clinical tone at lines 115, 321, 371, 385, 499; Parsai's deadpan mask openings at lines 211–213 and the translation gap at line 571).
- **Soviet/Russian short form — the bureaucratic absurd.** Kharms's "Today I Read Quite by Accident…" escalates a man's death through flat administrative clauses; the deadpan is in the *sentence order*, not in any character's voice.
- **Twentieth-century stage — the face as instrument.** Keaton's "great stone face" (lexicon record, 1928) and Beckett's Vladimir and Estragon (shared `work-frankenstein`-style boundary case: `work-deadpan-waiting-for-godot-1953`) establish that the delivery can carry the entire comic load while the content stays bleak.

---

## D. Craft mechanism inventory

Card §5 input. Ten mechanisms, each with a practice anchor:

1. **Litotes / meiosis** — "not unhopeful"; a disaster described as "a slight complication."
   - *Avoid:* courtesy litotes with no absurd content (sincerity failure, §G-1).
2. **Register stasis** — hold the institutional or clinical register *through* the absurd turn; never let the narration flinch.
   - *Avoid:* flinching mid-passage (a single wince collapses the frame); this is prose's core substitute for the Keaton face.
3. **Paratactic declaratives** — short coordinate sentences, no subordination, no hedge; the sentence refuses to react.
   - *Avoid:* subordination that explains *why* the speaker is calm — explanation breaks the echo.
4. **Catalogue cadence** — list the absurd items in the same rhythm as the mundane ones (Swift's itemised budget).
   - *Avoid:* ordering the list so the absurd item gets punchline emphasis; the rhythm must not signal which item matters.
5. **Withheld reaction** — the narrator never laughs, never winks, never labels the joke.
   - *Avoid:* the tagged reaction ("it was, of course, absurd") — it supplies the key *and* spends the gap in one clause.
6. **Literal-first phrasing** — choose wording whose *first* reading is sincere, so the second reading is the reader's discovery (Giora's salience mechanism used deliberately).
   - *Avoid:* wording whose first reading is nonsense — there is no sincere ladder to climb down from.
7. **Dead naming / bureaucratic euphemism** — "incident," "irregularity," "the matter" — institutional nouns that swallow horror.
   - *Avoid:* euphemism the reader cannot unpack; if the real term is never recoverable, the gap is invisible.
8. **Reportage attribution** — "according to the report," "it was noted that" — the citation habit of the record-keeper.
   - *Avoid:* fake citations in real-world-facing copy; attribution is a voice device here, not a factual claim.
9. **Timing by paragraph break** — the flat sentence lands, *then* the break; the laugh happens in the silence (prose's substitute for the comic beat).
   - *Avoid:* burying the beat mid-paragraph where running prose carries the reader past it.
10. **Escalation without inflection** — raise the stakes while keeping sentence length and vocabulary constant (Kharms's structural method).
    - *Avoid:* escalating by also escalating diction — that is comic crescendo (`tone-comedic` machinery, not deadpan).

---

## E. Cross-cultural survey

- **Anglo vaudeville / film (origin of the term; Anglophone context, not a counted tradition).** "Dead pan" enters print as film slang; the 1928 *New York Times* slang item (quoted in the lexicon record) defines it as "playing a role with expressionless face," citing Buster Keaton. The etymology is dead + pan (face); T. W. Barrett is credited as an early music-hall practitioner (Busby, 1976, as relayed by the lexicon). **Tier 5** — recognition and vocabulary only.
- **French — *pince-sans-rire* (recognition only, not a counted tradition).** Wiktionary records the adjective meaning "dry, deadpan" and the noun for a person with a deadpan sense of humour (accessed 2026-09-24). The literal gloss — "pinch without laughing" — is itself a craft instruction. **Tier 5**, lexical: kept for vocabulary and recognition, and deliberately excluded from the tradition count below.
- **India — Urdu/Hindi clinical-satiric mode (counted; Indian requirement met).**
  - *Manto (Urdu).* `src-deadpan-manto-selected-stories-2008` (Vintage India 2008, ISBN 81-8400-144-4) holds the partition stories in case-file cadence — inventory of bodies and goods, attributed speech, plain declaratives, no moral reaction from the narrator (`work-deadpan-manto-partition-stories`). Attestation locator inside §E: `genres/satirical-literature.md` lines 115, 321, 371, 385, 499 (clinical tone; flat, non-resolving endings), with `src-deadpan-jalal-pity-partition-2013` (Princeton University Press, 2013) supplying the scholarly framing of partition testimony. **Translation limit:** the English *Selected Stories* carries Manto's clinical stance but not the Urdu — this silo's record leaves the translator/imprint lineage unresolved (the Jalal-edited Vintage 2008 printing here, the detached silo's Penguin record there), and the genre file's translation-integrity disclosure at line 499 records that the older Ralph Russell translations occasionally formalize Manto's deliberately colloquial Urdu. Claims are therefore scoped to register and structure as rendered, not to his diction.
  - *Parsai (Hindi).* `src-deadpan-parsai-matadeen-2003` (Katha, 2003; practice record `work-deadpan-parsai-inspector-matadeen`) runs officialdom's own minimizing vocabulary through satiric situations. Attestation locator inside §E: `genres/satirical-literature.md` lines 211–213 (deadpan mask openings, set beside Swift and Kshemendra). **Translation limit:** Naim's English carries Parsai's bureaucratic stance and structure but not the Hindi idiom — the genre file's line 571 records that his satiric register depends on the bureaucratic Hindi of post-independence government offices, a register no English translation reproduces, and that polished English smooths away the roughness the satire functions on; it names this the most significant translation gap in that bibliography. Translator credits also vary between Nayar and Naim across printings (declared unresolved in `src-deadpan-parsai-matadeen-2003`), so claims are limited to narrative stance and structure as rendered, not to Parsai's wordplay.
  - **Tier 2/3** (scholarly translations and critical framing) with genre-file cross-links.
- **Russia — Kharms and the absurd bureaucratic sentence.** *Today I Read Quite by Accident* (English, Glas/Pushkin House, 2007) as the structural escalation exemplar. **Translation limit:** `src-deadpan-kharms-today-2007` records the English collection as translation-mediated, with Russian intonation and sentence rhythm flattened in English, so the paratactic beat the deadpan lives in is only partly recoverable — claims are scoped to escalation structure as rendered. **Tier 3/4** (published translation of a widely taught writer; secondary attestation).
- **Argentina/Spain — Borges's mock-scholarly deadpan.** *Ficciones* (shared `work-ficciones`, cross-linked not duplicated) parodies erudite commentary with straight-faced footnotes; the repo genres file references it. **Tier 2/3.**
- **Rasa engagement (hasya and dhvani).** Hasya — the comic rasa — is the applicable Indian frame, and it is held by the comedic silo: shared `src-natyashastra-ghosh-1951` (Ghosh's critical translation, ch. 6) treats hasya and its gradations of laughter, and `clm-tone-comedic-hasya-rasa` is the comedic silo's claim. This dossier records deadpan as **not a rasa** (cross-link `clm-rasa-emotional-aesthetic`): deadpan withholds the aesthetic-emotional signal the rasa framework requires, and no Sanskrit term maps directly onto it (evidence-incomplete item 6, §I) — recorded as an honest null inside §E, not papered over. *Dhvani* (shared `src-anandavardhana-dhvanyaloka-1990`) remains the Indian theoretical anchor: deadpan is *dhvani* with the emotional signal removed (§C) — a cross-linked analogy, not a claimed translation or equivalence.

**Tradition count and translation-limit summary.** The floor asks for at least two non-Anglophone traditions with named sources, including at least one Indian/regional analyzed in §E rather than only cross-referenced. Counted here: **India** (Manto and Parsai, with silo records and locators above), **Russia** (Kharms, `src-deadpan-kharms-today-2007`), and **Argentina/Spain** (Borges, shared `work-ficciones`) — three counted traditions, Indian requirement met inside §E. The Anglophone vaudeville bullet and the French lexical bullet are **recognition only, not counted traditions** (tier-5 lexical and Anglophone context respectively). Translation limits are stated inside each counted tradition's bullet: Manto's Urdu, Parsai's Hindi idiom, and Kharms's Russian intonation do not survive translation intact, so every claim resting on those traditions is scoped to register and structure as rendered.

---

## F. Exemplar field

| work_id | work | creator | mechanism demonstrated | verification note | transfer limit |
|---|---|---|---|---|---|
| work-deadpan-modest-proposal-1729 | *A Modest Proposal* (1729) | Jonathan Swift | Sustained bureaucratic cataloguing; no tonal break across 16 pages | Identity verified 2026-09-24 (printed 1729, S. Harding, 16 pp.; Project Gutenberg eBook #1080); `analysis_status: complete`; technique described, not reproduced | None — native prose; PD |
| work-deadpan-waiting-for-godot-1953 | *Waiting for Godot* (1953) | Samuel Beckett | Bleak content + vaudeville double act; the stage face carries the joke | Standard bibliographic identity cross-checked against the repo's absurdist-drama genre references; dates disambiguated (1953 = first French publication/performance; English revision 1955); no passage quoted | Stage delivery must be rebuilt in prose as register-stasis |
| work-deadpan-kharms-today-2007 | "Today I Read Quite by Accident" (Kharms, 2007) | Daniil Kharms (English collection, Glas/Pushkin House) | Escalation with zero inflection; death handled as paperwork | English collection identified 2026-09-24; translator attribution (Anna Mohr) standard for the edition but not re-verified page-by-page; `analysis_status: translation-mediated` | Translation-mediated; Russian intonation flattened |
| work-deadpan-manto-partition-stories | Manto partition stories (Jalal-framed English edition) | Saadat Hasan Manto | Clinical reportage of atrocity | Mechanism attested at `genres/satirical-literature.md` lines 115, 321, 371, 385, 499; passage-level close reading NOT performed (evidence-incomplete item 3, §I); tied to the declared Vintage/Penguin imprint discrepancy in `src-deadpan-manto-selected-stories-2008` | Translation-mediated; see imprint note in §I |
| work-deadpan-parsai-inspector-matadeen | *Inspector Matadeen* (Parsai, 2003) | Harishankar Parsai | Bureaucratic Hindi through satiric situations | Deadpan mask openings attested at `genres/satirical-literature.md` lines 211–213; record checked 2026-09-24; translator-by-imprint mapping not verified; ID deliberately non-colliding with the comedic silo's `work-parsai-inspector-matadeen` | Translation gap documented at genres file line 571 |
| work-deadpan-keaton-general-1926 | *The General* (1926) | Buster Keaton, Clyde Bruckman | The expressionless face against catastrophe | Film identity standard (1926, United Artists release year); `analysis_status: secondary-attested` — resting on the 1928 lexical record and tier-3 Keaton criticism; direct viewing not performed | **Visual/performance transfer limit:** the face is a *visual* channel; prose cannot reproduce it and must substitute register-stasis and withheld reaction (see `clm-tone-deadpan-performance-transfer`) |

**Buster Keaton and the transfer problem.** Deadpan as a *term* was built on Keaton's face; that is precisely the case that prose cannot copy. The research rule: **do not describe prose deadpan as "a straight face" without naming the prose mechanism that replaces it.** A neutral narrator in fiction is not a Keaton close-up; it is register stasis plus withheld reaction, and the comic load shifts to the content and the sentence rhythm. Esslin's staging discussion (1961) reinforces that theatrical absurdist delivery is a *staged* semiotic that prose must re-engineer, not transcribe.

---

## G. Failure and misuse research

Card §7 input. Six failure modes; each becomes a record-backed paragraph (or structured block) in the card:

**1. Flatness without absurdity.**
- *Mechanism:* expressionless delivery of content that is itself unremarkable.
- *Example (original, do not quote any source):* "The meeting concluded at four. Several items remained on the agenda." — sincere, competent, and completely inert.
- *Effect:* the reader detects no gap, so no comic inference fires; the prose reads sincere, then dull.
- *Diagnostic:* does the *content* contain a mismatch that the surface is hiding? If not, there is nothing for the flatness to contradict.
- *Revision:* load the content (make the agenda item absurd), or keep the content and change tone.
- *Scope:* all deadpan prose; the first check before using the tone. Basis: Giora (literal-first with no salient non-literal target), Wilson & Sperber (no dissociated echo), lexical record.

**2. Confusion with literal statement / sincerity failure.**
- *Mechanism:* missing play signal or missing key, so the frame is never inferred.
- *Example (original):* a case-file sentence about a bureaucratic catastrophe with no single detail that could not appear in a real report.
- *Effect:* reader accepts the absurd at face value, or rejects the prose as incompetent.
- *Diagnostic:* would a naive first reading be *sincere*? If yes, and sincerity is not intended, the key is missing.
- *Revision:* add one unmistakable incongruity early (a "tell") so the frame can be inferred and everything after it reads inside the frame.
- *Scope:* general readership, single-pass reading. Basis: Winner (learned competence), Clark & Gerrig (cue-obviousness varies), Giora.

**3. Corporate blandness.**
- *Mechanism:* adopting the *surface* of deadpan (neutral, hedged, institutional prose) without absurdist content or satiric intent.
- *Example (original):* "We are excited to announce our continued commitment to leveraging synergies." — flat, institutional, and dead in the wrong way.
- *Effect:* reads as lifeless marketing copy; the word "deadpan" gets used colloquially for exactly this failure.
- *Diagnostic:* is there a target or an absurdity? If neither, this is `tone-detached` at best, or plain blandness.
- *Revision:* either load the content with a real mismatch, or switch tone deliberately to a plain register / `tone-detached`.
- *Scope:* marketing, product, and generated-voice contexts. Basis: **tier 4–5 only** (craft and audience registers — evidence-incomplete item 2; never sole support).

**4. Saturation / repetition collapse.**
- *Mechanism:* repeating the flat-surface move within one piece; the surprise decays (Berlyne novelty) and the reader pre-cues (Clark & Gerrig).
- *Example (original):* three consecutive paragraphs each ending in the same deliberately flat understatement — by the third, the reader predicts it.
- *Effect:* the second and third deadpans land as literal statements; the tone flips to sincere or smug.
- *Diagnostic:* count the flat-surface beats; if the reader could predict the next one, it has saturated.
- *Revision:* vary the mechanism (switch operators), escalate stakes instead of repeating the punch shape, or break frame once to reset.
- *Scope:* sustained pieces; not a concern in single-sentence uses. Basis: Berlyne (book-level), Clark & Gerrig, Kharms structure.

**5. Machine-flat prose (the AI failure).**
- *Mechanism:* constant sentence length, constant vocabulary, no escalation — flatness *everywhere*, not just at the joke.
- *Example (original):* a passage where every sentence is the same declarative beat, whether the content is a shopping list or a death.
- *Effect:* no gap ever opens, because the surface offers no contrast against anything; the reader stops detecting a voice.
- *Diagnostic:* read two adjacent sentences aloud — if they are metrically identical, the surface has become the content.
- *Revision:* keep the *joke* flat; let the surrounding prose breathe (vary rhythm, allow one reaction or inflection outside the deadpan beat).
- *Scope:* generated and long-form prose especially. Basis: synthesis of Berlyne (arousal needs variation) and §D — **writer-inference** (claim 8's sibling; flagged as such).

**6. Deadpan vs. cruelty / target loss.**
- *Mechanism:* recording suffering without the institutional or absurd frame that makes the recording *say something*.
- *Example (original):* flat, affectless narration of a disaster with no borrowed register — the horror arrives unframed and unindicted.
- *Effect:* the prose replicates the atrocity instead of indicting it; the flatness reads as moral vacancy (adjacent to `tone-detached`, minus the intent).
- *Diagnostic:* whose voice is the flatness borrowed from — the record-keeper, the memo, the report — or nobody?
- *Revision:* anchor the flatness to a named register (case file, memo, dispatch) so the echo does the satiric work.
- *Scope:* documentary, disaster, and conflict material; particular responsibility for the Manto/Parsai lineage. Basis: Manto/Parsai practice (genre file), Jalal (2013) framing.

---

## H. Dosage and saturation findings

Card §4 input. No deadpan-specific numeric study exists (evidence-incomplete item 1; thresholds below are bounded writer-inference, not measured constants). The guidance:

- **Opening:** one flat sentence to establish the surface, then the first incongruity within the first paragraph.
  - *Rationale:* a longer runway risks the reader settling into sincerity — Giora's literal-first default hardening before the key arrives.
- **Sustained passages:** one flat-surface beat per paragraph at most; escalate stakes rather than repeat the same operator.
  - *Rationale:* Kharms's method (constant mechanics, rising stakes); Berlyne's novelty decay predicts habituation when the same collative cue recurs unchanged.
- **The frame break:** if a piece runs long, exactly one non-flat beat — a single inflection, a reaction, a syntactic swell — renews the surprise for the remainder.
  - *Rationale:* the prose analogue of Clark & Gerrig's pre-cueing observation — a fully transparent pretense cannot keep producing the effect, so transparency must be reset once.
- **Deadpan vs. machine-flat prose:** deadpan is *localized* flatness around a loaded content-bearing sentence; machine-flat prose is *global* flatness.
  - *Card must state this explicitly* — it is the most likely misuse of the tone in generated text (§G-5).
- **Reader-cue budget:** at least one unmistakable incongruity early; never more than one full re-cue per ~500 words.
  - *Rationale:* beyond that budget the reader oscillates between frames instead of holding the play frame (Goffman re-framing churn), and each re-cue reads as a repeated joke (§G-4 saturation).
- **Ending:** stop flat; do not add a reaction coda.
  - *Rationale:* a closing inflection re-frames the whole passage as a told joke, retroactively supplying the key the reader should have had to infer (§G-2 in reverse).

---

## I. Source records

Every source, claim, and primary work referenced above is written as a JSON
record in this silo. Two cross-silo records are read-only pointers and are
disclosed below rather than duplicated; shared registries are not edited here.

**Cross-links (shared registry, read-only):**
- `src-anandavardhana-dhvanyaloka-1990` — *dhvani* as the Indian theoretical anchor for surface-vs-meaning gap (shared with the rasa/sadness and other silos).
- `clm-rasa-emotional-aesthetic` — rasa theory contrast: deadpan is *not* a rasa; it withholds the aesthetic-emotional signal the rasa framework requires (boundary note for the card).
- `work-ficciones` — Borges's mock-scholarly deadpan (shared; not duplicated here).
- `genres/satirical-literature.md` lines 115, 211–213, 225–227, 321, 371, 385, 461, 477, 499, 571 — Manto clinical tone, deadpan mask openings (Swift, Kshemendra, Parsai), litotes, mask-collapse diagnostics, Parsai translation gap.

**Sibling-silo context (read-only):** the `comedic` silo owns `work-parsai-inspector-matadeen` (Manas 1994 / Katha 2003, trans. Naim); the `detached` silo owns `src-detached-manto-selected-stories-2008` (Penguin). This silo therefore uses `deadpan`-prefixed IDs for its own Manto/Parsai records and flags the imprint discrepancy in §I of the source records rather than resolving it.

**Evidence-incomplete items (declared, not padded):**
1. No deadpan-specific numeric dosage/saturation study; §H thresholds are bounded writer-inference.
2. "Corporate blandness" failure mode rests on tier 4–5 evidence only; never sole support.
3. Manto/Parsai passage-level close reading not performed; attestation rests on the repo genre file and published-translation records (confidence moderate).
4. Berlyne (1971) page-level locator not re-verified (book-level only).
5. No controlled prose-vs-performance comparison; claim 7's transfer limit is writer-inference from lexical and staging sources.
6. No Sanskrit term maps directly onto deadpan; *dhvani* is a theoretical anchor, *hasya* belongs to the comedic dossier.
7. Suls (1972) ch. 4 page range conflicts across catalogs (81–97 / 81–100).
