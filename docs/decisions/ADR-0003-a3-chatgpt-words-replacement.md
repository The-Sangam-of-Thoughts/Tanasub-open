# ADR-0003: A3 External Acquisition — Replace `chatgpt-words` with Research-Derived Approach

## Status

Accepted — 2026-09-23

## Context

The original conversion plan (Phase A3) referenced an external repository
`alexander-stewart/chatgpt-words` as a source for vocabulary-awareness terms
and humanization patterns. During implementation, this repository was found to
not resolve: the GitHub path does not point to an accessible public repository,
and no license or immutable revision could be obtained.

Meanwhile, the project independently developed a research-derived approach to
vocabulary awareness and humanization:

- `references/word-awareness-index.md` — project-authored prompts combined with
  categories observed in WikiProject AI Cleanup and vocabulary-awareness cautions
  motivated by population-level biomedical research. The file explicitly notes
  that `chatgpt-words` supplied no terms or data.
- `references/humanization-guide-full.md` — documented methodology for contextual
  voice calibration, cadence variation, and elimination of artificial tropes.
  The file explicitly notes that `chatgpt-words` supplied no data or license.

Both files are accepted, independently reviewed, and in active use. The
research-derived approach is not dependent on any external acquisition.

## Decision

Record an owner-approved plan amendment that replaces the `chatgpt-words`
external acquisition with the already documented research-derived approach.

Concretely:

1. **A3 is closed** with the research-derived approach as the accepted basis.
   No further search for `chatgpt-words` is required.
2. **E2 (Fabric flattening)** is unblocked. The Fabric files in
   `external/fabric-humanize/` are already flattened, retain their MIT licence,
   and have upstream paths recorded in `UPSTREAM.md`.
3. The roadmap and TODO.md are updated to reflect this amendment.

## Consequences

- A3 no longer blocks E2 or any downstream phase.
- The `chatgpt-words` name is retained in historical references only. No new
  material may be attributed to it.
- The research-derived vocabulary and humanization files remain the canonical
  source for their respective domains.
