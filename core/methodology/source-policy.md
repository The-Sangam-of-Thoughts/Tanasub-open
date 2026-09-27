# Source Policy

**Version:** 1.0.0  
**Scope:** discovery, selection, verification, extraction, reuse, translation, reception, access, and copyright  
**Authority:** master plan, [source schema](../schemas/v1/source.schema.json), and [claim schema](../schemas/v1/claim.schema.json)  
**Approval state:** prepared for independent review and G1 human decision; this file is not an approval record

## 1. Selection principle

Select sources for authority, direct relevance, independence, verifiability, cultural and historical coverage, and fitness for the claim being made. Counts are evidence floors, not collection targets. A weak, derivative, inaccessible, or irrelevant source is not admitted merely to increase a count.

Each selected item receives one schema-valid `src-*` record. A source record identifies its roles; it does not make the source equally strong for every role.

## 2. Evidence hierarchy and reliability tiers

The project applies this evidence hierarchy:

1. primary works, manuscripts, authorised scripts, author essays, lectures, diaries, and interviews;
2. peer-reviewed research, scholarly books, critical editions, and literary histories;
3. professional criticism and long-form literary or film reviews;
4. established craft books and work by editors, teachers, and practitioners;
5. reader and audience responses, used only for reception.

The numeric `reliability_tier` records the following operational judgment, with 1 strongest and 5 most limited:

| Tier | Typical use and requirement |
|---:|---|
| 1 | Direct primary evidence or an authoritative scholarly/library record verified in the relevant edition or record. Strong for what the item directly establishes, not automatically for general craft causation. |
| 2 | Peer-reviewed scholarship, scholarly books, critical editions, and literary histories with clear methods and traceable citations. |
| 3 | Independent professional criticism, long-form reviews, and well-documented institutional or industry sources. |
| 4 | Established practitioner, editor, teacher, or craft sources whose experience is relevant but whose claims require scope and triangulation. |
| 5 | Reader/audience response, community documentation, limited previews, or other constrained evidence. Use only for the role it can support and never as sole support for a consequential factual or universal craft claim. |

Tier is assigned after reviewing authorship, editorial control, method, citations, proximity to the subject, independence, currency where relevant, conflicts of interest, and access completeness. Prestige does not override an item's actual fitness for a claim.

### Controlled secondary-source classification

To satisfy the methodology evidence floor of at least 20 credible secondary sources before an axis reaches `evidence-complete`, each counted source must have `reliability_tier` 1, 2, 3, or 4 and its controlled `source_type` must belong to this closed sixteen-type set:

- `peer-reviewed-article`
- `scholarly-book`
- `critical-edition`
- `literary-history`
- `professional-criticism`
- `long-form-review`
- `craft-book`
- `editor-essay`
- `teacher-resource`
- `practitioner-essay`
- `library-vocabulary`
- `archival-record`
- `publisher-classification`
- `bookseller-classification`
- `industry-classification`
- `community-documentation`

Role, credibility, and counting limits:
- Primary creative works and creator-reflection types (`primary-work`, `manuscript`, `interview`, `author-essay`) count toward primary-work or craft evidence floors, not toward the 20 secondary-source floor.
- Reader and audience sources (`reader-response`, `audience-review`) are restricted to Tier 5 and may support only the reception layer; they do not count toward the secondary-source floor.
- Sources classified as `other` do not count toward the secondary-source floor unless formally reclassified under an approved controlled type through an audit-documented exception.
- Sources with `verification.verified_directly: false` or unverified access do not count toward the secondary-source floor.

## 3. Permitted roles and role limits

Use the controlled `source_roles`: `recognition`, `definition`, `history`, `craft-support`, `counterevidence`, `reception`, `translation`, `indian-context`, `screen-adaptation`, and `corpus-warrant`.

