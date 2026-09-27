# Version 1 Data Contracts

These JSON Schema Draft 7 contracts define the structured records that support canonical Markdown content. JSON is used for deterministic interchange and fixtures; Markdown remains the canonical publication format.

## Contracts

| Contract | Purpose |
|---|---|
| `axis.schema.json` | Canonical taxonomy identity and the complete package front matter required by the master plan. |
| `source.schema.json` | Bibliographic, access, verification, reliability, reuse, translation, and copyright metadata. |
| `primary-work.schema.json` | Primary creative-work identity, corpus role, access, and mechanics-analysis fields. |
| `claim.schema.json` | Consequential craft claims, supporting and contrary evidence, scope, exceptions, confidence, and report destinations. |
| `search-log.schema.json` | Reproducible discovery searches, decisions, dead ends, and access constraints. |
| `package-manifest.schema.json` | Canonical package identity, file inventory, hashes, dependency state, and publication readiness. |
| `status.schema.json` | Auditable lifecycle transition event. |
| `sign-off.schema.json` | Sprint, gate, package, family, or release decision with reviewer separation and evidence. |

`controlled-vocabularies.json` is the single review surface for controlled values. The schema enums deliberately mirror it and S01 tests check that they remain synchronized. `status-transitions.json` defines the permitted lifecycle graph; transition enforcement belongs to the permanent S02 harness.

## Contract rules

- Records reject unknown fields with `additionalProperties: false` unless a nested evidence payload is explicitly open.
- Stable IDs are lowercase ASCII kebab-case with a type prefix.
- Required arrays may be empty at early workflow stages unless the record itself represents completed evidence.
- Schema validity does not imply publishability. S02 and later gates enforce cross-record uniqueness, relationship reciprocity, evidence floors, required package files, and stage-dependent completeness.
- Exact dates use ISO `YYYY-MM-DD`; publication dates may use ISO `YYYY`, `YYYY-MM`, or `YYYY-MM-DD` when source precision is limited; timestamps use RFC 3339 date-time strings.
- A primary-work record with `analysis_status: complete` must contain non-empty text in every mechanics field. Nullable mechanics values are permitted only before completion or after a revision reopens the analysis.
- Every claim evidence link labels its expression as a quotation, paraphrase, synthesis, or researcher inference so downstream verification can apply the correct standard.
- Null is permitted only where the workflow explicitly allows information to be unavailable or not yet applicable.
