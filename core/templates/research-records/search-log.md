# Research Search Log — {{search_id}}

**Template status:** {{status}}  
**Execution date:** {{date}}

Use this Markdown worksheet to prepare one JSON record governed by `schemas/v1/search-log.schema.json`. The JSON record is authoritative for validation; retain this worksheet as reproducible research evidence. Record an explicit empty array or a plain-language negative result instead of omitting a required field.

## Schema field map

| Record field | Authoritative schema path | Required | Recording rule |
|---|---|---:|---|
| Search ID | `id` | yes | Stable lowercase `search-...` ID; corresponds to `{{search_id}}`. |
| Axis IDs | `axis_ids[]` | yes | One or more canonical `axis-...` IDs; include `{{axis_id}}` when this is a single-axis search. |
| Search stream | `search_stream` | yes | Exact value from `controlled-vocabularies.json#search_streams`. |
| Database or site | `database_or_site` | yes | Name the searched system, collection, catalogue, archive, or site. |
| Query | `query` | yes | Preserve the exact executed search string, including filters. |
| Executed at | `executed_at` | yes | RFC 3339 timestamp, not merely the displayed execution date. |
| Operator | `operator` | yes | Identifiable researcher or agent. |
| Languages | `languages[]` | yes | At least one BCP 47-style tag. |
| Regions | `regions[]` | yes | Explicit regions searched; an empty array means none. |
| Inclusion criteria | `inclusion_criteria[]` | yes | At least one criterion fixed before result selection. |
| Exclusion criteria | `exclusion_criteria[]` | yes | At least one criterion fixed before result selection. |
| Results reviewed | `results_reviewed` | yes | Non-negative count of results actually screened. |
| Included source IDs | `included_source_ids[]` | yes | Canonical `src-...` IDs created or selected from this search. |
| Excluded results | `excluded_results[]` | yes | For each item, record `citation_or_locator` and `reason`. |
| Dead ends | `dead_ends[]` | yes | Failed query variants, absent corpora, and unproductive routes. |
| Access constraints | `access_constraints[]` | yes | Paywalls, unavailable editions, licensing, preview limits, or access failures. |
| Notes | `notes` | yes | Context that does not belong in another field. |

## Search design

- Canonical axis IDs:
- Search stream:
- Research question or discovery purpose:
- Database, catalogue, archive, community record, or site:
- Exact query and filters:
- Execution timestamp and operator:
- Languages searched:
- Regions and traditions searched:
- Inclusion criteria:
- Exclusion criteria:

## Coverage checks

- Indian-language, regional, oral, and culturally specific search terms used:
- Translation-studies terms, original-language terms, and transliteration variants used:
- Contrary or revisionist terms used:
- Professional-criticism and audience-reception searches kept in separate streams:
- Screen or adaptation search relevance and boundary:

If no Indian or regional evidence, direct equivalent, translation evidence, or contrary view is found, preserve the unsuccessful queries and nearest relevant traditions here. Do not infer absence from a single English-language search and do not force equivalence.

## Results and decisions

- Results reviewed count:
- Included source IDs and inclusion reasons:
- Excluded citations or locators and item-specific reasons:
- Dead ends and query variants:
- Access constraints and attempted alternatives:
- Follow-up searches required:

## Provenance and verification

- Search interface or endpoint used:
- Collection/version and visible date coverage:
- Result-order or pagination notes:
- Saved evidence path, export path, or screenshot reference:
- Reproduction notes:

Do not record a source as directly verified merely because it appeared in search results. Create and directly verify its source record separately.

