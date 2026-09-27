# S03 Template Index

These are reusable research and editorial contracts, not completed research or publishable axis packages.

## Research records

| Template | Authoritative contract |
|---|---|
| `research-records/search-log.md` | `schemas/v1/search-log.schema.json` |
| `research-records/source-record.md` | `schemas/v1/source.schema.json` |
| `research-records/primary-work.md` | `schemas/v1/primary-work.schema.json` |
| `research-records/claim-matrix.md` | `schemas/v1/claim.schema.json` |
| `research-records/package-manifest.md` | `schemas/v1/package-manifest.schema.json` |
| `research-records/audit.md` | Sprint audit contract in `00_Project_Method/repository-contract.md` |
| `research-records/sign-off.md` | `schemas/v1/sign-off.schema.json` |

## Editorial templates

`editorial/` contains the main `00-how-to-write.md`, the required analyses `01` through `15`, and separate close-reading, neighbour-comparison, reception-analysis, exercise, genre-map, and independent-editorial-review templates.

## Token and release boundary

Only double-brace token names declared in `tools/qa/qa-config.json` are valid here. Their presence identifies an uninstantiated template; generated canonical package content must resolve every token. An approved token outside an approved template path, an unknown token, or an unresolved drafting marker blocks publication.

Templates supply structure and prompts, not evidence. They must never be read as claims that any taxonomy, corpus, package, dossier, or encyclopedia edition is complete.

## R1 use contract

Instantiate a template only from a named revision of the approved template, axis dossier, verified record set, and claim matrix. Before drafting, record the assigned artifact paths, finding IDs in scope, and required functional equivalents. Before handoff, return a section-purpose/evidence matrix, changed paths, unresolved limits, and author-check results. Templates may guide research and drafting while evidence is incomplete, but the resulting artifact remains blocked from lifecycle advance and release.

Every template section must produce a distinct reader or research function. A heading is complete only when it identifies its purpose, its supporting claim or verification-event IDs where consequential, a concrete result or example, scope or limitation, and the next action for researcher, writer, or reviewer. Do not fill template headings with stock prose, copied recommendations, invented examples, or approval language.
