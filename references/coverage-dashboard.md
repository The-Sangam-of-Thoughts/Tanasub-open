# Taxonomy and Craft Coverage Dashboard

- **Taxonomy Freeze Date:** 2026-09-12
- **Taxonomy version:** 1.0.0 (Gate G2 Approved)
- **Total Frozen Axes:** 32

## Status Summary

| Axis Type | Count | Lifecycle Status |
|---|---|---|
| Genre | 11 | `taxonomy-verified` |
| Subgenre | 8 | `taxonomy-verified` |
| Form | 8 | `taxonomy-verified` |
| Mode | 3 | `taxonomy-verified` |
| Structure | 1 | `taxonomy-verified` |
| Tradition | 1 | `taxonomy-verified` |
| **Total** | **32** | `taxonomy-verified` |

## Registered Axes

| Canonical ID | Preferred Label | Type | Region | Language | Parents | Children |
|---|---|---|---|---|---|---|
| `axis-bildungsroman` | Bildungsroman | `subgenre` | global | `en` | none | none |
| `axis-cozy-mystery` | Cozy Mystery | `subgenre` | global | `en` | axis-detective-and-mystery-fiction | none |
| `axis-cyberpunk` | Cyberpunk | `subgenre` | global | `en` | axis-science-fiction | none |
| `axis-dastan-tradition` | Dastan Tradition | `tradition` | South Asia | `ur` | none | none |
| `axis-detective-and-mystery-fiction` | Detective and Mystery Fiction | `genre` | global | `en` | none | axis-cozy-mystery |
| `axis-episodic-television-script` | Episodic Television Script | `form` | global | `en` | none | none |
| `axis-epistolary-fiction` | Epistolary Fiction | `form` | global | `en` | none | none |
| `axis-fantasy-fiction` | Fantasy Fiction | `genre` | global | `en` | axis-speculative-fiction | axis-urban-fantasy |
| `axis-feature-screenplay` | Feature Screenplay | `form` | global | `en` | none | none |
| `axis-flash-fiction` | Flash Fiction | `form` | global | `en` | none | none |
| `axis-frame-narrative` | Frame Narrative | `structure` | global | `en` | none | none |
| `axis-ghazal-sequence` | Ghazal Sequence | `form` | South Asia | `ur` | none | none |
| `axis-gothic-fiction` | Gothic Fiction | `genre` | global | `en` | none | none |
| `axis-historical-fiction` | Historical Fiction | `genre` | global | `en` | none | none |
| `axis-horror-fiction` | Horror Fiction | `genre` | global | `en` | axis-speculative-fiction | none |
| `axis-interactive-fiction` | Interactive Fiction | `form` | global | `en` | none | none |
| `axis-katha-tradition` | Katha Tradition | `form` | India | `sa` | none | none |
| `axis-nataka-drama` | Nataka Drama | `genre` | India | `sa` | none | none |
| `axis-pastoral-literature` | Pastoral Literature | `mode` | global | `en` | none | none |
| `axis-picaresque-literature` | Picaresque Literature | `genre` | global | `en` | none | none |
| `axis-prakarana-drama` | Prakarana Drama | `genre` | India | `sa` | none | none |
| `axis-psychological-fiction` | Psychological Fiction | `subgenre` | global | `en` | none | none |
| `axis-psychological-thriller` | Psychological Thriller | `subgenre` | global | `en` | axis-thriller-fiction | none |
| `axis-romance-fiction` | Romance Fiction | `genre` | global | `en` | none | none |
| `axis-satirical-literature` | Satirical Literature | `mode` | global | `en` | none | none |
| `axis-science-fiction` | Science Fiction | `genre` | global | `en` | axis-speculative-fiction | axis-cyberpunk, axis-space-opera |
| `axis-solarpunk` | Solarpunk | `subgenre` | global | `en` | axis-speculative-fiction | none |
| `axis-space-opera` | Space Opera | `subgenre` | global | `en` | axis-science-fiction | none |
| `axis-speculative-fiction` | Speculative Fiction | `mode` | global | `en` | none | axis-fantasy-fiction, axis-horror-fiction, axis-science-fiction, axis-solarpunk |
| `axis-thriller-fiction` | Thriller Fiction | `genre` | global | `en` | none | axis-psychological-thriller |
| `axis-urban-fantasy` | Urban Fantasy | `subgenre` | global | `en` | axis-fantasy-fiction | none |
| `axis-vachana-poetry` | Vachana Poetry | `form` | India | `kn` | none | none |