- Recognition requires explicit category recognition; topical mention is insufficient.
- Corpus warrant requires evidence that the cited work belongs to the candidate category, with disputes preserved.
- Craft support must bear on the exact recommendation and axis scope.
- Counterevidence records disagreement, counterexamples, and boundary conditions with the same care as support.
- Reception evidence establishes reported reception, not objective craft quality.
- Translation sources establish translation history, choices, or limits; an English rendering does not prove original-language mechanics.
- Screen-adaptation evidence is limited to writing, adaptation, storytelling, and writing-level reception.

One source may hold multiple roles only when each role is directly supported and recorded.

## 4. Direct verification

Before selection, inspect the source itself in the edition, version, page, timestamp, archival record, or stable database entry used. Aggregator snippets, generated summaries, citation-only references, and uninspected secondary quotations do not satisfy `verification.verified_directly: true`.

The source record must contain:

- complete title and creators;
- controlled source type and roles;
- publisher or container and the most precise defensible publication date;
- edition, DOI, or ISBN when applicable and available;
- language and region metadata;
- a durable locator, access date, and access conditions;
- verification time, verifier, and notes describing what was inspected;
- resolved axis and claim IDs;
- translation and copyright decisions.

Reverify when the locator changes, an online source is materially revised, a quotation or date is disputed, a different edition is used, or remediation reopens the claim.

## 5. Extraction and provenance

Every evidence link states its `evidence_expression`:

- `quotation`: exact words, reproduced sparingly, with an exact locator and edition;
- `paraphrase`: a faithful restatement that preserves qualification and scope;
- `synthesis`: a conclusion supported by multiple named evidence records;
- `researcher-inference`: an explicitly labelled inference not stated by the source.

Do not convert an inference into a paraphrase, remove a source's caveat, combine incompatible populations, or imply causal advice from reception correlation. Notes must make the connection between evidence and claim auditable.

Every consequential claim record includes supporting evidence, a deliberate counterevidence search, scope, exceptions, confidence, report locations, an inference label, and `last_verified`. An empty counterevidence array means no qualifying contrary evidence was found after a logged search; it does not mean none exists.

Confidence is assigned as follows:

- `strong`: convergent, directly verified evidence with no unresolved material counterevidence in the stated scope;
- `moderate`: credible support with meaningful limits or some disagreement that does not overturn the scoped claim;
- `limited`: sparse, indirect, translation-constrained, access-constrained, or narrowly applicable evidence;
- `disputed`: credible sources materially conflict or the boundary remains contested.

Confidence cannot exceed what the weakest necessary inference or access limitation permits.

## 6. Independence, duplication, and reuse

Multiple editions, translations, database copies, syndications, or summaries of the same originating work count once toward source independence. Record the edition actually verified and link related records when separate versions matter analytically.

A source may support more than one axis, but each use must be recorded through `axis_ids`, `claim_ids`, and the claim's scoped evidence link. Advice cannot be copied across axes merely because both cite the same general craft source.

Where a source conflicts with itself across editions or dates, preserve both versions, identify the change, and use the applicable version explicitly.

## 7. Translation and multilingual evidence

For translated material, record `translation.is_translation`, original-language code, translator, edition or version, and every known limitation. Name whether the researcher inspected the original, a translation, or both.

Claims about plot, structure, or reception may be defensible through a reliable translation if the limitation is stated. Claims about sound, rhythm, rhyme, diction, syntax, wordplay, prosody, register, or culturally embedded terminology require original-language competence or directly verified specialist evidence. Otherwise classify them as limited or omit them.

Do not invent translations, silently modernise wording, combine different translations into a quotation, or back-translate. When translations diverge materially, record the disagreement and its consequence for the claim.

Language access gaps must be visible in search logs and `evidence_limitations`. Lack of English-language results is not evidence that a tradition or equivalent does not exist.

## 8. Indian and regional coverage

