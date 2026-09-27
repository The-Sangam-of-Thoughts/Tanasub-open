# Axis Package Manifest — {{package_id}}

**Axis:** {{axis_id}}  
**Canonical path:** {{canonical_path}}  
**Version:** {{version}}  
**Taxonomy freeze date:** {{taxonomy_freeze_date}}  
**Lifecycle status:** {{status}}

Use this worksheet to prepare one JSON record governed by `schemas/v1/package-manifest.schema.json`. A complete-looking manifest does not make a package publishable; the QA harness and required independent and human gates remain authoritative.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Package ID | `package_id` | yes | Stable lowercase `pkg-...` ID; corresponds to `{{package_id}}`. |
| Axis ID | `axis_id` | yes | Canonical `axis-...` ID; corresponds to `{{axis_id}}`. |
| Canonical path | `canonical_path` | yes | One current `genres/<axis>.md` or `subgenres/<axis>.md` path. |
| Version | `version` | yes | Semantic `x.y.z` value. |
| Taxonomy freeze date | `taxonomy_freeze_date` | yes | ISO date or null before G2. |
| Lifecycle status | `lifecycle_status` | yes | Exact controlled lifecycle value. |
| Files | `files[]` | yes | At least one object with `path`, `artifact_type`, `sha256`, and `status`. |
| Source IDs | `source_ids[]` | yes | Unique canonical source references. |
| Primary-work IDs | `primary_work_ids[]` | yes | Unique canonical work references. |
| Claim IDs | `claim_ids[]` | yes | Unique canonical claim references. |
| Required predecessors | `required_predecessors[]` | yes | Unique valid sprint IDs. |
| Generated at | `generated_at` | yes | RFC 3339 timestamp. |

## Package identity and dependency state

- Package ID:
- Axis ID and authoritative axis-record path:
- Canonical package path:
- Content version:
- Taxonomy freeze date or reason for null:
- Lifecycle status and status-history evidence path:
- Required predecessor sprints and sign-off evidence paths:
- Generation timestamp and operator:

## File inventory

Record every canonical Markdown artifact exactly once. Hashes may be null only where the schema permits; publication readiness requires validated current hashes.

| Path | Controlled artifact type | SHA-256 | File status | Evidence or dependency note |
|---|---|---|---|---|
|  |  |  | `shell`, `in-progress`, `complete`, or `revision-required` |  |

Confirm inventory coverage for the core guide, files `01`–`15`, at least three close readings, one neighbour comparison, one reception/failure-pattern analysis, package research links, manifest, and genre map where applicable. A functional equivalent must be documented within the relevant file when a standard topic does not apply.

## Evidence references and floors

- Source IDs:
- Primary-work IDs:
- Claim IDs:
- Secondary-source count and QA evidence path:
- Primary-work count and QA evidence path:
- Creator count:
- Historical stages:
- Cultural and linguistic traditions:
- Formative, recognized, and contemporary coverage:
- Counterevidence coverage:

Never pad a quota. If credible evidence is insufficient, set the lifecycle state to `evidence-incomplete` and block downstream publication.

## Indian, regional, translation, screen, and reception coverage

- Indian examples or evidence-based absence record:
- Indian-language and regional traditions:
- Translation notes and limitations:
- Screen/adaptation relevance and writing-level boundary:
- Professional criticism coverage:
- Audience-response coverage kept separate:

## Publication-readiness checks

- Schema-valid axis and linked records:
- Unique IDs and reciprocal relationships:
- Mandatory file completeness:
- Citation and claim resolution:
- Forward-slash internal links and index membership:
- No accidental unresolved markers:
- Approved template tokens removed from publishable package content:
- Copyright and lawful-excerpt review:
- No invented quotation, translation, date, identity, classification, number, or research claim:
- No critical, high, or evidence-affecting medium finding open:
- Automated run evidence paths:
- Manual sample evidence paths:
- Independent review and sign-off evidence paths:
- Human gate evidence path where required:

Any failed validation means publication is blocked. Automated success is not human approval.

## Remediation history

| Finding ID | Severity | Affected artifact | Corrective action | Owner | Retest evidence path | Disposition |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |

Preserve original failed evidence separately from every retest; never replace a failed run with a successful result.
