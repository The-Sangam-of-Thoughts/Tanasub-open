# Research Workflow

**Version:** 1.0.0  
**Scope:** operational flow from candidate discovery to controlled publication  
**Authority:** [methodology](methodology.md), [taxonomy rules](taxonomy-rules.md), [source policy](source-policy.md), sprint governance, and [status transitions](../schemas/v1/status-transitions.json)  
**Approval state:** prepared for independent review and G1 human decision; this file is not an approval record

## 1. Roles and separation of duties

Every work item names:

- one exclusive author or production owner;
- one independent reviewer who is not the author;
- a human gate reviewer where the plan requires one;
- an integration owner for shared plans, schemas, vocabularies, indexes, dashboards, manifests, and release records.

Production owners may create and self-check only their assigned artifacts. They do not edit frozen shared inputs, approve their own output, or overwrite prior evidence. A missing reviewer leaves the item open.

## 2. Ready check

Work begins only when all applicable conditions are recorded:

1. sprint, story, artifact class, and exclusive owner are identified;
2. predecessor sprint or series has passed;
3. the governing schema, template, and acceptance criteria exist;
4. inputs are available and named in the sprint manifest;
5. the final verifier is named and independent;
6. the story is eight points or fewer and belongs to the sprint's single artifact class;
7. automated checks and manual sample are defined;
8. evidence, access, translation, copyright, privacy, and dependency risks are recorded;
9. for axis work, the axis is present in the applicable frozen taxonomy.

If any condition fails, record the exact blocker and perform only the review or remediation needed to restore readiness.

## 3. End-to-end flow

### Step 1 — Register and discover

Create the candidate or axis ID and all applicable search logs. Run distinct source streams rather than one blended search. Preserve queries, dates, languages, regions, inclusions, exclusions, dead ends, and access constraints.

**Stop if:** search provenance is missing, the candidate identity collides, or an applicable Indian/regional stream is omitted without a recorded reason.

### Step 2 — Adjudicate taxonomy

Resolve source independence, recognition path, corpus counts, distinctiveness dimensions, axis type, aliases, neighbours, and reciprocal relationships under [taxonomy-rules.md](taxonomy-rules.md). Record rejected and disputed candidates as well as accepted ones.

**Advance:** `identified` to `taxonomy-verified` only with `recognition-decision` and `canonical-id` evidence.

**Stop if:** threshold calculation, classification, relationship reciprocity, or independent review is incomplete.

### Step 3 — Freeze and map questions

After the applicable taxonomy freeze, create the axis-specific research-question map. It must cover every mandatory topic and identify functional equivalents for topics that do not naturally apply.

**Advance:** `taxonomy-verified` to `researching` only with `taxonomy-freeze` and `research-question-map` evidence.

### Step 4 — Evaluate and record sources

Inspect each source directly and create its `src-*` record. Assign source type, roles, reliability, access, translation, copyright, axes, and claims. Label every extracted item by expression type. Record contradictory evidence and limitations.

**Stop if:** direct verification cannot be completed, copyright status makes repository storage unsafe, or the source cannot support its assigned role. The source may remain excluded or limited; it cannot silently enter evidence counts.

### Step 5 — Analyse primary works

Create `work-*` records and inspect the stated edition or version. Complete all mechanics fields when `analysis_status` becomes `complete`, keeping critical and audience reception separate. Record a reasoned functional equivalent when a conventional mechanic does not apply.

**Stop if:** title, creator, date, category membership, edition, language, translator, or quotation is unverified.

### Step 6 — Build claims and countercheck

Create `clm-*` records for consequential recommendations. Link supporting evidence, run and retain a `contrary-revisionist` search, record counterevidence, define scope and exceptions, assign confidence, identify report locations, and label the inference.

**Stop if:** a consequential claim lacks resolved support, provenance, scope, counterevidence treatment, or a valid report destination. Never transfer a claim to a second axis until the record explicitly supports it.

### Step 7 — Test evidence sufficiency

Calculate source, work, creator, historical, cultural/linguistic, formative, recognised, contemporary, Indian/regional, contrary-view, and applicable screen/adaptation coverage from resolved records.

**Advance:** `researching` or `evidence-incomplete` to `evidence-complete` only with `evidence-floor-pass` and `g4-approval`.

**Branch:** when a documented search exposes a material gap, use `researching` to `evidence-incomplete` with `documented-search` and `evidence-gap`. Reopen through the allowed remediation path. Never pad a count.

### Step 8 — Produce analyses breadth-first

Complete the scheduled artifact class for every axis in the batch before advancing the series. Use only approved templates, dossiers, source records, work records, and claim matrices. Run completeness, reference, unresolved-marker, and content-specific checks after each artifact handoff.

**Advance:** `evidence-complete` to `analysis-complete` only with `mandatory-analysis-pass` and `case-study-pass`.

### Step 9 — Draft practitioner content last

After supporting analyses pass, draft the main guide, exercises, revision tools, and annotated sources. Do not introduce unsupported claims. Link exercises to findings and failure diagnoses.

**Advance:** `analysis-complete` to `drafted` only with `main-guide-pass`, `exercise-pass`, and `annotated-sources-pass`.

### Step 10 — Independent editorial review

The non-author reviewer evaluates teachability, evidence fidelity, disagreement, cultural and historical scope, originality, diagnostics, accessibility, exercise alignment, cross-links, and revision utility. Findings cite exact artifacts and severities.

