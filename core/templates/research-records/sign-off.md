# Review Sign-Off — {{signoff_id}}

**Scope:** {{sprint_id}}  
**Decision date:** {{date}}  
**Decision status:** {{status}}

Use this worksheet to prepare one JSON record governed by `schemas/v1/sign-off.schema.json`. Only the identified independent reviewer may render the independent decision. The preparer may not use this template to approve their own work.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Sign-off ID | `signoff_id` | yes | Stable lowercase `signoff-...` ID; corresponds to `{{signoff_id}}`. |
| Scope type | `scope_type` | yes | `sprint`, `gate`, `package`, `family`, or `release`. |
| Scope ID | `scope_id` | yes | Exact reviewed scope identifier; `{{sprint_id}}` is suitable for a sprint scope. |
| Preparer | `preparer` | yes | Artifact preparer identity. |
| Independent reviewer | `independent_reviewer` | yes | Non-author reviewer identity; `{{reviewer_id}}` may be used during instantiation. |
| Human gate reviewer | `human_gate_reviewer` | yes | Reviewer identity or null when no human gate applies; pending is not approval. |
| Decided at | `decided_at` | yes | RFC 3339 timestamp. |
| Status | `status` | yes | Exact decision: `pass` or `fail`. |
| Blocking findings | `blocking_findings[]` | yes | Each object maps all five required nested fields. |
| Evidence paths | `evidence_paths[]` | yes | At least one unique repository-relative evidence path. |
| Notes | `notes` | yes | Decision rationale and limits. |

Each `blocking_findings` item maps exactly to `finding_id`, `severity`, `summary`, `owner`, and `due_date`.

## Scope and identities

- Scope type:
- Scope ID:
- Artifacts reviewed:
- Preparer:
- Independent reviewer:
- Human gate reviewer or explicit non-applicability:
- Ownership-register evidence path:
- Identity-separation check:
- Decision timestamp:

The independent reviewer must differ from the preparer. Where a human gate is required, a null or unavailable human reviewer cannot yield gate approval.

## Evidence reviewed

- Frozen input and output hashes:
- Original automated results:
- Original failure register:
- Separate retest results:
- Deterministic rerun comparison:
- Manual sample or usability trial:
- Sprint audit and traceability:
- Exceptions and remediation:
- Publication-blocking negative tests:
- Approved-token scope and unresolved-marker tests:
- Copyright and sensitive-content checks:

## Review findings

| Finding ID | Severity | Summary | Owner | Due date | Evidence path | Retest evidence path | Open or closed |
|---|---|---|---|---|---|---|---|
|  | `critical`, `high`, `medium`, or `low` |  |  |  |  |  |  |

Include every open blocking finding in the structured `blocking_findings` array. A `pass` decision requires no unresolved critical, high, or evidence-affecting medium finding.

## Evidence-integrity decision

- Provenance and direct verification adequate:
- Quotation, paraphrase, synthesis, and researcher inference distinguished:
- Counterevidence, scope, exceptions, and confidence exposed:
- Access constraints and evidence limitations visible:
- Indian, regional, and translation coverage adequate for scope:
- Professional criticism and audience response separated:
- Copyright boundary and repository-copy permissions respected:
- Evidence paths resolve:

## Decision

- Status: only `pass` or `fail`
- Publication permitted by current automated result:
- Independent-review decision and rationale:
- Human-gate decision and rationale, when applicable:
- Blocking findings remaining:
- Required remediation and owner:
- Decision evidence paths:
- Limitations and notes:

Automated success cannot be represented as independent acceptance or human approval. A failed validation blocks publication. Preserve initial failures and record every remediation retest separately.
