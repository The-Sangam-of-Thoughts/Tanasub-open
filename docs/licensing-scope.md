# Licensing scope and intake status

This file records the current repository boundary; it is not legal advice or a substitute for a complete copyright review.

## Current scope

| Material | Current treatment | Distribution implication |
|---|---|---|
| Project-authored code and documentation unless otherwise marked | Root MIT licence | Redistributable under the root licence |
| `references/humanization-guide-full.md` | Contains adapted CC BY-SA 4.0 material | Keep attribution and share-alike notice with the adapted material |
| `references/structural-tells-catalog.md` | Adapted CC BY-SA 4.0 material | Keep attribution and share-alike notice |
| `references/word-awareness-index.md` | Adapted CC BY-SA 4.0 material | Keep attribution and share-alike notice |
| `layers/layer2-humanize.md` | Identified by the adaptation notice as part of the same adaptation set | Treat the adapted material as CC BY-SA 4.0 until file-level marking is completed |
| `external/fabric-humanize/` | Vendored MIT snapshot with pinned revision and checksums | Preserve upstream licence and provenance |
| `external/humanizer/` | Integration notes and licence exist, but the recorded upstream content is not actually vendored | Incomplete candidate; do not describe as an integrated dependency |
| Evidence records for copyrighted books and works | Bibliographic and analytical records, not licensed source-text bundles | Do not treat the records as permission to reproduce source works |

The root MIT licence does not erase narrower terms attached to identified third-party or adapted files. A future `LICENSES/` and file-level SPDX/REUSE pass must make these scopes machine-checkable.

## Open-source intake rule

Every dependency or vendored candidate requires:

1. exact repository, tag or commit, and cryptographic hash;
2. code, model, dataset, and content licences recorded separately;
3. transitive dependency and security review;
4. chosen integration mode: dependency, vendored snapshot, separate process, remote service, or clean-room implementation;
5. upgrade, replacement, and removal plan;
6. explicit review state before use.

Permissive licensing does not by itself establish suitability. Maintenance, security, data rights, model terms, service terms, and trademark constraints remain separate checks.

## Intake rule for restricted material

No public content, third-party dataset, prompt collection, model, or open-source component enters this repository merely because it is visible online. Reciprocal, source-available, non-commercial, no-derivatives, or unlicensed material remains excluded until a documented review approves the exact use.

Competitor research produces neutral capability specifications. It must not transfer proprietary prompts, code, client bundles, datasets, private traces, or protected expression into this repository.

## Completed follow-ups — 2026-09-22

- **File-level licence markings**: Added SPDX headers to all four humanization
  adaptation files: `references/humanization-guide-full.md`,
  `references/structural-tells-catalog.md`, `references/word-awareness-index.md`,
  and `layers/layer2-humanize.md`. Each now carries a `CC-BY-SA-4.0` identifier.
- **LICENSES/ directory**: Created with MIT and CC-BY-SA-4.0 full licence texts
  and a `README.md` mapping every file to its licence.
- **external/humanizer/ reconciliation**: Documented that this directory is an
  acquisition research record, not a vendored dependency. The `UPSTREAM.md` file
  explicitly states the actual files were never downloaded. This directory should
  not be described as vendored, integrated, or included in any SBOM.
- **Root copyright notice**: Reviewed and documented. The notice uses the
  historical project name variant ("Encyclopedic Creative-Writing Library
  Project Contributors") to maintain traceability. Individual contribution
  history is preserved in the Git commit log. No rewrite of historical
  ownership was performed.

## Open findings

- **SBOM deferred**: No executable dependency set is locked. The repository
  contains reference documentation and creative content, not a deployable
  application. The only external acquisition (`external/fabric-humanize/`) is
  a vendored MIT snapshot with no transitive dependencies. An SBOM will be
  generated when this repository gains a deployable component with an
  executable dependency set.
