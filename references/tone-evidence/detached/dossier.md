# Detached — Research Dossier

- Tone ID: `tone-detached`
- Family: Candor
- Researched: 2026-09-24
- Evidence status: complete (one honest null in §H, tagged `evidence-incomplete`; see §G/§H notes)

## A. Claims matrix

| claim_id | claim | tier | locator | scope | confidence |
|---|---|---|---|---|---|
| clm-tone-detached-restraint-vs-absence | Omission strengthens prose only when the omitted material exists and is inferable; with nothing beneath, the same surface reads as absence, not restraint. | 1 | Shklovsky 1965 (tier 1, strongest support); Hemingway 1932 ch.16 (tier 4); Miall & Kuiken 1994 (tier 2) | Prose narration that withholds affect | strong |
| clm-tone-detached-psychic-distance | Detached narration sits at mid-to-far psychic distance and shows only externally observable action and speech (external focalization), suppressing interior access by design. | 2 | Genette 1980 bk.2 ch.4; shared clm-point-of-view-psychic-distance | Third-person and first-person prose | strong |
| clm-tone-detached-reader-emotion-inference | Readers automatically infer a character's emotional state from described behavior, objects, and situation even when no emotion word appears; a mismatching emotion word slows comprehension. | 2 | Gernsbacher, Goldsmith & Robertson 1992, 89–111 | Narrative comprehension | strong |
| clm-tone-detached-transportation-risk | Detached narration lowers emotional transportation; low transportation predicts reduced empathy and disengagement, while high transportation predicts its increase. | 2 | Green & Brock 2000, 701–721; Bal & Veltkamp 2013, e55341 | Extended narrative reading | strong |
| clm-tone-detached-affective-distance | Aesthetic/psychical distance produces the "objective" reception detached prose seeks, but distance has an antinomy: past a threshold it collapses the viewer's personal relation to the object. | 2 | Bullough 1912, 87–118; Trope & Liberman 2010, 440–463 | Aesthetic reception; narratorial stance | strong |
| clm-tone-detached-defamiliarization | Reporting familiar or horrific material in stripped, procedural description de-automatizes perception and renews attention (ostranenie); empirical work links foregrounding to felt affect. | 1 | Shklovsky 1917/1965 (tier 1, strongest support, with Manto Selected Stories 2008, tier 1); Miall & Kuiken 1994, 389–407 (tier 2) | Description of violence, routine, and the familiar | strong |
| clm-tone-detached-indian-vairagya | In Indian thought vairagya (dispassion/renunciation) is a disciplined stance that stills the mind, not indifference; it is a training, not an absence of relation. | 1 | Patanjali, Yoga Sutras 1.12–1.15 (Bryant 2009) | Indian philosophical and literary context | moderate |
| clm-tone-detached-indian-clinical-manto | Manto's clinical, declarative Urdu prose withholds affect at scenes of atrocity; the withheld response is recoverable from event and consequence, producing moral pressure rather than numbness. | 1 | Manto, *Selected Stories* (Taseer 2008); genre file `genres/satirical-literature.md` §Ch07 | Indian/regional narrative; atrocity material | strong |
| clm-tone-detached-ai-slop-flatline | Machine-sounding flatness differs from crafted detachment: it combines uniform sentence length/frame and generic assertion with a missing inferable charge — precisely the structural tells the catalog flags. | 2 | Miall & Kuiken 1994 (tier 2, strongest support); `references/structural-tells-catalog.md` (tier 3) | AI-slop diagnosis of detached prose | moderate |
| clm-tone-detached-cross-cultural-objectivity | Objectivity movements recur independently — French chosisme (Robbe-Grillet), German Neue Sachlichkeit, Japanese shasei, Chinese baimiao — each defining a neutral descriptive register, not a universal code. | 1 | Shiki (Watson 1997) (tier 1, strongest support); Crockett 1999 (tier 2); baimiao reference entry (tier 3); Robbe-Grillet 1963 (tier 4) | Cross-cultural claim, scoped per tradition | moderate |

