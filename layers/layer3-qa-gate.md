# Layer 3 — Final QA Gate

Run this gate after drafting, storytelling enhancement, and humanization. Choose the academic or blog gate. Record each result and an evidence pointer such as a heading, sentence, citation, or measured value. Averages never cancel a blocking failure.

## Academic gate

Score every dimension: **3** ready; **2** present but needs improvement; **1** unsafe or materially incomplete; **0** absent or contradicted.

| Dimension | Blocking? | A score of 3 requires |
|---|---:|---|
| Teachability | Yes | Mechanism, example, effect, diagnosis, and revision action are usable. |
| Evidence fidelity | Yes | Consequential claims resolve to suitable evidence; inference and limits are explicit. |
| Disagreement and scope | Yes | Exceptions, counterevidence, applicability, and contested positions are honest. |
| Cultural and historical scope | Yes | Relevant traditions and periods appear without one norm becoming universal. |
| Indian and regional responsibility | When applicable | Specific language, region, oral tradition, or a documented evidence gap replaces tokenism. |
| Translation integrity | When applicable | Consulted language, edition, translator, and interpretive limits are named. |
| Primary-work mechanics | For work analysis | Analysis explains how textual or writing choices function; plot summary is insufficient. |
| Reception separation | When used | Professional criticism and audience response remain separately sourced. |
| Tone (when requested) | When requested | The named tone is sustained or deliberately modulated, its restraint rules are respected, and the tone does not override the genre engine; genre-engine conflicts follow `tones/_combination-rules.md`. |
| Originality and convention | No | Convention, cliché, innovation, and deliberate subversion are distinguished. |
| Diagnostics and revision | No | Observable failure signals lead to bounded repairs. |
| Exercise alignment | No | Each exercise practises a named mechanism with success criteria. |
| Accessibility | No | Plain language, logical headings, descriptive links, and non-visual meaning work. |
| Cross-links and identity | Yes | IDs, citations, paths, relationships, and related files resolve. |
| Copyright and privacy | Yes | Use is defensible; no excessive quotation, secret, or unsafe personal data appears. |
| Completion honesty | Yes | Status matches evidence; gaps and pending review remain visible. |

**Anti-padding check:** reject repeated definitions, stock paragraphs, label-swapped advice, generic encouragement, and length added without a new supported condition, example, effect, exception, diagnosis, or action.

**Academic pass:** every applicable blocking dimension scores 3; every other dimension scores at least 2; no unresolved Critical, High, or evidence-affecting Medium finding remains. Inspect every quotation, translation, date, identity, number, disputed or limited-confidence claim, and absence claim.

**Tone (when requested) is conditional-blocking.** It applies only when a tone was explicitly requested for the piece. A tone-less task records it as `not applicable` with a one-line reason and is neither blocked nor penalized by it; a requested tone that fails blocks until sustained, deliberately modulated, or corrected.

## Blog, social, and marketing gate

Mark each item **pass**, **revise**, or **not applicable**, with evidence.

| Check | Pass condition |
|---|---|
| Brief and platform fit | Reader, promise, action, register, format, and verified hard limits align. |
| Hook effectiveness | The first three sentences use a named Layer 1 hook and deliver on it without deception. |
| Structure and scan | Three to five purposeful units; headings, paragraphs, and bullets support both scanning and full reading. |
| Rhythm variation | Sentence lengths visibly vary; measure standard deviation when tooling exists and inspect the result in context. |
| Voice naturalness | The Coffee Shop Test sounds appropriate for the named reader and register. |
| Tone fidelity | When a tone was requested, the named tone is sustained or deliberately modulated, its restraint rules were respected, and genre-engine conflicts follow `tones/_combination-rules.md`. `Not applicable` requires a one-line reason when no tone was requested. |
| Headline | The 4-U review records useful, urgent, unique, and ultra-specific; weak dimensions are revised or justified. |
| Practical value | The piece provides a concrete takeaway, decision, or next action. |
| Claim integrity | Material facts and quotations are verified; examples, opinion, sponsorship, and limitations are labelled. |
| Cultural and audience fit | Language and assumptions fit the actual audience without stereotypes or false universals. |
| Humanization | The Layer 2 word-, sentence-, paragraph-, and document-level reflection is recorded. |
| Accessibility | Links, headings, meaning, and calls to action are understandable without visual styling alone. |
| Completion honesty | No placeholder, unsupported result, invented testimonial, fake urgency, or false readiness claim remains. |

**Blog pass:** every applicable item passes. `Not applicable` requires a one-line reason. Claim integrity, accessibility, and completion honesty are always blocking. Any legal, health, safety, financial, privacy, copyright, or reputational claim that lacks suitable verification also blocks.

**Tone fidelity is conditional-blocking.** It blocks only when a tone was requested and the named tone is not sustained or deliberately modulated, its restraint rules are disrespected, or a genre-engine conflict ignores `tones/_combination-rules.md`. With no tone requested it is `not applicable` and does not block or inflate the gate.

## Failure routing

Do not patch only the scorecard. Return the work to the phase that introduced the defect:

| Failure | Return to |
|---|---|
| Audience, purpose, structure, evidence, scope, accessibility, or platform fit | **Phase 1 — Draft:** revise with the selected Layer 0 and genre instruction. |
| Hook, tension, story shape, rhythm, headline, or engagement | **Phase 2 — Enhance:** revise with Layer 1. |
| Register, cadence, generic phrasing, symmetry, hedging, or impersonal voice | **Phase 3 — Humanize:** rerun Layer 2 reflection, then revise. |
| Tone choice, engagement, or a requested tone that fails to serve the brief | **Phase 2 — Enhance:** revise with Layer 1 and the requested tone; resolve genre-engine conflicts through `tones/_combination-rules.md`. |
| Tone drift, tonal whiplash, or tone/register mismatch | **Phase 3 — Humanize:** rerun Layer 2 reflection and the tone's restraint rules, then revise. |
| Broken link, formatting error, unresolved marker, or inconsistent status introduced during review | **Phase 4 — QA:** correct it and rerun the entire applicable gate. |

Tone routing rows apply only when a tone was requested; tone-less work has no tone failure to route and returns to its normal phase. After any revision, rerun all later phases and the full gate. Preserve the failed result separately from the retest.

## Decision record

Record mode, artifact/version, reviewer, date, check or dimension, result, evidence pointer, finding ID, required revision, and retest result. An author's check may produce `ready-for-review`; it cannot create independent acceptance or human approval. Automated success is evidence only. Never invent a reviewer, sign-off, gate decision, or publication status.
