# Comedic — Research Dossier

- Tone ID: `tone-comedic`
- Family: Humor
- Researched: 2026-09-24
- Evidence status: complete (3 items flagged evidence-incomplete, see §I)

Scope note: this dossier follows the frozen boundary in
`docs/architecture/tone-taxonomy.md`. Comedic humour is carried by content and
structure (setup/payoff, escalation, wordplay). It differs from `tone-deadpan`
(where humour lives in flat delivery) and from the `satirical-literature` mode
(which critiques a specific target). Many real comic texts also satirize; where
an exemplar straddles the boundary, that is recorded rather than hidden.

## A. Claims matrix

| claim_id | claim | tier | locator | scope | confidence |
|---|---|---|---|---|---|
| clm-tone-comedic-incongruity-resolution | Comic effect peaks when a violated expectation is resolved into a second, compatible frame. | 2 | Suls 1972, `src-comedic-suls-1972`, ch. 4, pp. 81–100 | Jokes and short comic structures in all forms | strong |
| clm-tone-comedic-benign-violation | Humour requires a simultaneous violation and a benign framing; if the threat is not made benign, amusement collapses into offence. | 2 | McGraw & Warren 2010, `src-comedic-mcgraw-warren-2010`, Studies 1–5 | Humour across moral/social content | strong |
| clm-tone-comedic-superiority-limits | Superiority/mockery explains only part of humour and fails when the audience identifies with a non-benign target. | 2 | Lintott 2016, `src-comedic-lintott-superiority-2016`; Ford & Ferguson 2004, `src-comedic-ford-ferguson-2004` | Humour aimed at persons/groups | moderate |
| clm-tone-comedic-comic-distance | Laughter requires a degree of emotional distance; too much proximity to real stakes suppresses the comic response. | 2 | Bergson 1900, `src-comedic-bergson-laughter-1900`, ch. I | Craft control of psychic distance | strong |
| clm-tone-comedic-escalation-heightening | Comic scenes intensify by repeating and heightening one rule or game rather than adding unrelated jokes. | 2 | Halpern, Close & Johnson 1994, `src-comedic-halpern-truth-comedy-1994` (practitioner); Suls 1972, `src-comedic-suls-1972`, ch. 4 (incongruity-resolution mechanism) | Scene/section construction | moderate |
| clm-tone-comedic-density-saturation | Humorous material has a workable density band; excess comic detail crowds the substantive point (seductive-details effect). | 2 | Harp & Mayer 1998, `src-comedic-harp-mayer-1998`; double 2005, `src-comedic-double-standup-2005` | Blog/marketing, academic, long-form | moderate |
| clm-tone-comedic-hasya-rasa | Classical Indian poetics names the comic as a primary rasa (hasya) with its own causes, expressions, and graded laughter, and institutionalizes it in the Vidushaka clown. | 1 | Natyashastra (Ghosh 1951), shared `src-natyashastra-ghosh-1951`, ch. 6 | Indian/regional tradition; cross-cultural validity | strong |
| clm-tone-comedic-crosscultural-oral | Non-Anglophone oral comic traditions (Japanese rakugo, Chinese xiangsheng) carry humour through performed timing, character voice, and patterned sound, not only verbal content. | 2 | Shores 2021, `src-comedic-shores-rakugo-2021`; Lawson 2020, `src-comedic-lawson-xiangsheng-2020` | Cross-cultural survey; translation limits | moderate |
| clm-tone-comedic-figurative-register | Understatement and hyperbole work by violating register or scale expectations; wordplay works by exploiting an unexpected second sense of a word or phrase. | 2 | Suls 1972, `src-comedic-suls-1972`; Bergson 1900, `src-comedic-bergson-laughter-1900`; exemplars Wodehouse, Pratchett | Prose and copy; figurative moves | moderate |
| clm-tone-comedic-disparagement-harm | Disparagement humour aimed downward can normalize prejudice in audiences; this is a documented ethical and craft failure, not merely taste. | 2 | Ford & Ferguson 2004, `src-comedic-ford-ferguson-2004`; McTernan 2024, `src-comedic-mcternan-punching-down-2024` | Humour targeting persons/groups | strong |

