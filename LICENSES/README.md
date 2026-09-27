# Licence Mapping

This directory provides machine-readable licence texts for REUSE/SPDX compliance.

## Licences in Use

| Licence | Identifier | Files |
|---------|-----------|-------|
| MIT | MIT | All project-authored code and documentation unless otherwise marked |
| CC-BY-SA-4.0 | CC-BY-SA-4.0 | Four humanization adaptation files (see below) |

## File-Level SPDX Identifiers

### MIT-licensed (root licence)

All files in the repository are MIT-licensed unless they contain an explicit
CC-BY-SA-4.0 header. The root `LICENSE` file applies to:

- All files under `genres/`, `subgenres/`, `layers/` (except layer2-humanize.md),
  `docs/`, `core/`, `references/` (except the three adapted files),
  and `platform-adapters/`.
- `external/fabric-humanize/` (vendored MIT snapshot).

### CC-BY-SA-4.0-licensed (adapted material)

These four files contain adapted material from WikiProject AI Cleanup's
field guide (CC BY-SA 4.0) and require share-alike attribution:

1. `references/humanization-guide-full.md`
2. `references/structural-tells-catalog.md`
3. `references/word-awareness-index.md`
4. `layers/layer2-humanize.md`

Each file carries an SPDX licence identifier header. The original
WikiProject AI Cleanup field guide is available at:
https://en.wikipedia.org/wiki/Wikipedia:WikiProject_AI_Cleanup/field_guide

### External acquisitions

| Path | Licence | Status |
|------|---------|--------|
| `external/fabric-humanize/` | MIT | Vendored snapshot, pinned revision, checksums recorded |
| `external/humanizer/` | MIT (upstream) | Integration notes only; NOT vendored (see below) |

## external/humanizer/ Reconciliation

The `external/humanizer/` directory does NOT contain vendored upstream files.
It contains only integration analysis documents and a copy of the upstream
MIT licence. The `UPSTREAM.md` file explicitly states: "The actual files need
to be vendored by downloading from the pinned commit."

This directory is therefore an acquisition research record, not a distributed
dependency. It should not be described as vendored, integrated, or included
in any SBOM. The integration analysis was used to inform Layer 2 humanization
design decisions but the upstream code was never incorporated.

## SBOM Deferral

A Software Bill of Materials (SBOM) is deferred because:

1. No executable dependency set has been locked. The repository contains
   reference documentation and creative content, not a deployable application.
2. The only external acquisition (`external/fabric-humanize/`) is a vendored
   MIT snapshot with no transitive dependencies.
3. The `external/humanizer/` directory is not a dependency—it is research notes.

An SBOM will be generated when this repository gains a deployable component
with runtime dependencies.

## Root Copyright Notice

The root copyright notice reads:

    Copyright (c) 2026 Encyclopedic Creative-Writing Library Project Contributors

This notice was established during the public rebrand from "Universal Writing
Guide" to "Tanasub Open." It does not rewrite historical ownership—it records
the collective contributor base as of the rebrand date. Individual contribution
history is preserved in the Git commit log. The notice intentionally uses the
project's historical name variant ("Encyclopedic Creative-Writing Library
Project") to maintain traceability to the pre-rebrand identity.
