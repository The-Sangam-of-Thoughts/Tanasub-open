# Taxonomy Rules

**Version:** 1.0.0  
**Scope:** candidate discovery, recognition, classification, relationships, freeze, and change control  
**Authority:** master plan, [axis schema](../schemas/v1/axis.schema.json), and [controlled vocabularies](../schemas/v1/controlled-vocabularies.json)  
**Approval state:** prepared for independent review and G1 human decision; this file is not an approval record

## 1. Canonical axis types

Assign exactly one controlled `axis_type` to each canonical axis:

| Type | Operational meaning |
|---|---|
| `form` | The broad compositional form, such as novel, poem, play, or screenplay. |
| `genre` | A recognised category organised by a characteristic cluster of reader promise, emotional engine, conventions, history, and corpus. |
| `subgenre` | A recognised, distinct category nested under or strongly derived from one or more genres. |
| `mode` | A manner or tonal orientation, such as satire, tragedy, suspense, or absurdism. |
| `structure` | A recurring architecture, such as a frame narrative or locked-room design. |
| `audience` | A readership or developmental market category. |
| `medium` | The delivery or performance medium. |
| `tradition` | A historically or culturally grounded practice or lineage. |
| `hybrid` | A recognised category whose identity depends on a substantive combination of multiple parents. |

Marketing labels are evidence to evaluate, not an additional axis type. Modes, structures, audiences, media, and traditions may receive craft guides but must not be relabelled as genres for convenience.

## 2. Candidate record and independence

Every proposed label begins as a candidate with:

- original wording and exact source locator;
- provisional preferred label, aliases, language, region, and axis type;
- linked `src-*` recognition and corpus-warrant records;
- the source's `independent_group`;
- candidate parent, child, related, and hybrid relationships;
- recognition-path counts and a distinctiveness worksheet;
- decision status and reason.

Sources are independent only when their recognition judgments are not controlled by, copied from, or substantially derived from the same originating publication, organisation, catalogue, dataset, or editorial group. Multiple pages, editions, translations, imprints, mirrors, or summaries of one underlying authority count as one independent group. A source may be credible without being independent for threshold counting.

## 3. Recognition threshold

A label qualifies as an independent genre or subgenre only when it passes one complete recognition path and the distinctiveness test.

### Path A — independent-source recognition

- at least three credible recognition sources from three independent groups explicitly identify the label as a distinct category; and
- a recognisable corpus contains at least eight works by at least four creators.

### Path B — authoritative recognition

- at least one authoritative scholarly or library source explicitly recognises the category;
- a recognisable corpus contains at least five works by at least three creators; and
- evidence demonstrates a distinct writing practice.

The reviewer recalculates counts from resolved records. A title, creator, or source cannot be counted twice because it has multiple editions, identifiers, formats, or citations. A work included only as a disputed example must be labelled and cannot silently satisfy the corpus floor.

Commercial popularity, a retailer shelf, a single practitioner coinage, community enthusiasm, awards, sales, or search-result volume cannot alone establish recognition. Community and industry evidence can contribute when its provenance, durability, corpus warrant, and independence are documented.

## 4. Distinctiveness test

The candidate must differ materially from its nearest non-equivalent neighbours in at least two of these dimensions:

1. reader promise;
2. emotional engine;
3. plot or structural logic;
4. character functions;
5. setting or world assumptions;
6. voice and stylistic conventions;
7. conflict and stakes;
8. ending or resolution conventions;
9. historical or cultural tradition.

For every claimed difference, record the neighbour, dimension, evidence IDs, observed practice, counterexample or overlap, and conclusion. Two labels for the same practice do not pass merely because their descriptions use different words. A difference in market packaging alone does not satisfy the test unless evidence shows a distinct writing practice in a qualifying dimension.

Decision rule:

- recognition path passed and at least two evidence-backed dimensions passed: create a canonical axis;
- recognition passed but fewer than two dimensions passed: resolve as an alias or broader/narrower term, as the evidence warrants;
- distinctiveness passed but recognition evidence or corpus floor failed: retain as a disputed or rejected candidate for the current version;
- evidence is contradictory or borderline: retain the dispute, confidence, and competing definitions; do not force a pass;
- candidate is a form, mode, structure, audience, medium, or tradition: classify it accurately and do not use genre thresholds to disguise its type.

