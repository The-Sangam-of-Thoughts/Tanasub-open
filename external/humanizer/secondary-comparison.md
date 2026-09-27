# Secondary Source Comparison: conorbronsdon/avoid-ai-writing

- **Source:** `conorbronsdon/avoid-ai-writing`
- **Stats:** MIT licensed, ~4.4k stars.
- **Content:** 36 patterns, 109-word replacement table, 5 voice profiles.

## Analysis
This source offers a large volume of specific word replacements (109 words). While the 36 patterns and 5 voice profiles are interesting, the heavy reliance on a replacement table conflicts with our core principle: *Treat vocabulary as awareness signals. Never convert word examples into unconditional bans. Preserve precise terms, quotations, dialect, cultural language, technical vocabulary, and intentional voice.*

The primary source (`blader/humanizer`) categorizes structural and rhetorical behaviors (e.g., "significance inflation", "staging instead of stating") rather than just listing words to swap. The secondary source does not add independently supported structural guidance that is absent from the primary source; its main addition is volume of vocabulary.

## Recommendation
**Do not vendor.** The reliance on a static replacement table poses a high risk of false positives and stripping intentional voice or precise terminology. The structural insights it does have are already better articulated by `blader/humanizer` and our existing Layer 2 system.
