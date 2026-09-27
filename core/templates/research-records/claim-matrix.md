# Claim Matrix — {{claim_id}}

**Axis:** {{axis_id}}  
**Template status:** {{status}}  
**Last verified:** {{date}}

Use one copy per consequential craft claim to prepare a JSON record governed by `schemas/v1/claim.schema.json`. Do not copy advice to another axis unless that destination is explicitly supported by the evidence and recorded in `axis_ids` and `report_locations`.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Claim ID | `id` | yes | Stable lowercase `clm-...` ID; corresponds to `{{claim_id}}`. |
| Craft claim | `craft_claim` | yes | Exact, testable recommendation; avoid unsupported universals. |
| Axis IDs | `axis_ids[]` | yes | One or more supported canonical axes, including `{{axis_id}}` where applicable. |
| Supporting evidence | `supporting_evidence[]` | yes | At least one evidence link with all four nested fields. |
| Counterevidence | `counterevidence[]` | yes | Contrary evidence or an explicit empty array after a documented search. |
| Scope | `scope` | yes | Cultural, historical, linguistic, audience, form, medium, and situational boundary. |
| Exceptions | `exceptions[]` | yes | Known cases where the recommendation should not be followed. |
| Confidence | `confidence` | yes | `strong`, `moderate`, `limited`, or `disputed`. |
| Report locations | `report_locations[]` | yes | One or more forward-slash Markdown paths, with optional anchors. |
| Inference label | `inference_label` | yes | `source-stated`, `synthesis`, or `researcher-inference`. |
| Last verified | `last_verified` | yes | ISO date corresponding to `{{date}}`. |

Each item in `supporting_evidence` or `counterevidence` maps exactly to `evidence_id`, `location`, `evidence_expression`, and `note`. `evidence_expression` must be one of `quotation`, `paraphrase`, `synthesis`, or `researcher-inference`.

## Claim statement

- Exact craft recommendation:
- Intended writer action or diagnostic outcome:
- Consequential because:
- Inference label:

## Supporting evidence

| Evidence ID | Exact location | Expression type | What it supports | Direct-verification evidence path |
|---|---|---|---|---|
|  |  | `quotation`, `paraphrase`, `synthesis`, or `researcher-inference` |  |  |

Quotations require direct verification and minimal lawful excerpting. Paraphrases must preserve meaning without quotation styling. Synthesis must name its inputs. Researcher inference must not be attributed to a source.

## Counterevidence and disagreement

| Evidence ID | Exact location | Expression type | What it challenges or qualifies | Direct-verification evidence path |
|---|---|---|---|---|
|  |  | `quotation`, `paraphrase`, `synthesis`, or `researcher-inference` |  |  |

If the JSON array is empty, record the contrary/revisionist searches performed and their search-log IDs. Absence of located counterevidence is not proof of universality.

## Scope

- Supported axis IDs:
- Forms, modes, structures, audiences, and media:
- Historical periods:
- Languages, regions, and traditions:
- Indian contexts and closest relevant traditions:
- Translation dependence:
- Screen/adaptation relevance:
- Conditions under which the recommendation works:

## Exceptions and limits

- Known exceptions and counterexamples:
- Functional equivalents where the advice does not naturally apply:
- Evidence shortages and access constraints:
- Copyright or quotation limitations:
- Risk of copying the advice to unsupported axes:

## Confidence and destinations

- Controlled confidence:
- Confidence rationale, including disagreement and source independence:
- Required review depth: all `limited` and `disputed` claims receive full review
- Report locations:
- Claim IDs superseded or qualified:
- Last verified date:

## Reception boundary

- Professional criticism evidence and supported reception claim:
- Audience-response evidence and supported reception claim:
- Separation check:
- Writing-level implication versus excluded non-writing factors:

## Verification and remediation

- Dates, titles, creators, classifications, numerical assertions, quotations, and translations directly checked:
- Open evidence-affecting finding:
- Remediation action, owner, due date, and retest evidence path:
- Independent reviewer:

The author may assess readiness but may not sign off or independently verify this claim.

## Transfer and destination test

For every destination in `axis_ids` and `report_locations`, record a relevance rationale, direct supporting evidence or labelled bounded inference, counter-search ID, and exception. A general source may motivate a hypothesis but does not establish a destination-specific convention. Delete no limitation merely because the same wording appears in another axis; unsupported destinations remain absent from the record and report.
