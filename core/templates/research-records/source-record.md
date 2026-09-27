# Research Source Record — {{source_id}}

**Template status:** {{status}}  
**Record date:** {{date}}

Use this worksheet to prepare one JSON record governed by `schemas/v1/source.schema.json`. The structured record is authoritative. Bibliographic discovery alone is insufficient: the schema requires direct verification.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Source ID | `id` | yes | Stable lowercase `src-...` ID; corresponds to `{{source_id}}`. |
| Title | `title` | yes | Verify the title directly against the source used. |
| Creators | `creators[]` | yes | At least one directly verified creator name. |
| Source type | `source_type` | yes | Exact controlled value. |
| Source roles | `source_roles[]` | yes | One or more exact controlled values; reception evidence stays reception-scoped. |
| Reliability tier | `reliability_tier` | yes | Integer 1–5 with rationale below; tier is an evaluation, not proof. |
| Publication | `publication.*` | yes | Map publisher/container, date precision, edition, DOI, and ISBN exactly. |
| Languages | `languages[]` | yes | At least one BCP 47-style language tag. |
| Regions | `regions[]` | yes | Cultural or geographic relevance; empty is explicit. |
| Access | `access.*` | yes | Locator, access date, and controlled access condition. |
| Verification | `verification.*` | yes | `verified_directly` must be true; record timestamp, verifier, and method. |
| Axis IDs | `axis_ids[]` | yes | One or more canonical `axis-...` IDs; include `{{axis_id}}` when applicable. |
| Claim IDs | `claim_ids[]` | yes | All consequential claims supported, qualified, or contradicted. |
| Translation | `translation.*` | yes | Translation state, original language, translator, and limitations. |
| Copyright | `copyright.*` | yes | Controlled status, repository-copy permission, and specific notes. |

## Bibliographic identity

- Verified title:
- Verified creators and roles:
- Source type:
- Source roles:
- Publisher or container:
- Publication date at the source’s supported precision:
- Edition or version:
- DOI:
- ISBN:
- Languages:
- Regions or traditions:

## Access and direct verification

- Stable locator or physical holding:
- Accessed date:
- Access condition: `open`, `licensed`, `library`, `purchased`, `limited-preview`, or `unavailable`
- Directly verified: must be true before the JSON record is accepted
- Verification timestamp:
- Verified by:
- Verification method, pages/sections checked, and identity checks:
- Evidence path for retained notes or lawful excerpt metadata:

Never claim direct verification from a citation snippet, search-result summary, secondary reference, or inaccessible record.

## Evaluation and provenance

- Reliability tier and rationale:
- Author/editor/institution expertise:
- Independence group and relationship to other sources:
- Intended axis IDs:
- Intended claim IDs:
- Search-log IDs that discovered this source:
- Limits, conflicts of interest, and uncertainty:

## Evidence extraction register

Create one row per extracted item. Keep original expression types distinct.

| Expression type | Exact location | Research note | Claim ID | Verification evidence path |
|---|---|---|---|---|
| `quotation`, `paraphrase`, `synthesis`, or `researcher-inference` |  |  |  |  |

For quotations, record exact wording only in a lawful, minimal excerpt and verify punctuation and location. For paraphrases, avoid language that could be mistaken for quotation. A synthesis combines identified evidence; a researcher inference must be plainly labelled and must not be attributed to the source.

## Counterevidence, scope, and exceptions

- Claims this source challenges or qualifies:
- Counterexamples or contrary interpretation:
- Cultural, historical, linguistic, medium, and audience scope:
- Exceptions and non-transferable contexts:
- Confidence impact:

## Indian, regional, and translation coverage

- Indian-language or regional context:
- Original-language terminology and transliteration:
- Translator identity and edition used:
- Translation-dependent conclusions:
- Translation losses, contested choices, or inaccessible originals:
- Closest relevant tradition when no direct equivalent is evidenced:

## Reception boundary

- Professional criticism findings:
- Reader or audience response findings:
- Writing-level implications:
- Excluded performance, direction, acting, editing, or music observations:

Do not merge professional criticism with audience response. Use either only for the reception claims its source role supports.

## Copyright and reuse

- Copyright status:
- Repository copy allowed:
- Permitted use and attribution:
- Excerpt or reproduction limits:
- Full-text storage check:
- Copyright uncertainty and remediation owner:

Do not store copyrighted books, screenplays, articles, or substantial excerpts unless explicit permission or applicable rights are recorded.

## Verification-event register

Record one event for each distinct operation; do not collapse discovery into direct verification.

| Event ID | Operation (`discovery`, `metadata-verification`, `text-access`, `passage-verification`, `reception-sampling`) | Exact edition/version and language | Locator checked | Date/time and operator | Result and evidence path |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

A source may support a quotation, translation observation, date, identity, or reception assertion only when the corresponding event identifies that exact locator and passes. For reception sampling also name the reviewer, publication, review date, independence group, position, and whether the assertion concerns writing-level evidence.