Every row resolves to a record in `claims/`.

## B. Cognitive and psychological foundations

Three classical families of theory recur across the literature: superiority,
relief, and incongruity (Morreall, `src-comedic-morreall-sep-2012`, §1–3).
Morreall's synthesis treats each as partial: superiority captures mockery, relief
captures tension discharge, incongruity captures the perception of something
that clashes with expectation. No single family is a general theory, so a card
should not present one as the whole explanation.

**Incongruity-resolution.** Suls's two-stage information-processing model holds
that a joke first disconfirms an expectation, then requires the hearer to find a
rule that makes the punchline fit (`src-comedic-suls-1972`, pp. 81–100). The
comic payoff is therefore not mere surprise; it is surprise plus a recoverable
second frame. Craft consequence: a punchline that cannot be resolved into a new
frame reads as randomness or nonsense rather than humour (see
`clm-tone-comedic-incongruity-resolution`; cf. shared `clm-suspense-vs-surprise`).

**Benign violation.** McGraw and Warren argue humour occurs when something is
simultaneously a violation (of norms, expectations, or identity) and benign
(`src-comedic-mcgraw-warren-2010`, Studies 1–5). They identify three routes to
benign-ness: an alternative norm, a large psychological distance, or a weak
commitment to the violated norm. Craft consequence: the same content can be
funny or offensive depending on framing and distance, which makes framing a
craft decision, not an accident (`clm-tone-comedic-benign-violation`).

**Superiority and its limits.** Superiority theories (Plato, Hobbes) explain
laughter as delight in another's inferiority, but Lintott argues the theory
captures only a subset of humour (`src-comedic-lintott-superiority-2016`).
Ford and Ferguson show that disparagement humour has measurable social effects,
including activating prejudiced norms (`src-comedic-ford-ferguson-2004`). See
`clm-tone-comedic-superiority-limits` and §G.

**Distance.** Bergson's public-domain essay makes "absence of feeling" a
condition of laughter: indifference is laughter's "natural environment," and
emotion is its enemy (`src-comedic-bergson-laughter-1900`, ch. I). This is the
psychological basis for psychic distance as a comic dial
(`clm-tone-comedic-comic-distance`) and links to the shared craft claim
`clm-point-of-view-psychic-distance`.

**Why flatness works (neighbour disambiguation).** A neutral or flat surface can
carry comic content because the incongruity is generated by the content, while
the delivery refuses to signal it; that is the deadpan mechanism, not this tone's
(see `tone-deadpan`). Comedic, by contrast, actively stages the setup–payoff
machinery in the language itself.

**Timing.** Practitioner work on stand-up treats the pause before a punchline as
a tension-builder that the punchline then releases (Double,
`src-comedic-double-standup-2005`). This is Tier 4 practitioner testimony; it is
triangulated with the incongruity and relief theories rather than used as sole
support for a consequential claim.

## C. Rhetorical and literary tradition

Comic theory has a long lineage. Superiority accounts run from Plato and
Aristotle to Hobbes; relief accounts from Spencer to Freud; incongruity accounts
from Kant and Schopenhauer through Kierkegaard and Koestler's bisociation
(Morreall, `src-comedic-morreall-sep-2012`, §1–4). Bergson added a social-
corrective reading: laughter is a social gesture that checks mechanical
inelasticity in conduct (`src-comedic-bergson-laughter-1900`, ch. I). What
remains contested is whether any of these is primary; the honest position for a
card is plural and mechanism-first.

The essayistic humorous voice (the personal comic essay, the light column, the
comic memoir) and the comic novel both rest on the same machinery: an
incongruity staged within a controlled, unpanicked narrator. P. G. Wodehouse is
the canonical English prose stylist of this mode: elaborate, mock-formal
narration; mixed-register diction; and a plot built as escalating farce rather
than a sequence of discrete gags (see `work-wodehouse-code-woosters`; the
contemporary critical reception is recorded by the *New Criterion* and the
*European Journal of English Studies* essays located in §I).