**Advance:** `drafted` to `editorially-reviewed` only with `independent-editorial-review` and `g5-approval`.

### Step 11 — Family and release control

Confirm the parent, every frozen child, and every shared blocking hybrid is complete; aliases resolve; links are reciprocal; manifests and hashes pass; and the release audits are complete.

**Advance:** `editorially-reviewed` to `published` only with `family-complete`, `g6-approval`, and `release-audit-pass`.

No automated result substitutes for a named human gate decision.

## 4. Defect and remediation flow

When a defect is found:

1. assign a stable finding ID, severity, affected artifacts, owner, and due date;
2. decide whether it affects evidence, taxonomy, factual accuracy, copyright, downstream claims, or publication control;
3. preserve the original artifact hashes, automated results, manual sample, and failure register;
4. set the affected subject to `revision-required` through a `recorded-defect` transition; a published subject also requires `release-impact-assessed`;
5. approve a bounded remediation scope;
6. return from `revision-required` to `researching` only with `remediation-scope-approved`;
7. apply only the scoped correction;
8. write a separate retest result and have a non-author reviewer verify it;
9. close the finding only when the evidence path and closure date are recorded.

Critical and high findings always block. Medium findings block when they affect taxonomy, evidence sufficiency, factual accuracy, copyright, or a downstream consequential claim. Low findings may be deferred only with an owner and release-blocking due date.

## 5. Test and audit package

Each sprint retains these files under `tests/runs/<sprint-id>/`:

- `manifest.yaml` with environment, operator, inputs, validators, timing, revision, and hashes;
- `automated-results.json` with expected and actual outcomes by test ID;
- `manual-sample.md` with population, sampled records, method, evidence, reviewer, and result;
- `failures.csv` with severity, owner, disposition, retest ID, and closure date;
- `retest-results.json`, separate from the original result.

Each sprint retains `sprint-audit.md`, `traceability.csv`, `exceptions.md`, `remediation.md`, and `sign-off.yaml` under `audits/sprints/<sprint-id>/`.

Original results are immutable. A retest adds evidence and never replaces the failure it addresses. Passed artifacts are changed only through recorded remediation and version control.

## 6. Manual sampling procedure

Build the sample population from resolved record IDs, then select and record:

- 100% of quotations, translations, dates, titles, creator identities, recognition decisions, numerical assertions, limited-confidence claims, disputed claims, insufficient-evidence records, and no-Indian-equivalent conclusions;
- 10% of all other consequential claims per batch, minimum five and maximum twenty, or all when fewer than five exist;
- at least one Indian or regional record in every applicable batch.

For each item, the reviewer inspects the cited source or work directly, checks identity and locator, compares expression type to the evidence, verifies scope and exception handling, and records pass or a defect. The sample record identifies the population, deterministic or documented selection method, selected IDs, reviewer, date, source consulted, and result.

## 7. Deterministic validation and publication interlock

Run the permanent QA harness against the integrated repository. Repeat clean runs when the sprint or release plan requires deterministic confirmation, retain each output separately, and compare normalized reports or recorded hashes.

The harness checks stable IDs, schema-valid front matter, mandatory files, internal links and citations, evidence floors, graph reciprocity, lifecycle transitions, unfinished-marker rules, manifests and hashes, indexes and orphans, reviewer separation, and publication interlock.

Only the approved closed vocabulary of double-brace tokens may appear, and only within configured template paths. Method files and publishable package content contain no such tokens. Unknown tokens, approved tokens in a non-template path, ordinary unfinished markers, or any other finding must produce a nonzero result and `publication_allowed: false`.

If validation fails, publication and lifecycle advancement stop. Record the failure, remediate within ownership, retain the first result, and rerun into a separate evidence file.

## 8. Completion checklist

An artifact or sprint is complete only when:

- the artifact is substantive, schema-valid where applicable, and free of unfinished markers;
- acceptance criteria and evidence floors pass without padding;
- citations, source IDs, work IDs, claim IDs, relationships, and links resolve;
- automated results and required deterministic reruns pass;
- manual fact and claim sampling passes;
- original failures and separate retests are retained;
- no blocking finding remains open;
- the independent reviewer records acceptance;
- the human gate records `pass` where required;
- status, dashboard, manifest, audit, and sign-off records agree.

Until every applicable item is present, the outcome is `ready-for-review`, `blocked`, or `fail`, never `pass`.

## 9. Per-axis readiness dashboard and stop rules

Maintain one current row per axis and artifact class with taxonomy state; source, work, creator, and reception counts; required diversity dimensions; direct-verification status; evidence gaps; claim-matrix revision; mandatory and supplementary artifact paths; open finding IDs; input manifest hash; author check; independent review; human decision; and release eligibility. These fields report separate facts. A green automated check, an unassigned reviewer label, or a historical result must never populate an independent-review or human-decision field.

Stop an artifact handoff when its exact approved template, axis dossier, required source/work records, claim matrix, or verification events are missing; when a claim would need unsupported transfer; or when a source, edition, locator, translation, or work/category relationship is unverified. The author records the unmet input and affected destinations, then works only on an independent remediation task. A package with state `researching` or `evidence-incomplete` may remain a draft but cannot enter a family or release workflow.

For each completed handoff, retain the changed paths, requirement and finding IDs, input/output hashes, author self-check, unresolved limitations, and deterministic check result. The integration owner reconciles these rows with manifests and the current-status record before a lifecycle advance.