Every row resolves to a record in `claims/`.

Reading the matrix: tier shows the strongest single support, not an average; where a claim pairs a Tier-4 practitioner statement (e.g., Hemingway on omission) with stronger peer-reviewed or scholarly support, the cell records the strongest tier and the full pairing is recorded in `locator`, so no consequential claim rests on craft assertion alone. `strong` means convergent evidence plus a verified exemplar; `moderate` means the mechanism is attested but the transfer to this tone is inferential or translation-limited. Counterevidence is recorded per claim rather than buried.

## B. Cognitive and psychological foundations

**Distancing is a mechanism, not an absence.** Edward Bullough's "'Psychical Distance' as a Factor in Art and an Aesthetic Principle" (1912) is the foundational account: aesthetic experience depends on a degree of removal from the viewer's "practical, actual self," permitting attention to "objective" features. Crucially Bullough names an **antinomy of Distance** — too little distance is sentimental, too much is cold and unpersuasive; the tone is therefore a calibrated position, not a maximum. This is the single most important corrective to "neutral = emotionless." (Bullough 1912, §II.2 "The antinomy of Distance," pp. 87–118.) Construal Level Theory supplies the general-psychology analogue: greater psychological distance (social, temporal, spatial, hypothetical) yields higher-level, more abstract construal (Trope & Liberman 2010, *Psychological Review* 117(2), 440–463).

**Readers infer the withheld emotion.** Gernsbacher, Goldsmith & Robertson (1992) demonstrated that during narrative comprehension readers form explicit, lifelike representations of characters' emotional states; a subsequent mismatching emotion word slows reading, evidence that the expected emotion is represented even when it is not stated. This is the empirical basis for the tone's central move: describe behavior, object, and situation; let the inference do the affect. (Cognition and Emotion 6(2), 89–111.)

**Why the inference needs material under it.** Miall & Kuiken's empirical work on foregrounding shows that stylistic deviation prompts defamiliarization, which evokes feeling, which in turn guides interpretation. If nothing is foregrounded — no selection, no charged detail — there is nothing for feeling to attach to. This is the experimental counterpart to Hemingway's craft warning (claim `clm-tone-detached-restraint-vs-absence`). (Miall & Kuiken 1994, *Poetics* 22(5), 389–407; cross-link `clm-dhvani-suggestion-theory` for the suggested-meaning parallel.)

**Two failure poles, predicted.** Bullough's antinomy implies the tone has two opposite failure modes, and the evidence supports both: too little distance produces sentimentality (handled by the genre engine's own norms; cross-link `clm-melodrama-unearned-emotion`), while too much distance produces the cold, unpersuasive surface and the low-transportation disengagement documented above. The craft target is therefore a *band*, not a maximum — the card must give writers signals for correcting in both directions, not merely "withhold more."

**Disengagement risk is measurable.** Green & Brock (2000) define transportation as absorption entailing imagery, affect, and attentional focus, and show it drives narrative persuasion. Bal & Veltkamp (2013) found that fiction readers who were *not* emotionally transported showed *decreased* empathy over one week, while highly transported readers increased; the effect was specific to emotional transportation, not general reading. Detached narration is the stylistic condition most likely to produce the low-transportation case, so the tone's dosage problem is not aesthetic preference but a documented mechanism. (JPSP 79(5), 701–721; PLOS ONE 8(1), e55341.)

**Restraint is not suppression.** The psychological literature on emotion suppression (expressive suppression reducing visible response) is about a person managing their own affect; the tone's move is a *narrator* declining to name affect that the scene supplies. The distinction matters because suppression can leave a reader with nothing, while crafted restraint leaves an inferable state. This is the psychological counterpart of the craft boundary between restraint and absence (claim `clm-tone-detached-restraint-vs-absence`).