Terry Pratchett shows the same machinery inside speculative fiction: comic
repetition, mock-heroic register, and a wide-angle satirical narrator; scholars
note that his comedy is more often "heavy" structural repetition than incidental
lightness (`work-pratchett-guards-guards`). Pratchett's work also targets
institutions, so it overlaps the satirical-literature mode; the card should
describe the comedic machinery without claiming he is target-free.

Indian comic writing is a major modern strand: Harishankar Parsai (Hindi,
1924–1995) and Rajshekhar Basu "Parashuram" (Bengali, 1880–1960) are the two
most-cited modern humorists in their languages (see §E and §F). Both work in the
`vyangya` / satirical-comic essay and short story, meaning they again straddle
the comedic/satire boundary.

## D. Craft mechanism inventory

Each entry names the technique, why it works by the mechanism claims above, and a
verified exemplar that uses it (described, never quoted).

| # | Technique | Why it works | Verified exemplar |
|---|---|---|---|
| D1 | Setup–turn (misdirection then resolution) | Incongruity-resolution: expectations are built and then re-framed | Suls model (`clm-tone-comedic-incongruity-resolution`); Wodehouse's Jeeves plots build a false reading before the reveal |
| D2 | Escalation / heightening of one rule | Repeating a game and raising stakes per beat concentrates the incongruity | Halpern et al. practice (`clm-tone-comedic-escalation-heightening`); `work-wodehouse-code-woosters` farce escalation |
| D3 | Rule of three (two pattern beats + a turn) | The third term resolves/ruptures an established pattern | Morreall on pattern (SEP); confirmed as a stated principle in practitioner comedy manuals (practitioner record card, §D note) |
| D4 | Understatement / litotes | Violates scale expectation: a large event is named with a small phrase | Bergson on incongruity (`clm-tone-comedic-figurative-register`); Wodehouse narration |
| D5 | Hyperbole / mock-formal inflation | Violates scale in the other direction; clashes diction with subject | Pratchett's mock-heroic narration (`work-pratchett-guards-guards`) |
| D6 | Wordplay / double sense | A phrase activates an unexpected second script, then resolves | Suls script resolution (`clm-tone-comedic-incongruity-resolution`); Wodehouse's mixed-register diction |
| D7 | Comic distance and unpanicked narrator | Absence of feeling is a condition of laughter; narrator refuses alarm | Bergson (`clm-tone-comedic-comic-distance`); Wodehouse's Bertie-register narration |
| D8 | Comic repetition / running motif | A returning phrase or object re-activates a known frame and inverts it | Shores on rakugo repetition (`clm-tone-comedic-crosscultural-oral`); Pratchett's recurrence devices |
| D9 | Concrete, low-register imagery against high subject | Register clash produces the incongruity | Bergson; Parsai's bureaucratic-mundane imagery (`work-parsai-inspector-matadeen`) |
| D10 | Paragraph/section shape: short build, sharp turn | Timing is spatial in prose: white space and sentence length pace the release | Double (`clm-tone-comedic-density-saturation`); Wodehouse chapter-end turns |

Craft notes for card §5: lexicon fields cluster around mock-formality
(elevated diction used for trivial matters), concrete domestic nouns, and
intensifier/slang contrast; syntax favours the periodic build ending in a short
punch clause; rhythm is long–long–short; psychic distance sits near the
detached/observational end while the narrator stays unpanicked.

## E. Cross-cultural survey

**India — hasya and the Vidushaka.** The Natyashastra treats the comic (hasya)
as one of the primary rasas, arising from determinants such as unseemly dress or
awkwardness, with laughter (hasa) as its stable state, and it grades laughter
into types (Natyashastra, shared `src-natyashastra-ghosh-1951`, ch. 6;
`clm-tone-comedic-hasya-rasa`). The same tradition institutionalizes the comic
in the Vidushaka, the clown/jester of classical Sanskrit drama, whose
incongruities (a brahmin friend who is a bumbling glutton) provide comic relief
and commentary. This is the strongest structural precedent for comedy as an
engine rather than a decoration. Translation limit: technical Sanskrit terms and
the precise taxonomy of laughter are mediated by Ghosh's edition; the card should
not quote rhythm or wordplay from translated Sanskrit.

