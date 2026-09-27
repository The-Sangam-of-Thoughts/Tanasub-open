# Primary Work Analysis — {{work_id}}

**Axis:** {{axis_id}}  
**Template status:** {{status}}  
**Analysis date:** {{date}}

Use this worksheet to prepare one JSON record governed by `schemas/v1/primary-work.schema.json`. The structured record is authoritative. Plot summary does not satisfy a mechanics field.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Work ID | `id` | yes | Stable lowercase `work-...` ID; corresponds to `{{work_id}}`. |
| Title | `title` | yes | Directly verify against the edition or version analysed. |
| Creators | `creators[]` | yes | At least one directly verified creator. |
| Work type | `work_type` | yes | Exact controlled value. |
| Published date | `published_date` | yes | Use supported precision: year, year-month, date, or null. |
| Languages | `languages[]` | yes | At least one BCP 47-style tag. |
| Regions | `regions[]` | yes | At least one region or cultural context. |
| Axis IDs | `axis_ids[]` | yes | One or more canonical IDs, including `{{axis_id}}` where applicable. |
| Period role | `period_role` | yes | `formative`, `recognized`, `contemporary`, or `other`. |
| Source ID | `source_id` | yes | Directly verified `src-...` record for the analysed work. |
| Access | `access.*` | yes | Edition/version, language used, translator, and controlled access condition. |
| Analysis status | `analysis_status` | yes | `not-started`, `in-progress`, `complete`, or `revision-required`. |
| Mechanics | `mechanics.*` | yes | All 19 named fields are required; every field must be non-empty when complete. |

## Identity, corpus role, and access

- Verified title and creators:
- Work type:
- Publication date and precision:
- Languages and regions:
- Axis IDs and classification evidence:
- Period role and rationale:
- Source ID:
- Edition or version analysed:
- Language used:
- Translator:
- Access condition:
- Direct-verification evidence path:
- Copyright boundary for notes and excerpts:

## Mechanics analysis

Complete every schema field. Before `analysis_status: complete`, use null in the JSON record only when allowed; explain non-applicability and analyse the functional equivalent here.

### Premise — `mechanics.premise`

- Craft mechanism, evidence location, scope, and exceptions:

### Reader promise — `mechanics.reader_promise`

- Expected experience, delivery pattern, evidence location, scope, and exceptions:

### Opening — `mechanics.opening`

- Initial situation, orientation, promise, evidence location, and effect:

### Point of view — `mechanics.point_of_view`

- Perspective, distance, tense, shifts, evidence location, and function:

### Character system — `mechanics.character_system`

- Roles, agency, relationships, arcs or functional equivalent, and evidence location:

### Conflict and stakes — `mechanics.conflict_and_stakes`

- Pressure system, stakes, escalation, alternatives, and evidence location:

### Structure — `mechanics.structure`

- Causality, sequence, turning points, frame, nonlinearity, or functional equivalent:

### Scene movement — `mechanics.scene_movement`

- Unit-to-unit change, rhythm, transitions, or medium-specific equivalent:

### Dialogue — `mechanics.dialogue`

- Speech, subtext, silence, voice differentiation, or functional equivalent:

### Setting — `mechanics.setting`

- Place, time, social world, atmosphere, research demands, and consistency:

### Style and devices — `mechanics.style_and_devices`

- Diction, syntax, imagery, rhetoric, culturally specific techniques, intended effects, and misuse risks:

### Emotional progression — `mechanics.emotional_progression`

- Emotional sequence, modulation, release, fatigue risk, and evidence location:

### Suspense or anticipation — `mechanics.suspense_or_anticipation`

- Withholding, expectation, revelation, surprise, or functional equivalent:

### Climax — `mechanics.climax`

- Culmination, decisive change, anti-climax, or functional equivalent:

### Ending — `mechanics.ending`

- Resolution, closure, ambiguity, aftermath, hook, or functional equivalent:

### Conventions — `mechanics.conventions`

- Fulfilled, varied, resisted, or culturally specific conventions with evidence:

### Innovation or subversion — `mechanics.innovation_or_subversion`

- Innovation mechanism, reader-contract effect, limits, and evidence:

### Critical reception — `mechanics.critical_reception`

- Separately attributed professional criticism; agreement, disagreement, and writing-level relevance:

### Audience reception — `mechanics.audience_reception`

- Separately attributed reader or audience response; sampling limits and writing-level relevance:

## Evidence-expression discipline

For every consequential observation, identify its source/work location and label it as quotation, paraphrase, synthesis, or researcher inference in the linked claim record. Record counterevidence, cultural and historical scope, exceptions, confidence, and downstream report locations there.

## Indian, regional, and translation analysis

- Indian or regional tradition and terminology:
- Original-language evidence available:
- Translation and translator used:
- Conclusions dependent on translation:
- Regional-cinema or adaptation relevance:
- Risk of false equivalence or overgeneralisation:

## Remediation and review handoff

- Unverified dates, identities, quotations, translations, classifications, or numerical assertions:
- Evidence limitations and access barriers:
- Open copyright questions:
- Required remediation and owner:
- Independent reviewer:
- Evidence paths for review:

The author may self-check completeness but may not approve this analysis.

## Category and passage-verification checks

Before marking this analysis complete, record: (1) the source record and locator that supports this work's relationship to `{{axis_id}}`; (2) the exact edition/version, consulted language, translator, and access condition; (3) one passage or unit-verification event for each consequential mechanics observation; and (4) any counterreading or classification dispute. An unavailable passage, mismatched edition, or unsupported work/axis assignment leaves the relevant mechanic and every dependent claim incomplete.
