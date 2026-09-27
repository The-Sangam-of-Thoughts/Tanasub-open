# Research Methodology

**Version:** 1.0.0  
**Scope:** research infrastructure and all later creative-writing axes  
**Authority:** master plan, sprint plan, sprint governance, and [Version 1 data contracts](../schemas/v1/README.md)  
**Approval state:** prepared for independent review and G1 human decision; this file is not an approval record

## 1. Purpose and governing principles

This methodology produces a versioned, practitioner-facing creative-writing library in which every recognised genre and subgenre receives the same research obligations, document contract, and quality gates. Equal importance means equal method, not equal word count and never quota padding.

The method is:

- evidence-led: consequential recommendations are traceable to directly verified sources or primary works;
- axis-specific: evidence is not transferred between axes unless the claim record explicitly supports every destination axis;
- breadth-first: the project completes the same research class across all frozen axes before advancing to the next class;
- culturally plural: Indian, regional, oral, multilingual, and translated traditions are searched deliberately rather than treated as optional additions;
- disagreement-preserving: counterevidence, exceptions, confidence, and contested classifications remain visible;
- fail-closed: incomplete evidence, invalid records, unresolved blocking findings, or a missing independent decision prevents the affected lifecycle advance and publication.

## 2. Unit of research

The unit is a canonical axis record with a stable `axis-*` identifier and one `axis_type`: `form`, `genre`, `subgenre`, `mode`, `structure`, `audience`, `medium`, `tradition`, or `hybrid`. A qualifying genre or subgenre receives one canonical package. A hybrid may have multiple parents, but its research files exist only once.

All structured records use the exact field names and controlled values in `schemas/v1/`. Markdown is the canonical publication format; JSON is the deterministic interchange and validation format.

## 3. Research stages and exit evidence

### Stage 1 — Taxonomy census

Harvest candidate labels through the `taxonomy-authoritative` and `taxonomy-cultural-industry` search streams. Include library and archival vocabularies, scholarship, publishers and booksellers, historical and regional taxonomies, Indian literary institutions and language traditions, and documented communities.

For each candidate:

1. Preserve the source wording, locator, access date, language, region, and provisional axis type.
2. Normalise spelling without discarding historical, regional, marketing, or contested names.
3. Test the label against the recognition and distinctiveness rules in [taxonomy-rules.md](taxonomy-rules.md).
4. Record a pass, rejection, alias decision, or disputed state with its evidence and rationale.
5. Build reciprocal parent, child, related, and hybrid relationships without duplicating canonical identity.

**Exit evidence:** reproducible search logs, source records, corpus-warrant records, recognition calculation, distinctiveness assessment, relationship proposal, and adjudication record. Taxonomy drafting cannot begin until the census evidence is independently reviewable.

### Stage 2 — Research-question mapping

Create an axis-specific question map covering definition and history; reader expectations and emotional effect; titles and openings; structure and progression; character and dialogue; setting and worldbuilding; voice, style, and devices; suspense and pacing; climax and resolution; conventions and innovation; failure patterns; cultural variation; Indian examples; exercises; and revision.

Questions must expose genuine uncertainties, boundary disputes, media differences, contrary views, and culturally specific practices. Reusing a generic question unchanged is acceptable only when it remains materially applicable; otherwise rewrite it for the axis.

**Exit evidence:** a complete question map linked to the axis ID and reviewed for the same topical depth required of every other axis.

### Stage 3 — Source discovery

Run and retain separate searches for every applicable controlled `search_stream`:

- `primary-works`, `historical-criticism`, `contemporary-scholarship`, and `craft-practitioner`;
- `interviews`, `professional-reviews`, and `audience-reception`;
- `indian-regional`, `translation-studies`, and `screen-adaptation`;
- `contrary-revisionist`;
- taxonomy streams when recognition or boundaries remain in scope.

Each search record must state the database or site, exact query, execution time, operator, languages, regions, inclusion and exclusion criteria, result count, included source IDs, excluded results with reasons, dead ends, and access constraints. An unsuccessful search is evidence only when the search is reproducible and its limitations are explicit.

**Exit evidence:** schema-valid search logs whose included source IDs resolve and whose omissions can be audited.

### Stage 4 — Source evaluation and extraction