**India — modern Hindi and Bengali.** Parsai (Hindi) and Parashuram (Bengali)
show the comic essay/short story in a modern Indian register: mock-serious
argument, absurd literal-mindedness, and bureaucratic or domestic imagery
(`work-parsai-inspector-matadeen`; `work-parashuram-anandibai`). Translation
limit: both are inspected mainly through English collections; tone, idiom, and
wordplay claims must be scoped to what the translations show.

**Japan — rakugo.** Kamigata rakugo is a four-century solo comic-storytelling
form in which a seated performer voices all characters and builds humour through
pacing, character voice, and patterned repetition; Shores documents its satire
and social mobility themes (`src-comedic-shores-rakugo-2021`). This supports the
claim that comic timing and character-voice are cross-cultural craft levers,
not Anglophone inventions (`clm-tone-comedic-crosscultural-oral`). Limit: the
performance features (pause, vocal contrast) cannot be fully transferred to
prose modelling from a monograph.

**China — xiangsheng.** Xiangsheng ("crosstalk") is a traditional Chinese comic
double-act built on rapid exchanges; Lawson analyses its "hidden musicality,"
showing that speech rhythm and patterned sound carry part of the humour
(`src-comedic-lawson-xiangsheng-2020`). This reinforces that verbal comedy is
also sonic and sequential, and that studying it only as written text loses
information.

**Additional.** French comic dramaturgy (Molière's comedies of manners and
character) is a further well-documented tradition; it is noted here but not
load-bearing, and no separate source record is claimed for it.

No false universal: these traditions do not share one comic theory. What they
share at the craft level is staged incongruity plus controlled delivery time.

## F. Exemplar field