Operational applicability is defined strictly: every qualifying genre and subgenre axis without exception must execute and retain a dedicated `indian-regional` search (and, when needed, `translation-studies` search) across relevant languages, regions, institutions, histories, oral/performance traditions, and regional cinemas before any finding, absence, or scope conclusion is reached. An axis cannot be exempted from this requirement by assertion. For non-genre axes (forms, modes, traditions, structures, audiences), the dedicated search is mandatory unless an evidence-backed rationale demonstrates that the axis represents a culturally or geographically localized non-Indian tradition, in which case the search must examine comparative reception, transmission, translation, and parallel or antecedent traditions before any absence or scope boundary is concluded. The corpus may not default to English-language Indian writing or Hindi cinema.

Indian examples require resolved work and source records, not name-only mentions. Indian aesthetic concepts such as rasa, dhvani, vakrokti, and aucitya must be explained through suitable primary or scholarly sources and not flattened into approximate Western labels.

If no direct equivalent is found, retain the search queries, resources, languages, access barriers, excluded results, and closest non-equivalent traditions. State the conclusion as limited by that search and send it for 100% audit review.

## 9. Reception evidence

A reception analysis uses at least three independent professional reviews. Seek positive and negative assessments where available. Code professional criticism separately from reader or audience response, and identify when a source mixes the two.

Reader and audience sources can support only the separately labelled reception layer. Ratings, sales, awards, popularity, and comment volume do not establish writing quality. Film analysis excludes direction, acting, editing, cinematography, and music unless the source and analysis show a material effect on perception of screenplay-level writing.

## 10. Copyright and repository-copy boundary

Do not store copyrighted books, screenplays, paywalled articles, unauthorised scans, substantial excerpts, or other full texts in the repository. Store bibliographic metadata, lawful locators, verification notes, and concise evidence excerpts only when necessary for criticism, scholarship, or verification and permitted by applicable rights and project policy.

For each source, set `copyright.status`, `repository_copy_allowed`, and explanatory notes. `repository_copy_allowed: true` requires a documented public-domain, licensed, permission-based, or otherwise approved basis. Unknown status defaults to no repository copy.

Quotations must be no longer than needed, directly verified, correctly attributed, and located. Prefer paraphrase where exact language is not analytically necessary. Never evade access controls, redistribute purchased or library-only material, or treat availability on the internet as permission.

Records may retain restricted-access metadata and analysis, but not the restricted source itself. A suspected infringement is critical: stop affected publication, quarantine the copied material without destroying audit evidence, record the finding, assess downstream claims, remediate, and obtain independent retest.

## 11. Sufficiency, exceptions, and blocking

The evidence floor and diversity requirements in [methodology.md](methodology.md) apply before `evidence-complete`. If sources are unavailable, unreliable, non-independent, translation-constrained, or copyright-constrained, record the exact limitation. Do not substitute weak material or conceal the gap.

Fabricated evidence, invented quotation or translation, copyright breach, unresolved identity/date/classification error, or failed publication control is release-blocking. A pending source check leaves the claim and dependent artifact incomplete. Automated schema success cannot turn an unverified source into acceptable evidence.

## 12. Verification-event contract

Record distinct events for discovery, metadata verification, text access, passage verification, and reception sampling. Each event identifies its record ID, purpose, exact source or work edition/version, language and translator where applicable, locator checked, access condition, date/time, operator, method, result, and retained evidence path. `located` or `metadata-confirmed` never means `passage-verified`; `passage-verified` never authenticates a different edition or translation.

A quotation, translation-dependent observation, mechanics assertion, date, identity, classification, or numerical assertion is eligible for use only after the event that checks that exact assertion and locator. For professional reception, also record publication, reviewer, review date, relationship or independence group, position, and whether the observation concerns writing rather than production. Missing event fields leave the assertion unverified and block every dependent claim.

Source ledgers must retain unsuccessful searches, including query, corpus or repository, language, date, result count or access barrier, and decision. An absence conclusion must point to those events and state the searched scope; no result is never proof of absence.