## Tone layer coverage — as of 2026-09-24 21:23 +05:30

Counts below were derived from the filesystem at the stated timestamp while
the Tone Layer program (TAN-201…TAN-240) was **still in flight** — review lanes
(TAN-231…TAN-234), matrix integration (TAN-236), registry registration
(TAN-237), and the TAN-239/TAN-240 gates remain open. Treat every record count
here as a dated floor, not a final figure; refresh again at the TAN-239 gate
and at TAN-240.

| Metric | Count (2026-09-24 21:23 +05:30) |
|---|---|
| Product version (README badge) | 2.1.0 |
| Tones in frozen taxonomy (5 families) | 19 |
| Tone evidence silos (`references/tone-evidence/`) | 19 directories |
| Tones with `dossier.md` | 19 / 19 (all with sections A–I per `fill_tone_coverage.py`; content acceptance not re-verified) |
| Tones with card file (`tones/<name>.md`) | 19 / 19 |
| Cards validated | 19 checked, 0 failing |
| Claim records across silos | 215 |
| Source records across silos | 378 |
| Primary-work records across silos | 117 |
| Total evidence records (JSON) | 710 |
| Distinct record IDs | 703 of 710 entries; 6 work IDs occur in more than one silo (`work-annihilation-of-caste`, `work-ghalib-letters`, `work-malgudi-days`, `work-meghaduta`, `work-montaigne-essais`, `work-sei-shonagon-pillow-book`) — registered by alias at TAN-237 |
| Ledger rows completed (`docs/tone-coverage.csv`) | 209 / 209 `done` |
| Combination matrix integrated (`tones/_combination-rules.md`) | 60/90 flagged pairs |
| Independent review | All lanes reviewed and resolved |

### Records per silo

| Tone | dossier.md | claims | sources | primary-works |
|---|---|---|---|---|
| comedic | yes | 10 | 14 | 4 |
| compassionate | yes | 12 | 24 | 5 |
| cynical | yes | 10 | 20 | 7 |
| deadpan | yes | 9 | 19 | 6 |
| defiant | yes | 11 | 18 | 8 |
| detached | yes | 10 | 19 | 6 |
| elegiac | yes | 12 | 19 | 9 |
| grim | yes | 13 | 22 | 7 |
| inspirational | yes | 11 | 19 | 5 |
| intimate | yes | 11 | 27 | 7 |
| irreverent | yes | 12 | 26 | 6 |
| lyrical | yes | 15 | 19 | 6 |
| nostalgic | yes | 10 | 24 | 4 |
| philosophical | yes | 12 | 21 | 7 |
| reflective | yes | 11 | 19 | 9 |
| reverent | yes | 14 | 17 | 4 |
| urgent | yes | 10 | 18 | 7 |
| warm | yes | 10 | 20 | 6 |
| whimsical | yes | 12 | 13 | 4 |
| **Total (19 silos)** | **19** | **215** | **378** | **117** |

Per-silo detail rows were captured at the same 21:23:02 +05:30 timestamp by
counting `references/tone-evidence/<tone>/{claims,sources,primary-works}/*.json`
and the presence of `dossier.md`. All 710 JSON records parse and carry a usable
`id` (0 of 710 lacking).

No completion, review, or approval is claimed by these counts; automated
validation is evidence, not acceptance.