| work_id | work | creator | mechanism demonstrated | verification note |
|---|---|---|---|---|
| work-wodehouse-code-woosters | The Code of the Woosters (1938) | P. G. Wodehouse | Escalating farce (D2); mock-formal narration and mixed-register wordplay (D5, D6); unpanicked comic distance (D7) | Publication verified (7 Oct 1938, Herbert Jenkins); technique described from the novel's structure and the critical sources in §I; no text reproduced |
| work-pratchett-guards-guards | Guards! Guards! (1989) | Terry Pratchett | Comic repetition/running motif (D8); mock-heroic hyperbole (D5); wide-angle comic narrator with satirical overlap | Publication verified (1989, Discworld #8); scholars note structural comic repetition; satirical overlap recorded |
| work-parashuram-anandibai | Anandibai Ityadi Galpa (1957) | Rajshekhar Basu ("Parashuram") | Absurd literal-mindedness and mock-serious narration (D1, D4); domestic imagery (D9) | Existence and date verified (1957; Sahitya Akademi 1958); technique at collection level, translation limit noted; no text reproduced |
| work-parsai-inspector-matadeen | Inspector Matadeen on the Moon and Other Satires (1994, trans.) | Harishankar Parsai; trans. C. M. Naim | Bureaucratic/mundane imagery (D9); mock-formal escalation (D2); satirical overlap recorded | Translated collection verified (Manas 1994; Katha reprint 2003); translation limit noted; no text reproduced |

Mechanism confirmation method: the works' existence and basic structure were
verified through the sources and catalogues in §I; the comedy mechanisms were
identified from structural description and secondary criticism, not from
reproducing copyrighted passages.

## G. Failure and misuse research

**Punching down (documented harm).** Disparagement humour directed at
lower-power targets is not just a taste problem. Ford and Ferguson's prejudiced
norm theory shows that exposure to disparagement humour can increase tolerance
of discrimination for high-prejudice audiences by establishing a norm of
levity around the expression (`src-comedic-ford-ferguson-2004`). McTernan
analyses the ethics of "punching down" and the duties of comedians, arguing the
standard ethic needs refinement rather than abandonment
(`src-comedic-mcternan-punching-down-2024`). Craft consequence: if the target
is a group rather than a person-in-a-situation, and the framing gives no benign
route, the material has crossed from comedic into disparagement
(`clm-tone-comedic-disparagement-harm`).

**Joke inflation.** Stacking gags in place of substance produces the
"seductive-details" failure: attention-grabbing humorous detail is recalled
better than the main point and can depress overall comprehension
(`src-comedic-harp-mayer-1998`; `clm-tone-comedic-density-saturation`). This is
the evidence-based version of "humour cannibalizing substance."

**Bathos.** An unintended drop from the elevated to the trivial can sabotage a
serious passage; the same low-register move that is comic when intended becomes
bathos when it collides with stakes the text is trying to honour. The card
should pair bathos with shared `clm-melodrama-unearned-emotion` as the
mirror-image failure (unearned high emotion vs. unearned low turn).

**Boundary trap — comedic vs. satire.** Wodehouse and Pratchett both attract
satirical readings; Parsai and Parashuram are usually called satirists. A card
must not claim that their comedy is targetless. It should say: the comedic
tone is the voice texture; whether there is a target is a mode/genre question
(`satirical-literature`).

**Weak persuasion effect.** Humour's effect on persuasion is small and
condition-dependent (O'Quin & Aronoff; meta-analytic evidence cited in §I), so a
card must not promise that jokes make an argument convincing
(`clm-tone-comedic-superiority-limits` counterevidence).

## H. Dosage and saturation findings

Evidence on density comes mainly from practitioner craft sources and from the
seductive-details literature; there is no single peer-reviewed "optimal jokes
per page" figure, so the card should state a band, not a universal law.

- Practitioner comedy writing describes a broad rule of thumb of roughly three
  jokes per page, with modern screen comedy increasing density to nearly every
  line of dialogue (practitioner craft sources, §I). Treat as Tier 4.
- Seductive-details research shows that adding engaging but off-topic humorous
  material reduces retention and transfer of the main content, and can harm
  learning even when learners enjoy the material (`src-comedic-harp-mayer-1998`).
- Comic material requires room to land: stand-up practice treats the pause as
  load-bearing, so density that eliminates beats removes the release mechanism
  (`src-comedic-double-standup-2005`).

Saturation signals for the card: every sentence reaching for a laugh; jokes
displacing the reader's promised takeaway; the same comic rule reused until the
inversion is predictable; humour at a stakes-peak that the piece cannot then
re-earn. Where to yield: at the emotional peak, the thesis sentence, and the
call to action for blog/marketing; substitute a single restrained beat or let
the serious line stand.

## I. Source records

All sources, claims, and primary works referenced above are written as JSON
records in this silo. One shared source is cross-linked read-only rather than
duplicated: `references/evidence/sources/src-natyashastra-ghosh-1951.json`
(Tier 1 critical edition) supports `clm-tone-comedic-hasya-rasa`. Shared
registries are not edited here. Cross-linked shared claims (read-only):
`clm-rasa-emotional-aesthetic`, `clm-dhvani-suggestion-theory`,
`clm-point-of-view-psychic-distance`, `clm-suspense-vs-surprise`,
`clm-pacing-rhythm-syntax`, `clm-melodrama-unearned-emotion`.

Silo sources: `src-comedic-suls-1972`, `src-comedic-mcgraw-warren-2010`,
`src-comedic-morreall-sep-2012`, `src-comedic-lintott-superiority-2016`,
`src-comedic-ford-ferguson-2004`, `src-comedic-harp-mayer-1998`,
`src-comedic-martin-humor-styles-2003`, `src-comedic-bergson-laughter-1900`,
`src-comedic-shores-rakugo-2021`, `src-comedic-lawson-xiangsheng-2020`,
`src-comedic-double-standup-2005`, `src-comedic-halpern-truth-comedy-1994`,
`src-comedic-oquin-aronoff-1981`, `src-comedic-mcternan-punching-down-2024`.

Primary works: `work-wodehouse-code-woosters`, `work-pratchett-guards-guards`,
`work-parashuram-anandibai`, `work-parsai-inspector-matadeen`.

Evidence-incomplete items: (1) direct peer-reviewed evidence for a numeric joke-
density optimum was not found; density guidance is scoped as practitioner Tier 4
plus seductive-details Tier 2. (2) Original-language assessment of Parsai and
Parashuram wordplay was not possible; claims are scoped to English translations.
(3) Rakugo performance features (pause, vocal contrast) are documented
scholarly but not transferable to prose modelling beyond the general timing
principle.