**Situation models.** Bal & Veltkamp (2013) build on Zwaan's Immersed Experiencer Framework, in which readers mentally simulate described events and integrate them with existing models. The implication for this tone is that a reader who has enough concrete event structure will simulate the scene and arrive at the feeling; the simulation, not the adjective, is the source of affect. A passage that gives an abstract summary without event structure gives the simulation nothing to run on.

**Craft consequences of the two theories.** If readers infer emotion automatically (Gernsbacher et al.), a writer can trust omission to be filled; if foregrounding is what drives feeling (Miall & Kuiken), the writer must still *select* one charged element within the plain surface. The first licenses the tone; the second constrains it. A just-falsifiable prediction follows: detached passages that contain one foregrounded concrete detail should produce more reported affect than equally detached passages containing none. This prediction is offered for the card's exercises, not as a tested result.

**Honest limit.** No study located measures a specific optimal ratio of neutral to affect-laden prose. The mechanism is supported by adjacent findings; the numeric thresholds in §H are writer-inference and labeled as such.

## C. Rhetorical and literary tradition

The tone has a distinct lineage rather than a single origin.

- **The iceberg / theory of omission.** Hemingway's *Death in the Afternoon* (1932) states the doctrine: a writer who knows the omitted material "may omit things that he knows" and the reader "will have a feeling of those things as strongly as though the writer had stated them," while one "who omits things because he does not know them only makes hollow places." The dignity of the iceberg is "due to only one-eighth of it being above water." This is the tradition's primary statement and its built-in failure condition.
- **Impersonal narration and free indirect style.** Flaubert's impersonal method and the free-indirect technique later theorized by Booth and Wood (shared `clm-point-of-view-psychic-distance`) established that a narrator can render feeling through a character's idiom without entering consciousness directly. Detached prose is the far end of that continuum.
- **Russian Formalism.** Shklovsky's "Art as Technique" (1917) argues that habitual perception is automatized and that art "makes strange," restoring perception by refusing the accepted name of things. A stripped, procedural account of violence is a direct instance.
- **The objective correlative.** T. S. Eliot's 1919 formulation — that emotion in art is evoked by "a set of objects, a situation, a chain of events" rather than named — gives the tradition its aesthetic rationale: the external surface is not a refusal of feeling but its chosen vehicle. Record `src-detached-eliot-objective-correlative-1919` (Eliot, *Hamlet and His Problems*, 1919) supplies that formulation as the tradition's craft rationale, and it underwrites §D-7's buried-charge mechanism. Detached prose is objective-correlative writing taken to its plainest register.
- **The camera eye and objectivity movements.** Genette's external focalization (Narrative Discourse, 1972/1980) formalizes narration that reports only externally observable action; the "camera eye" of Dos Passos's *U.S.A.* and Isherwood's "I am a camera" are the journalistic-literary realizations. In Germany, Neue Sachlichkeit ("New Objectivity," term coined by Hartlaub, 1925) carried a literature of "non-sentimental, emotionless reporting style, with precise detail and veneration for 'the fact'" (Crockett 1999; Midgley 2000). In France, Robbe-Grillet's *Pour un nouveau roman* (1963) argues for a neutral registering of sensations and things.
- **Documentary and clinical reportage.** The tone also descends from the reportorial register: war correspondence, autopsy and hospital notes, bureaucratic minutes, and crime reporting all model the withholding of affect that literary detachment borrows. Hemingway's own account roots the iceberg in his newspaper training, where reports "focus on immediate events, with very little context or interpretation."
- **The camera eye proper.** Dos Passos's *U.S.A.* sequence titled "The Camera Eye" and Isherwood's narrator in *Goodbye to Berlin* ("I am a camera") translate external focalization into a narrative persona — an observer who records and declines to interpret. This is the bridge between the formal concept and a usable voice.
- **Late-twentieth-century minimalism and its backlash.** The Carver-era "minimalist" surface carried detached narration into the mainstream; its critics (Wood's discussions of style and the "Kmart realism" label applied to brand-name, stripped-down realism) argued that the method had become a formula. That reception history is a live warning for this tone: a technique that was once a discipline can calcify into a default, at which point it reads as an absence of authorial decision.
- **Contested status.** The tradition's own critics note that "objectivity" is a stance with an agenda, not a view from nowhere; Neue Sachlichkeit was understood as political engagement, not philosophical detachment, and Robbe-Grillet himself rejected the label *chosisme* as an over-reading. The tone should be taught as a disciplined construction whose neutrality is a chosen effect.

## D. Craft mechanism inventory

Each mechanism lists the technique, why it works, and a verified exemplar (described, never quoted).

| # | Mechanism | Technique | Why it works (claim) | Verified exemplar |
|---|---|---|---|---|
| 1 | Behavior-and-object substitution | Replace emotion nouns and evaluative adjectives with concrete nouns and bodily/procedural verbs; report what a body does. | Readers infer emotion from behavior; a stated mismatching emotion word is disruptive (`clm-tone-detached-reader-emotion-inference`). | Camus, *The Stranger* (Meursault reports heat, walking, cigarettes, procedures). |
| 2 | External focalization / camera-eye | Restrict access to thought; give visible action and speech only. | Withholding interiority is a formal stance, not an oversight; inference continues (`clm-tone-detached-psychic-distance`). | Robbe-Grillet, *Jealousy* (a camera-like, unnamed observer catalogs surfaces and repetitions). |
| 3 | Parataxis and declarative syntax | Short main clauses; low subordination; active voice; few intensifiers or exclamation. | Even cadence can be foregrounded by a single variation; uniform cadence flattens affect (`clm-tone-detached-ai-slop-flatline`; shared `clm-pacing-rhythm-syntax`). | Hemingway, "Hills Like White Elephants" (dialogue and gesture carry the argument). |
| 4 | Procedural cadence | Sequence steps, quantities, times; let the procedure supply rhythm. | Instrumental detail de-automatizes horrific or familiar matter (`clm-tone-detached-defamiliarization`). | Manto's Partition stories (transactional sequence; flat final sentence). |
| 5 | Metonymic imagery | Part-for-whole; objects, instruments, surfaces; no pathetic fallacy. | "Objective" features hold attention without importing the narrator's mood (Bullough 1912). | Masaoka Shiki's *shasei* sketches (observed fact set beside observed fact). |
| 6 | Understatement and litotes | Meiosis; negative constructions; a smaller word where a larger one is expected. | The gap between event and register is the charged foreground (`clm-tone-detached-defamiliarization`). | Hemingway; Manto's clinical endings. |
| 7 | Buried charge / selected detail | One concrete object or act carries the withheld affect; everything else stays plain. | Foregrounding one detail elicits feeling; suggestion exceeds statement (Eliot's objective correlative, 1919; shared `clm-dhvani-suggestion-theory`). | Manto, *Khol Do* / *Thanda Gosht* (a single act or object carries the horror). |
| 8 | Psychic-distance control | Hold mid-to-far across a scene; drop briefly to close only at a stakes peak. | Distance is continuous and modulable, and over-distance collapses engagement (`clm-tone-detached-affective-distance`; shared `clm-point-of-view-psychic-distance`). | Camus, *The Stranger* (procedural distance held until the trial, then briefly charged). |
| 9 | Ellipsis / white space | Omit the emotional climax; end on the next ordinary act. | The omitted part strengthens only if it exists and is inferable (`clm-tone-detached-restraint-vs-absence`). | Manto (the flat sentence that returns to routine after atrocity). |
| 10 | Register anchoring | Procedural, technical, or administrative diction; suppress evaluative adverbs. | Neutral register re-presents the familiar as strange without editorializing (`clm-tone-detached-cross-cultural-objectivity`). | Neue Sachlichkeit reportage; Robbe-Grillet. |

**How the mechanisms combine.** The tone is not one device but a chain: (i) establish a stable, plain register (rows 3, 10); (ii) choose a surface that substitutes behavior and object for affect (rows 1, 2, 5); (iii) foreground exactly one detail that carries the buried charge (row 7); (iv) manage distance so the reader stays near enough to care (row 8); and (v) omit the emotional beat itself, ending on the next ordinary act (row 9). Failure at any link produces the flatline or roboticism diagnoses in §G. The order matters: details must be *selected* before they can be *withheld*; a writer cannot omit a charge they never placed.

**Ties to sources:** rows 1–3 and 6–9 depend on the inference and foregrounding findings in `src-detached-gernsbacher-emotion-inference-1992` and `src-detached-miall-kuiken-foregrounding-1994`; rows 5 and 10 on `src-detached-bullough-psychical-distance-1912` and the objectivity-movement sources; row 4 on `src-detached-manto-selected-stories-2008`.

## E. Cross-cultural survey

**Indian/regional (primary analysis).**

1. **Vairagya (dispassion).** Yogic and Vedantic thought treats *vairagya* — dispassion, renunciation — as one of two means (with *abhyasa*, practice) to still the mind (Yoga Sutras 1.12–1.15; Bryant 2009). The crucial distinction for this tone: vairagya is achieved detachment, not indifference. It is a trained stance one *takes toward* experience, parallel to Bullough's aesthetic distance but with an ethical/soteriological goal. This gives the tone an Indian philosophical warrant that separation-of-self is not coldness. (Cross-link `clm-rasa-emotional-aesthetic`, `clm-dhvani-suggestion-theory`.)
2. **Manto's clinical Urdu prose.** Saadat Hasan Manto renders communal violence and Partition trauma in flat, declarative, unadorned sentences, refusing sentimental or moralizing narration. The repository's own `genres/satirical-literature.md` names this "clinical detachment" and makes the flat final sentence its mechanism (§Ch07: "the last line should be the quietest"). The affect is withheld from the wording and supplied by event and consequence. Confidence in the technique is strong; the **translation limit** is real: Taseer's English (Penguin, 2008) preserves more of Manto's roughness than older Russell translations, and English loses the sociolinguistic register of Urdu. Claims about his *texture* should be scoped to the translation used.
3. **Suggested meaning (dhvani).** Anandavardhana's dhvani theory holds that the highest resonance is suggested rather than stated (shared `clm-dhvani-suggestion-theory`). Detached prose that omits the emotion and supplies the objective correlate is a prose genus of the same principle; this is an analogue, not an identity claim.

**Other non-Anglophone traditions.**

4. **Japanese: shasei ("sketch from life").** Masaoka Shiki's reform program rejected ornate puns and fantasy for "realistic observation of nature," recording observed fact plainly and trusting it (Shiki, *Selected Poems* trans. Watson 1997; Beichman 2002). The objectivity is a discipline of attention, not a thesis about emotion; haiku's brevity then leaves the affective inference to the reader.
5. **Chinese: baimiao (plain line drawing).** A descriptive register of unembellished, subtractive plainness applied in Chinese painting and narrative (reference work on *baimiao*, 2026). Applied to prose it means telling a scene in plain lines with no ornament — structurally analogous to the iceberg. **Translation limit:** the Chinese literary application is best verified in the original; this dossier therefore records baimiao as a documented technique but does not over-claim specific passages in translation.
6. **German: Neue Sachlichkeit.** Interwar literature rendered dystopia "in a non-sentimental, emotionless reporting style, with precise detail and veneration for 'the fact'" (Crockett 1999; Midgley 2000). Its neutrality was politically loaded — evidence that "neutral" is always an attitude with a position.
7. **French: chosisme.** Robbe-Grillet's essays argue for a neutral registering of sensations and things and against "nature, humanism, tragedy" (Pour un nouveau roman, 1963).

**Translation-limit summary.** Every Indian/regional and East Asian source here reaches the dossier through translation. Manto's effect partly lives in Urdu register, Shiki's in Japanese compression and kigo/kireji, and the Chinese baimiao evidence is concept-level rather than passage-level. The tone card should therefore present these traditions as genuinely load-bearing for the *principle* (withholding affect as a deliberate construction) while scoping all *texture* claims to the English edition named in `src-*`. This is not a hedge against the cross-cultural floor; it is the honest form of it.

**No false universals.** These movements are not the same stance. Vairagya is soteriologically motivated; shasei is a perceptual discipline; Neue Sachlichkeit is politically motivated reportage; chosisme is an anti-humanist program. What they share is only the surface technique of withholding affect — which is why the tone card must state scope per tradition rather than assert a universal "objective voice."

## F. Exemplar field

| work_id | work | creator | mechanism demonstrated | verification note |
|---|---|---|---|---|
| work-detached-the-stranger | The Stranger (L'Étranger, 1942) | Albert Camus | Behavior-and-object substitution; held mid-far psychic distance; affect withheld and inferred | Novel verified; Meursault's affectless reporting is the canonical description. Matthew Ward's translation (1988) noted for tone fidelity. |
| work-detached-manto-selected-stories | Selected Stories (partition/street narratives, 1940s–1950s) | Saadat Hasan Manto | Procedural cadence; ellipsis; clinical declarative endings; buried charge | Collection verified (Penguin, trans. Aatish Taseer, 2008); mechanism corroborated by repo `genres/satirical-literature.md`. |
| work-detached-hills-like-white-elephants | "Hills Like White Elephants" (1927) | Ernest Hemingway | Parataxis; dialogue and gesture over stated feeling; ellipsis | Story verified; standard iceberg exemplar. |
| work-detached-jealousy | Jealousy (La Jalousie, 1957) | Alain Robbe-Grillet | External focalization; camera-eye catalog; metonymic surface imagery | Novel verified; the unnamed observing eye is the standard illustration. |
| work-detached-shiki-selected-poems | Masaoka Shiki: Selected Poems (1997) | Masaoka Shiki (trans. Burton Watson) | Shasei: plain observed-fact juxtaposition; affect left to inference | Edition verified (Columbia University Press). Translation of haiku/tanka; scope to the translation for English claims. |
| work-detached-luxun-call-to-arms | Call to Arms / Nahan (1923) | Lu Xun | Baimiao plain-line description; cool observational distance | Collection verified. Chinese original not inspected directly; baimiao mechanism attested in criticism — treated as limited for passage-level claims. |

No copyrighted passages are reproduced anywhere in this dossier.

**Cross-work pattern.** The four prose exemplars (Camus, Manto, Hemingway, Robbe-Grillet) achieve the same reader effect by different formal routes: Camus by first-person procedural report, Manto by third-person declarative reportage, Hemingway by objective dialogue, Robbe-Grillet by an observing eye. The constant is not a syntax but a *relationship between selection and omission* — a concrete surface that omits the named feeling while retaining the event that licenses the inference. The two poetic exemplars (Shiki, Lu Xun's baimiao) extend the same relationship to the image. This is why the tone card should teach the ratio, not a house style.

## G. Failure and misuse research

**G1. Emotional flatline (absence mistaken for restraint).**
- **Mechanism:** the writer omits affect but has not supplied inferable material beneath it.
- **Example:** a scene of a death reported only as movement and administration, with no selected detail and no consequence legible to the reader.
- **Effect:** reader cannot reconstruct what anyone feels; the scene reads as hollow (Hemingway's "hollow places").
- **Diagnostic:** after the passage, can the reader state what the character wanted and what it cost? If not, nothing was withheld — something was missing.
- **Revision action:** keep the neutral surface but add one concrete charged object or consequence (`clm-tone-detached-restraint-vs-absence`, `clm-tone-detached-defamiliarization`).
- **Scope:** never a failure in procedural or documentary writing whose contract is information alone.

**G2. Roboticism (machine-sounding flatness).**
- **Mechanism:** uniform sentence length and frame, generic assertion, and the absence of any foregrounded detail — the surface signature of the structural-tells catalog.
- **Example:** a paragraph of near-equal declaratives with abstract nouns ("the situation was difficult") and no specific object.
- **Effect:** no foregrounding → no affect (Miall & Kuiken); reads as committee voice / automated text.
- **Diagnostic:** measure sentence-length variance; scan for the catalog rows *Uniform sentence length*, *Uniform sentence frame*, *Committee voice*, *Generic significance*.
- **Revision action:** vary syntax to foreground one idea; replace each abstraction with a specific (number, name, object); keep the neutral register.
- **Scope:** note that surface tells are diagnostics, not proof; a deliberately even cadence can be craft when a specific detail carries the charge.

**G3. Manufactured neutrality (view-from-nowhere alibi).**
- **Mechanism:** a perfectly level voice conceals an unstated stance, presenting a judgment as fact.
- **Example:** atrocity described with the same cadence as weather, with no pressure distinguishing perpetrator from victim.
- **Effect:** reader senses a hidden angle and distrusts the narrator; at scale, numbing (Sontag 2003).
- **Diagnostic:** ask whose interests this neutrality serves; would a different victim/agent assignment read the same way?
- **Revision action:** change structure or consequence, not adjectives — let the event order reveal the asymmetry.
- **Scope:** In satire (Manto's mode), neutrality is the vehicle of a critique and is governed by the genre engine, not the tone alone.

**G4. Numbing at atrocity scale.**
- **Mechanism:** sustained detachment across extended violence trains the reader to look away.
- **Example:** a long sequence of clinically reported deaths with no change in distance.
- **Effect:** disengagement; empathy decreases under low transportation (Bal & Veltkamp 2013).
- **Diagnostic:** has psychic distance changed at any stakes peak? If flat across chapters, over-distance.
- **Revision action:** yield the tone at the peak — one close, sensory breach — then return. Cross-link `clm-melodrama-unearned-emotion` to avoid overshooting into sentimentality.
- **Scope:** documentary reportage may legitimately hold one plane throughout.

**G5. Mannered minimalism (restraint as costume).**
- **Mechanism:** the writer adopts the *look* of detachment — clipped sentences, brand names, withheld comment — because it signals seriousness, not because anything is withheld.
- **Example:** a passage of terse, unadorned declaratives whose only purpose is stylistic display; no stake changes and no charge is carried.
- **Effect:** the reader feels mannerism rather than discipline; the prose is admired as style but does not move.
- **Diagnostic:** remove the mannerisms and ask whether any meaning is lost; if the meaning survives unchanged, the style was costume.
- **Revision action:** either supply the buried charge the mannerism implies, or drop the mask and write the scene in the register its genre engine actually calls for.
- **Scope:** mannered minimalism is a recognized school with real practitioners; the failure is not the style but the absence of a reason for it in a given passage.

**Genre-overlap traps.** (a) *Deadpan*: flatness in service of comic effect — detached has no comic intent. (b) *Reflective*: inward, personal observation — detached is outward. (c) *Grim/cynical*: detachment with bleak weight or bitter irony is a hybrid, not this tone alone. (d) *Satirical mode*: Manto's detachment serves a target; the tone itself does not.

**AI-slop cross-link.** `references/structural-tells-catalog.md` applies hardest here. Crafted detachment and machine flatness can share a plain surface; they diverge on (i) selection — a specific, charged detail present vs absent; (ii) variability — purposeful variation vs uniform frames/lengths; (iii) accountability — an implied stance vs the "committee voice." A card must give the writer observable tests for all three (claim `clm-tone-detached-ai-slop-flatline`).

## H. Dosage and saturation findings

**Honest null — `evidence-incomplete`.** No experimental study located measures how long a reader will tolerate sustained affect-free narration before disengaging. Any numeric thresholds below are **writer-inference** built from the transportation findings in §B, not measured craft data, and are labeled as such for the card author.

**What the adjacent evidence supports.**
- Engagement requires emotional transportation (imagery + affect + attention); the low-transportation condition predicts reduced empathy over time (Green & Brock 2000; Bal & Veltkamp 2013). Detachment sustained without any affective anchor approximates that condition.
- Foregrounding is what evokes feeling; a text with no foregrounded element cannot, by that account, provoke it (Miall & Kuiken 1994).

**Working dosage guidance (writer-inference).**
- One sustained neutral passage per scene of roughly 600–900 words, then yield: a scene that changes stakes needs at least one charged concrete detail or one brief drop in psychic distance.
- Never carry the tone flat across two consecutive stake-changing scenes without a modulation bridge.
- At the story's climactic beat, detachment should yield entirely for a short passage; substitute briefly close psychic distance, one sensory intrusion, or a short turn toward `tone-reflective`/`tone-elegiac`, then return.
- A useful proportion signal: at least one *named or clearly inferable* stake or want per scene, and at least one concrete charged detail per ~500 words in extended detached passages. These are writer-inference, not measurements.
- In a work of sustained detachment, vary the distance across the whole piece: far for routine, mid for conflict, briefly close at the single peak. A flat distance line across a whole book is the signature of the failure modes below.

**Saturation signals (reader behavior → draft test).**
- Reader cannot summarize any character's motive or want after a scene → insufficient inferable material.
- Skimming of descriptive passages → cadence too uniform; add foregrounding.
- "So what?" reaction at an atrocity → over-distance; yield at the peak.
- Distrust of the narrator → manufactured-neutrality problem (G3).
- Reader describes the prose as "cold" or "flat" without describing any feeling it produced → the surface has consumed the affect it was meant to hold back.

**Modulation, not abandonment.** The tone yields rather than switches off. A single close sentence — one sensory intrusion, one physical reaction named, one object charged — can reset the reader's distance without importing sentimentality. The card should give the writer a *bridge* phrase pattern for the return to neutrality (a procedural sentence after the close beat), so the detachment reads as a recovered discipline rather than a lapse.

**Dosage by form.** In fiction the yield-point is the stakes peak; in essay/academic prose the tone can hold longer because the contract is argument and the "pulse" is carried by the claim sequence rather than by character feeling; in copy/marketing the tone should not be sustained at all beyond a headline or a single body sentence, where its coolness signals confidence rather than indifference.

**Reader-state caution.** Detachment depends on the reader already caring enough to do inferential work. In a cold open with no established stake, the tone cannot borrow an affect the reader has not yet invested; it should be introduced after the reader has a reason to lean in.

**Context prohibitions.** Do not use pure detachment where the genre engine's promise is grief, fear, or love and no modulation is planned; do not deploy it to render a victim's suffering without supplying the reader an inferable moral footing (G3/G4).

## I. Source records

All sources, claims, and primary works referenced above are written as JSON records in this silo. Shared registries are **not** edited here. Cross-linked read-only claims: `clm-point-of-view-psychic-distance`, `clm-melodrama-unearned-emotion`, `clm-dhvani-suggestion-theory`, `clm-rasa-emotional-aesthetic`, `clm-pacing-rhythm-syntax`, `clm-showing-telling-balance`.

- Sources: `src-detached-*` (19 records).
- Claims: `clm-tone-detached-*` (10 records).
- Primary works: `work-detached-*` (6 records).

Shared cross-links are read-only and not re-registered here: `clm-point-of-view-psychic-distance` (distance modulation), `clm-melodrama-unearned-emotion` (the sentimentality pole), `clm-dhvani-suggestion-theory` and `clm-rasa-emotional-aesthetic` (Indian suggestion/affect theory), `clm-pacing-rhythm-syntax` (cadence), `clm-showing-telling-balance` (summary/scene rhythm).