Create one source record per selected source. Record bibliographic identity, `source_type`, `source_roles`, reliability tier, publication detail, languages, regions, access conditions, direct-verification evidence, linked axes and claims, translation state, and copyright decision.

Every extracted item is labelled as `quotation`, `paraphrase`, `synthesis`, or `researcher-inference`. Quotations retain an exact locator. Paraphrases remain faithful to the source scope. Syntheses identify all supporting records. Researcher inferences are never phrased as source statements. Contradictory material is recorded rather than silently discarded.

**Exit evidence:** schema-valid source records and extraction records sufficient for another reviewer to repeat each verification.

### Stage 5 — Primary-work analysis

Select works for corpus breadth and craft relevance, not prestige alone. The complete mechanics analysis covers premise, reader promise, opening, point of view, character system, conflict and stakes, structure, scene movement, dialogue, setting, style and devices, emotional progression, suspense or anticipation, climax, ending, conventions, innovation or subversion, critical reception, and audience reception.

Critical and audience reception remain distinct fields. A work with `analysis_status: complete` must have substantive text in every mechanics field; a non-applicable conventional topic requires a reasoned functional equivalent, not an empty value.

**Exit evidence:** schema-valid primary-work records with resolved source and axis IDs and directly verified edition, language, translator, and access information.

### Stage 6 — Claim formation and comparative synthesis

Enter every consequential craft recommendation as a `clm-*` record. State the exact claim, supported axes, supporting evidence, counterevidence, scope, exceptions, confidence, report locations, inference label, and verification date.

Compare evidence within an axis; across sibling and parent relationships; across periods, cultures, and languages; between Indian and international traditions; between prose and writing-level screen adaptation; between praised and criticised works; and between conventional execution and deliberate subversion. Similarity does not erase category boundaries, and contrast does not imply hierarchy.

**Exit evidence:** claim records whose evidence IDs and report locations resolve, plus comparison notes that preserve disagreement and limitations.

### Stage 7 — Drafting and editorial synthesis

Draft only after the relevant evidence stage passes, in this order:

1. evidence dossier and claim matrix;
2. required analyses;
3. close readings;
4. comparison, failure, and reception analyses;
5. main practitioner guide;
6. exercises and revision tools;
7. annotated sources;
8. cross-links and indexes.

The main guide must synthesise completed support and cannot introduce a new consequential claim. Each exercise must trace to an analysis finding or failure mode. Each file must be usable independently and connected to the canonical package.

**Exit evidence:** complete template-derived artifacts, resolved references, QA results, manual sample, independent editorial decision, and lifecycle evidence.

## 4. Evidence floor and sufficiency

Before an axis can become `evidence-complete`, its dossier must contain at least:

- 20 credible secondary sources;
- 12 primary creative works by at least eight creators;
- three historical stages where the category is old enough;
- two cultural or linguistic traditions where evidence exists;
- one formative, three recognised, and three contemporary examples;
- contrasting critical or practitioner positions;
- Indian examples or a documented, independently reviewable search explaining their absence;
- screenplay, adaptation, or film-reception evidence where relevant to writing.

Counts are necessary but not sufficient. Duplicate editions, dependent publications, or recycled assertions do not manufacture independence. If credible evidence is inadequate, set the affected state to `evidence-incomplete`, record the gap and search history, and block dependent analysis and drafting. Never add a weak source merely to reach a number.

## 5. Indian, regional, oral, and translation coverage

Operational applicability is defined strictly: every qualifying genre and subgenre axis without exception must execute and retain a dedicated `indian-regional` search before any finding, absence, or scope conclusion is reached. An axis cannot be exempted from this requirement by assertion. For non-genre axes (such as forms, modes, traditions, structures, or audiences), the dedicated search is mandatory unless an evidence-backed rationale demonstrates that the axis represents a culturally or geographically localized non-Indian tradition, in which case the search must examine comparative reception, transmission, translation, and parallel or antecedent traditions before any absence or scope boundary is concluded.

Every applicable axis records:

- documented Indian examples and their source IDs;
- relevant Indian-language terminology and regional or oral traditions;
- ways those traditions complicate imported or Western classifications;
- translation dependence and limitations;
- the eventual cross-link to the Indian literature atlas.

Regional cinema research must not default to Hindi cinema. Film evidence is restricted to story conception, screenplay structure, character construction, dialogue and subtext, adaptation, genre development, cultural specificity, emotional design, suspense and revelation, endings, and writing-level reception.