## 5. Canonical identity, names, and aliases

Each concept receives one stable lowercase ASCII kebab-case `axis-*` ID and one `preferred_label`. Store genuine synonyms, historical names, regional names, language-specific names, and marketing names in `aliases`; an alias never creates a second package.

Normalisation must not erase cultural or historical meaning. When two labels overlap but are not synonyms, use broader, narrower, or `related_ids` relationships and document the boundary. When a regional term is translation-dependent, preserve the original-language term where available, identify the transliteration convention, and record the limitation.

Renaming a preferred label does not change the canonical ID unless an approved version decision requires it. Every rename, merge, split, or reclassification is recorded in the taxonomy changelog after the relevant gate authorises the change.

## 6. Relationship rules

- `parent_ids` and `child_ids` are reciprocal.
- `related_ids` are reciprocal and never substitutes for a known parent-child edge.
- `hybrid_parent_ids` identify every substantive parent of a hybrid; each parent points back to the hybrid through its child relationship.
- A hybrid has one canonical package even when it belongs to multiple families.
- An alias resolves to exactly one canonical ID.
- Self-links, dangling IDs, duplicate edges, and unrecorded one-way relationships are invalid.
- A category may have multiple parents only when sources and distinctiveness evidence support each relationship.
- Relationship graphs must be cycle-checked. A detected cycle requires classification review rather than automatic deletion of an edge.

Neighbour comparisons use stable dimensions and state both overlap and difference. They cannot collapse distinct axes or manufacture hierarchy from familiarity, market size, or geography.

## 7. Indian, regional, oral, and emerging categories

Apply the same recognition and distinctiveness rules to all traditions. Do not raise the evidence bar for Indian, regional, oral, hybrid, historical, or emerging categories, and do not lower it to fill a perceived coverage gap.

Recognition research must include relevant Indian literary institutions, regional and language-specific scholarship, oral and performance traditions, translation scholarship, and documented communities. English-language visibility is not a proxy for corpus existence. An English label must not be imposed as an equivalent when the source tradition does not support that equivalence.

When access, digitisation, cataloguing, or translation limitations prevent a defensible decision, retain the candidate with the limitation and blocked state. Every rejection, borderline case, hybrid, disputed classification, and claim that no Indian equivalent exists receives full independent review.

Emerging categories may use documented community and industry evidence, but the same source-independence, corpus, and distinct-practice requirements apply. Categories discovered after the freeze normally enter the next version.

## 8. Adjudication record

Every decision must state:

- candidate label and proposed canonical ID;
- axis type and preferred label;
- recognition path used;
- resolved source IDs and independent groups;
- corpus work and creator counts;
- distinctiveness dimensions passed and failed;
- nearest neighbours;
- aliases and contested definitions;
- Indian, regional, language, and translation considerations;
- decision: qualify, alias, relate, reject for this version, or disputed;
- decision rationale, verifier, date, and evidence paths.

Recognition decisions, including rejections, are audited at 100%. The decision maker may prepare evidence but cannot supply the final independent verification.

## 9. Freeze and version control

Before G2, the Version 1 registry must contain every qualifying candidate discovered by the recorded `taxonomy_freeze_date`, all canonical identities, aliases, reciprocal relationships, disputed cases, and evidence-linked exclusions.

After G2:

- newly established categories enter the next release unless they correct a material Version 1 omission;
- additions, merges, splits, renames, or reclassifications require a changelog entry, impact assessment, remediation record, and version decision;
- existing package files are never duplicated to accommodate a new parent relationship;
- downstream manifests, indexes, cross-links, and affected evidence are retested;
- a material omission, broken identity, or graph defect blocks the affected family and release.

## 10. Lifecycle and publication control

An axis begins at `identified`. It may enter `taxonomy-verified` only after a recorded recognition decision and canonical ID. It may enter `researching` only after taxonomy freeze and a research-question map. Later transitions follow [the controlled transition graph](../schemas/v1/status-transitions.json).

Recognition or relationship defects set the affected subject to `revision-required` through a recorded defect. No axis, package, family, or release becomes `published` on the basis of taxonomy schema validity alone. Required evidence, analyses, reviews, family completeness, human gates, and release audit must also pass.

