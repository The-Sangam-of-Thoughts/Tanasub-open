# Reverent — Research Dossier

- Tone ID: `tone-reverent`
- Family: Elevation
- Researched: 2026-09-24
- Evidence status: complete

Scope of this tone: the narrator's voice holds **awe and sacred attention toward
something treated as holy or profound**. Stakes still belong to the genre engine;
the reverent voice owns texture only. The boundary the repository enforces:
`tone-grim` carries weight without awe, and `tone-lyrical` prizes the beauty of
the language itself rather than devotion to an object. The reverent voice makes
the *object* — a god, a dead, a landscape, a body of knowledge, a moral absolute —
larger than the speaker, and it declines to reduce that object to a slogan.

Nearest neighbours: `tone-grim` (weight, no awe), `tone-lyrical` (aesthetic sound,
not devotion), `tone-inspirational` (forward possibility, not present awe),
`tone-philosophical` (ideas as subject, not a held-holy object).

## A. Claims matrix

| claim_id | claim | tier | locator | scope | confidence |
|---|---|---|---|---|---|
| clm-tone-reverent-awe-vastness-accommodation | Awe is an epistemic emotion triggered by perceived vastness that forces accommodation of existing mental schemas. | 2 | Keltner & Haidt 2003, *Cognition & Emotion* 17(2):297–314 | Descriptive appraisal of awe stimuli; basis for scaling the sacred object | strong |
| clm-tone-reverent-small-self | Awe diminishes self-focus (the "small self") and shifts attention toward the collective; the small self is not the sole mediator of its prosocial effects. | 1 | Piff et al. 2015, *JPSP* 108(6):883–899; Perlin & Li 2020, *Perspectives on Psych. Science* 15(2):291–308; Ramanujan trans. 1973, *Speaking of Śiva* (vachana speakers dissolve the "I" into the named lord) | Psychic-distance operator; first-person retreat before the object | strong |
| clm-tone-reverent-numinous-wholly-other | The religious feeling is a *sui generis*, non-rational state — the numinous — whose object is the "wholly other," experienced as *mysterium tremendum et fascinans*. | 2 | Otto 1923 (trans. Harvey), *The Idea of the Holy*, chs. II–VI | Recognition criterion for a genuinely sacred object vs borrowed solemnity | strong |
| clm-tone-reverent-apophatic-construal | Negative (apophatic) construal — saying what the sacred is *not* — conveys religious awe better than positive description, and is theorized as a psychological contribution to awe. | 2 | Otto 1923, chs. IV–V; Sundararajan 2002, *J. Theoretical & Philosophical Psychology* 22(2):174–197 | Figuration and lexicon for the unnameable | moderate |
| clm-tone-reverent-sublime-cadence | Grandeur is produced by elevated thought married to figured, rhythmically suspended composition that "transports" the hearer beyond persuasion. | 1 | [Pseudo-]Longinus 1964 (Russell), *On the Sublime*, §§ I, VIII–IX; Burke 1757, *Enquiry*, Part II | Cadence and periodic syntax operators | strong |
| clm-tone-reverent-sacred-vs-threat-awe | Threat-based awe (fear, power, submission) is a distinct variant from positive awe; reverent narration must not collapse into dread, which is the `tone-grim` surface. | 2 | Gordon et al. 2017, *JPSP*, DOI 10.1037/pspp0000120; Keltner & Haidt 2003 | Boundary test against `tone-grim` and horror engines | moderate |
| clm-tone-reverent-bhakti-named-address | Devotional poetics works through named, personal address (the *ankita*) rather than abstract adoration; the deity is an interlocutor, not a theme. | 1 | Rūpa Gosvāmī, *Bhaktirasāmṛtasindhu*; Ramanujan trans. 1973, *Speaking of Śiva* | Vocative operator; Indian/regional anchor | strong |
| clm-tone-reverent-rasa-dhvani-suggestion | Sacred resonance is carried by suggested meaning (*dhvani*) resolving into a dominant aesthetic emotion (*rasa*), not by literal statement. | 1 | Nāṭyaśāstra (Ghosh 1951), ch. 6; Ānandavardhana (Ingalls et al. 1990), Uddyota 1 | Non-literal figuration; cross-link `clm-dhvani-suggestion-theory` | strong |
| clm-tone-reverent-embodied-sacred | Bhakti and Vīraśaiva traditions locate the sacred in the body, labour, and named place; the ethereal "hushed" register is a Western default, not a universal. | 1 | Ramanujan trans. 1973, *Speaking of Śiva*; *vachana*s of Basava and Akka Mahādevī | Concrete-image operator; anti-universal scope; cross-link `axis-vachana-poetry` | strong |
| clm-tone-reverent-translation-limits | Claims about sacred lexicon, vocables, and cadence do not survive translation intact; universalist English renderings can flatten devotional specificity. | 1 | Niranjana 1992, *Siting Translation*; Ramanujan trans. 1973 (translator's note); Zeami 1984 (Rimer/Yamazaki) | Scope limit on all cross-cultural mechanism claims | moderate |
| clm-tone-reverent-yugen-suggestion | Japanese *yūgen* holds that profundity is suggested, not stated — what is left unspoken is part of the meaning. | 1 | Zeami 1984 (Rimer & Yamazaki), *On the Art of the Nō Drama*, *Kadensho* | Silence and brevity operator; second non-Anglophone anchor | strong |
| clm-tone-reverent-liturgical-parallelism | Parallelism and anaphora encode ritual cadence and make a passage memorable and choral, not merely emphatic. | 1 | Alter 1985, *The Art of Biblical Poetry*, chs. 1–3; Rumi, *The Mathnawi of Jalalu'ddin Rumi* (Nicholson ed. & trans. 1925–1940), refrain and paired figure | Anaphora/parallel-series operator | moderate |
| clm-tone-reverent-failure-borrowed-gravity | A sacred register applied to a non-sacred object yields false solemnity and unearned profundity; vacuous profundity is measurably distinguishable from meaningful depth. | 2 | Pennycook et al. 2015, *Judgment & Decision Making* 10(6):549–563; cross-link `clm-melodrama-unearned-emotion` | Failure mode §G; feeds card §7 | moderate |
| clm-tone-reverent-dosage-yield | Sustained awe habituates and, under threat framing, curdles; the voice must yield to plain register at stakes peaks and does not travel intact across cultures. | 2 | Katz & Franz 2026, *American Psychologist* 81(1):82–93; Perlin & Li 2020; Gordon et al. 2017 | Dosage/saturation; feeds card §4 | moderate |

Every row resolves to a record in `claims/`.

**Evidence grade (honesty note).** No experimental study isolates a "reverent
narrative voice" as an independent variable; the psychological claims above
concern awe and the numinous as reader states, and are imported as adjacent
findings, not as direct proof of a prose technique. The craft claims (bhakti,
rasa/dhvani, *yūgen*, sublime) are anchored in primary poetics and verified
exemplars. Where translation blocks an acoustic claim, the claim is scoped to
structure rather than sound.

## B. Cognitive and psychological foundations

**Awe: vastness and accommodation (Keltner & Haidt 2003).** Keltner and Haidt
define awe as an *epistemic* emotion — one that arises when an encounter falls
outside existing cognitive schemas and prompts reappraisal — and name two
necessary features: *perceived vastness* and *need for accommodation*. They
propose an evolutionary root ("primordial awe" before powerful others) that
generalizes to spiritual experience, grand nature, art, music, and grand theory,
and they list five "flavours" that colour it: threat, beauty, ability, virtue,
and the supernatural. Craft consequence: the sacred object must be rendered
*vast enough to exceed the frame*; a god or a truth described only in comfortable
domestic terms will not produce awe (`clm-tone-reverent-awe-vastness-accommodation`).

**Counterevidence / cultural limit (Katz & Franz 2026).** Katz and Franz argue
that awe still lacks an uncontested definition, that "vastness" as a necessary
feature has caused neglect of the full range of awe experiences, and — most
important here — that there is "very little scientific knowledge about
differences in awe across various languages, cultures, and time periods." The
dossier therefore treats the Western awe construct as one bounded account, not a
universal grammar of the sacred (`clm-tone-reverent-dosage-yield`).

**Small self (Piff et al. 2015; Perlin & Li 2020).** Across five studies Piff
and colleagues found that awe reduces the emphasis on the individual self — the
"small self" — and increases prosocial behaviour, ethical decision-making, and
identification with collectives. Perlin and Li's review complicates the
mechanism: the small self is not the only route to awe's prosocial effects, and
the construct risks over-simplification. Craft consequence: the reverent
narrator recedes — uses fewer first-person claims, yields the frame to the object
— but the mechanism is not a formula (`clm-tone-reverent-small-self`).

**The numinous (Otto 1923).** Otto names the *numinous* as a non-rational,
non-sensory state whose object is *ganz Andere* — "wholly other" — and analyses
it as *mysterium tremendum et fascinans*: a mystery that is at once daunting
(*tremendum*) and compelling (*fascinans*). The state is *sui generis* and
"incomparable," not reducible to ethics or reason. This is the dossier's
recognition criterion: a reverent passage is aimed at something its speaker
genuinely experiences as beyond full grasp, not at a value the speaker merely
endorses (`clm-tone-reverent-numinous-wholly-other`).

**Apophatic construal (Otto 1923; Sundararajan 2002).** Otto observes that the
numinous resists positive description and is approached through negation and
"ideograms." Sundararajan argues that negative theology offers a genuine
psychological contribution to the study of religious awe: what cannot be
predicated can still be gestured toward. Craft consequence: the strongest
reverent figuration often removes attributes rather than adding them
(`clm-tone-reverent-apophatic-construal`).

**Threat-based awe (Gordon et al. 2017).** Gordon, Stellar, Anderson, McNeil,
Loew, and Keltner distinguish a threat-based variant of awe from positive awe;
threat-based awe is associated with feelings of fear, diminished sense of control,
and submission, and is not reliably prosocial. This is the dossier's boundary
evidence: reverent narration may include dread as an edge, but if submission to
power dominates, the voice has slid into `tone-grim` or horror
(`clm-tone-reverent-sacred-vs-threat-awe`).

## C. Rhetorical and literary tradition

**Classical sublime.** The Roman-era Greek treatise *On the Sublime* (author
uncertain, conventionally "Pseudo-Longinus") treats grandeur as the product of
elevated thought and "figured" composition that transports the listener rather
than persuading them; it analyses the grand style's rhythms, its use of
amplification and hyperbaton, and its capacity to leave an audience "struck."
Edmund Burke's *Enquiry* (1757) splits the sublime from the beautiful and ties it
to terror and obscurity; Kant's *Critique of Judgment* (1790) formalizes the
sublime as the mind's reaction when imagination fails before magnitude or power.
This tradition supplies the cadence and scale operators
(`clm-tone-reverent-sublime-cadence`). What remains contested: whether the
sublime is an aesthetic category separable from religious awe; this dossier uses
it as a craft lineage, not as a synonym.

**Devotional verse and the liturgical voice.** From the Hebrew psalter's
parallelism to Christian liturgy and the *Four Quartets*, devotional writing
organizes itself by repetition and cadence. Robert Alter's *The Art of Biblical
Poetry* (1985) shows that biblical parallelism is not mere redundancy but a
systematic semantic movement — second lines intensify, specify, or complicate the
first — which gives ritual language its forward pressure
(`clm-tone-reverent-liturgical-parallelism`).

**Modern drift.** The reverent register migrates from liturgy and scripture into
secular elegy, nature writing, science writing, and memorial prose. What changed:
the warrant shifts from divine to existential or civic, while cadence and
apophatic reserve persist. The open hazard is "borrowed gravity" — importing the
sound of devotion with no object worthy of it (§G).

## D. Craft mechanism inventory

Every item is tied to a named source or a verified exemplar. Exemplar techniques
are described, never quoted.

| technique | why it works (source) | verified exemplar use (described) |
|---|---|---|
| Vast object framing | Awe requires perceived vastness exceeding schemas (Keltner & Haidt 2003) | *Four Quartets* repeatedly sets a single moment against the scale of all time; the temporal frame dwarfs the speaker |
| First-person retreat / small self | Awe de-emphasizes the self (Piff et al. 2015) | Akka Mahādevī's *vachana*s dissolve the speaker into the named lord; the "I" is consumed, not centre-stage |
| Apophatic construal (via negativa) | The numinous resists positive predication (Otto 1923; Sundararajan 2002) | *Four Quartets* describes illumination by stripping away image after image rather than depicting it |
| Named address / *ankita* | Devotion is personal, directed, and named (Rūpa Gosvāmī; Ramanujan 1973) | Basava's *vachana*s close on a specific lord ("Lord of the Meeting Rivers"), making the address structural, not decorative |
| Embodied concrete image | Bhakti locates the sacred in body and labour (Ramanujan 1973) | Basava's temple built of the living body; Allama Prabhu's impossible *bedagu* images that defy paraphrase |
| Periodic / suspended cadence | Grandeur is produced by figured, rhythmic composition (Longinus; Burke) | *Four Quartets*' long accumulating sentences that suspend closure until a quiet, weighed final clause |
| Parallelism and anaphora | Ritual repetition encodes cadence and intensifies meaning (Alter 1985) | The psalter's paired lines and the *Masnavi*'s refrains build choral pressure |
| Figurative height / light / stillness | Sublime and numinous imagery of magnitude and radiance (Longinus; Otto) | *Four Quartets*' "still point," its rose and fire imagery; Rumi's sun and ocean figures for the divine |
| Psychic distance widening | Awe shifts attention outward, away from self (Piff et al. 2015; Keltner & Haidt 2003) | Nature/scriptural passages that withdraw the narrator and let the object occupy the sentence |
| Silence, brevity, aposiopesis | Profundity is suggested, not stated (*yūgen*, Zeami 1984) | Nō's dramatic theory prizes the unspoken and the "flower" of restrained gesture; a verse that stops before explanation |
| Self-lowering / *kenosis* | Devotional self-humbling before the object (Rūpa Gosvāmī; Rumi) | Rumi's reed-flute lament frames the speaker as separated and small before union; Sufi *fanā* (annihilation) imagery |

## E. Cross-cultural survey

**Indian / Kannada — Vīraśaiva *vachana* (load-bearing; cross-link
`axis-vachana-poetry`).** A.K. Ramanujan's *Speaking of Śiva* (Penguin, 1973)
translates the 12th-century Kannada *vachana*s of Basava, Akka Mahādevī, Allama
Prabhu and others. The form's engine is *anubhava* (direct experience) and the
*ankita* — a closing, named invocation of the poet's deity (Basava's "Lord of the
Meeting Rivers"; Akka Mahādevī's "Lord, white as jasmine"). Devotion here is
embodied and confrontational, not hushed: the body is the temple, labour is
worship, and the speaker scolds or loves the divine directly. This matters for
the tone boundary: a Western "devotional hush" is only one register of the
sacred (`clm-tone-reverent-bhakti-named-address`, `clm-tone-reverent-embodied-sacred`).

**Indian / Sanskrit — rasa and dhvani (load-bearing).** Bharata's *Nāṭyaśāstra*
(Ghosh trans., 1951) makes *rasa* the emotional relish produced by the
combination of determinants, consequents, and transient states; a sustained
dominant state (*sthāyi bhava*) organizes the work. Ānandavardhana's
*Dhvanyāloka* (Ingalls, Masson & Patwardhan, 1990) argues that *dhvani* —
suggested meaning — is the soul of poetry, surpassing literal statement. For the
reverent voice this supplies the non-literal operator: the sacred is *suggested*
into being, not defined (`clm-tone-reverent-rasa-dhvani-suggestion`; cross-link
shared `clm-rasa-emotional-aesthetic`, `clm-dhvani-suggestion-theory`). Rūpa
Gosvāmī's *Bhaktirasāmṛtasindhu* later systematizes *bhakti* as a distinct rasa,
with the deity as the supreme object of aesthetic-devotional relish.

**Persian / Sufi — Rumi's *Masnavi* (load-bearing).** Rumi's *Masnavi* (13th c.;
R. A. Nicholson's critical translation, Gibb Memorial, 1925–40) turns anecdote
into sacred instruction, moving from homely story to ecstatic figure — the reed
cut from its bed, the sun, the ocean — and framing union as self-annihilation.
The mechanism is the same family as *yūgen* and *dhvani*: meaning is carried by
figure and suggestion, not proposition.

**Japanese — *yūgen* and Nō (load-bearing).** Zeami's treatises (*Kadensho*;
Rimer & Yamazaki, Princeton UP, 1984) theorize *yūgen* as "profound grace and
subtlety" — the beauty of what is only suggested, of gesture and shadow. Zeami's
images of a boat vanishing behind islands or shadows of bamboo on bamboo show a
sacred-profound register that trusts omission. This is the dossier's second
non-Anglophone anchor and a counterweight to declarative awe
(`clm-tone-reverent-yugen-suggestion`).

**Translation limits (explicit).** Vīraśaiva cadence, *bedagu* wordplay, and
occupational register are Kannada-bound; Ramanujan's English necessarily flattens
them, and Tejaswini Niranjana's *Siting Translation* (1992) critiques such
renderings for producing a "universalist" poetry consumable by the West. Sanskrit
technical terms (*rasa*, *dhvani*, *bhakti*) resist single-word English
equivalents. *Yūgen*'s acoustic and imagistic texture is not fully recoverable in
English. Accordingly, all mechanism claims above are scoped to structure and
function, not to sound or exact lexical equivalence
(`clm-tone-reverent-translation-limits`).

## F. Exemplar field

| work_id | work | creator | mechanism demonstrated | verification note |
|---|---|---|---|---|
| work-four-quartets | *Four Quartets* (1943) | T. S. Eliot | vast temporal framing, apophatic stripping, suspended cadence, "still point" imagery | Publication and structure verified (Harcourt/Faber, collected 1943); technique described from criticism; **no text reproduced** (copyrighted) |
| work-speaking-of-siva | *Speaking of Śiva* (1973) | A. K. Ramanujan (trans.); Basava, Akka Mahādevī, Allama Prabhu et al. | named *ankita*, embodied sacred, *bedagu* paradox, direct address | Penguin Books, 1973, ISBN 9780140442700, verified via Open Library; described from translator's framing and scholarship; no passages reproduced |
| work-masnavi | *Masnavi* (13th c.) | Rumi; R. A. Nicholson (trans.) | figure-mediated instruction, ecstatic figure, self-annihilation, refrain | Nicholson critical translation, Gibb Memorial, 1925–40, verified; described structurally; no passages reproduced |
| work-ramcharitmanas | *Rāmcharitmānas* (16th c.) | Tulsidas | vocative devotion, rhythmic verse cadence, sacred narrative sequence | Gita Press editions verified via Open Library; described from form and reception; translation limits noted; no passages reproduced |

## G. Failure and misuse research

**Borrowed gravity / false solemnity.** The arch-failure: importing the sound of
devotion — elevated diction, slow cadence, archaic pronouns — when the object is
a product, a brand, or a trivial observation. The prose performs awe it has not
earned. The mechanism is a mismatch between register and object, and it is the
same defect as unearned emotion in fiction
(cross-link `clm-melodrama-unearned-emotion`).

**Unearned profundity (pseudo-profound language).** Pennycook and colleagues
(2015) showed that people rate syntactically well-formed but semantically empty
"bullshit" statements as profound, and that low reflectiveness predicts greater
receptivity; they also found that such statements are distinguishable from
genuinely meaningful ones. Craft consequence: vagueness and abstraction are not
depth signals; a reverent passage that survives paraphrase-testing as empty is a
failure (`clm-tone-reverent-failure-borrowed-gravity`).

**Threat collapse.** If the sacred object is rendered chiefly as a power that
subjugates — punishment, inescapable judgement, terror without *fascinans* — the
threat variant of awe dominates and the voice becomes `tone-grim` or horror
(Gordon et al. 2017). The Fascinans is what keeps it reverent.

**Museumification.** Rendering the object inert: treating a living devotional
tradition as static antique décor. The *vachana* genre file documents the parallel
failure for its own form — abstract universalism that strips the Sharana
movement's named anti-caste protest into "generic spiritual sentiment."

**Kitsch solemnity.** Repetition of sacred cadence until it reads as parody or
advertising. Saturation signals in §H.

## H. Dosage and saturation findings

1. **Awe habituates and its definitions are culturally bounded.** Katz and Franz
   (2026) note contested definition and cross-cultural incommensurability; a
   sustained reverent register is neither universally legible nor indefinitely
   potent. Practical threshold: reserve the full register for one constituted
   passage per section; do not hold it continuously.
2. **Threat framing curdles awe.** Gordon et al. (2017): threat-based awe is
   distinct and not reliably prosocial. When the material is genuinely about
   danger or loss, the tone must yield to `tone-grim` or `tone-elegiac`.
3. **The small-self mechanism is not a formula.** Perlin and Li (2020) warn that
   the "small self" is not the sole mediator of awe's effects. Dosage rule: do not
   reduce the speaker to a repeated negation ("I am nothing") as a substitute for
   rendering the object.
4. **Where the tone must yield.** At stakes peaks and in direct address of
   suffering, drop to unadorned or compassionate register; when the matter is a
   real deadline, `tone-urgent`; when the subject is possibility rather than
   presence, `tone-inspirational`.
5. **Saturation signals.** (a) Two or more consecutive sentences of elevated
   diction with no new concrete particular; (b) abstract nouns outnumbering
   concrete and named things; (c) the sacred object's specific attributes
   removable without loss; (d) the passage still "works" if read as an
   advertisement; (e) a passage that collapses under the paraphrase test of
   Pennycook et al. (2015).

## I. Source records

Claims: `clm-tone-reverent-awe-vastness-accommodation`,
`clm-tone-reverent-small-self`, `clm-tone-reverent-numinous-wholly-other`,
`clm-tone-reverent-apophatic-construal`, `clm-tone-reverent-sublime-cadence`,
`clm-tone-reverent-sacred-vs-threat-awe`, `clm-tone-reverent-bhakti-named-address`,
`clm-tone-reverent-rasa-dhvani-suggestion`, `clm-tone-reverent-embodied-sacred`,
`clm-tone-reverent-translation-limits`, `clm-tone-reverent-yugen-suggestion`,
`clm-tone-reverent-liturgical-parallelism`,
`clm-tone-reverent-failure-borrowed-gravity`, `clm-tone-reverent-dosage-yield`.

Sources: `src-reverent-keltner-haidt-2003`, `src-reverent-piff-2015`,
`src-reverent-perlin-li-2020`, `src-reverent-otto-idea-holy-1917`,
`src-reverent-sundararajan-2002`, `src-reverent-gordon-2017`,
`src-reverent-katz-franz-2026`, `src-reverent-longinus-russell-1964`,
`src-reverent-burke-sublime-1757`, `src-reverent-kant-judgment-1790`,
`src-reverent-rupa-goswami-brs`, `src-reverent-ramanujan-speaking-of-siva-1973`,
`src-reverent-niranjana-siting-translation-1992`,
`src-reverent-zeami-rimer-yamazaki-1984`, `src-reverent-alter-biblical-poetry-1985`,
`src-reverent-pennycook-pseudo-profound-2015`,
`src-reverent-rumi-nicholson-masnavi`.

Shared sources cited read-only (registered by coordinator):
`src-natyashastra-ghosh-1951`, `src-anandavardhana-dhvanyaloka-1990`.

Primary works: `work-four-quartets`, `work-speaking-of-siva`, `work-masnavi`,
`work-ramcharitmanas`.

Cross-links (read-only, shared claims): `clm-rasa-emotional-aesthetic`,
`clm-dhvani-suggestion-theory`, `clm-melodrama-unearned-emotion`,
`clm-point-of-view-psychic-distance`, `clm-pacing-rhythm-syntax`.

Genre cross-link: `axis-vachana-poetry` (`genres/vachana-poetry.md`).

Shared registries are not edited here; registration is the coordinator's step.