If no direct Indian equivalent is found, audit all searches, state their language and access limits, and discuss the closest relevant traditions without asserting equivalence. Every such absence claim receives 100% audit review.

Conclusions drawn through translation must name the edition, language used, and translator. They must state what cannot be verified in the original language and must not claim unverified sound, rhythm, diction, wordplay, prosody, or culturally embedded meaning.

## 6. Reception method

A reception study uses at least three independent professional reviews and, where available, contrasting positive and negative assessments. Code only writing-relevant observations such as originality, narrative coherence, motivation, dialogue, pacing, emotion, suspense, theme, cultural specificity, genre satisfaction, climax, ending, predictability, exposition, cliché, and adaptation quality.

Professional criticism is evidence for critical reception. Reader or audience response is evidence only for a separately labelled audience-reception layer. Popularity, awards, ratings, or sales are not proof of craft quality. Acting, direction, editing, visuals, and music are excluded unless the analysis explicitly demonstrates how they alter perception of screenplay-level writing.

## 7. Verification and audit sampling

Direct verification is mandatory for 100% of quotations, translations, dates, titles, creator identities, recognition decisions, numerical assertions, limited-confidence claims, disputed claims, insufficient-evidence records, and assertions that no Indian equivalent exists.

For all other consequential claims, inspect 10% of each batch, with a minimum of five and maximum of twenty; inspect all when the batch contains fewer than five. Each applicable batch includes at least one Indian or regional record. Sampling records name the population, selection method, sampled IDs, verifier, evidence consulted, result, and findings.

An author may self-check but cannot supply final independent verification. Any critical, high, or evidence-affecting medium finding blocks progression until remediation is recorded and independently retested. Original failures remain immutable; successful retests are stored separately.

## 8. Publication boundary

Schema validity alone does not establish evidence completeness, editorial acceptance, gate approval, or publishability. Two distinct publication boundaries are governed:

1. **Research-infrastructure preview releases:** Releases such as the S00–S03 preview governed by `Plan/accelerated-release-plan-2026-09-11.md` are bounded strictly to governance, data contracts, QA harness, methodology, policies, quality rubric, research and editorial templates, and test/audit evidence. They do not contain production genre packages, do not assert family completeness, and do not require G6 approval. Their release requires all sprint obligations through S03 passed, passing deterministic QA harness validation, independent review acceptance without open critical, high, or evidence-affecting medium findings, a completed manual usability trial, and signed human gate G1 approval (or an explicitly designated `v0.1.0-rc1` pre-release when G1 is pending).
2. **Canonical axis, package, and genre-family publication:** Full publication of creative-writing encyclopedia content requires allowed lifecycle transitions (`publishable` status), complete package and evidence contracts (meeting all Section 4 evidence floors), passing deterministic validation, manual sampling, independent acceptance, complete family coverage, G6 human approval for each family, and a final release-audit pass.

Under either boundary, any validation finding sets publication permission to false. Missing evidence, missing reviewer, pending applicable human gate, unresolved blocking finding, accidental unfinished marker, unknown template token, secret, credential, invented quotation, unverified claim, or copyright breach is a stop condition. Automated success never substitutes for G1 or any later human gate.

## 9. Axis-transfer test and author handoff

Advice developed for one axis may be reused in another only when its claim record names the destination axis and records: (a) a relevance rationale based on the destination's form, medium, tradition, language, and reader contract; (b) direct supporting evidence or a clearly labelled bounded inference for that destination; (c) a documented counter-search; and (d) a limitation or exception. A general craft source can supply a hypothesis, but cannot by itself verify a category-specific convention.

Before a production series, walk the template through one parent genre, one established subgenre, and one regional or form axis. The analyses must use the same required functions while demonstrating different, evidence-supported implementations. Record input dossiers, output paths, open gaps, and reviewer observations. Calibration establishes template fitness; it does not confer a release decision or preferential treatment.

Each author handoff must name the assigned artifact class and paths, approved template revision, axis dossier revision, source/work records, claim-matrix revision, and finding IDs in scope. The author returns changed paths; claim and finding mapping; unresolved access, evidence, or copyright limits; and author-check results. Missing inputs stop dependent drafting and are recorded as gaps. A reviewer receives sealed input and output hashes plus the same evidence packet; a reviewer label alone does not establish independence.

