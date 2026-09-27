<!-- SPDX-License-Identifier: CC-BY-SA-4.0 -->
<!-- This file contains adapted material from WikiProject AI Cleanup's field guide -->
<!-- (CC BY-SA 4.0) and research by Kobak, González-Márquez, and Horvát. -->
<!-- See LICENSES/CC-BY-SA-4.0.txt for the full licence text. -->

# Humanization guide — rationale and method

Humanization is contextual editing. It asks whether the prose fits a particular reader, writer, purpose, and setting while preserving truth. It does not assume that casual language is more human, that uncommon words are inherently better, or that any token proves who wrote a passage.

## Evidence boundary

The Fabric `humanize` and `improve_writing` patterns emphasize clarity, coherence, meaning preservation, register consistency, active construction, and iterative revision. This project uses those principles as inputs but replaces blanket preferences for short sentences or everyday words with audience-dependent questions. The pinned upstream text and MIT notice are preserved under `external/fabric-humanize/`.

WikiProject AI Cleanup's field guide documents recurring content, language, formatting, and citation patterns observed on Wikipedia. The pinned page explicitly describes its list as observational rather than prescriptive, warns that indicators also occur in human writing, and advises addressing underlying quality problems instead of merely removing surface signs. Its Wikipedia-specific observations are translated here into general editing questions. They are not detector rules.

Kobak, González-Márquez, and Horvát studied changes in word frequencies across large corpora of biomedical abstracts and inferred population-level effects associated with LLM-assisted writing. That design can support awareness of aggregate lexical shifts. It cannot establish the authorship of an individual sentence, and its biomedical scope should not be generalized to every genre.

## Revision workflow

1. Freeze the requested meaning, factual claims, cited evidence, quotations, technical terms, and accessibility needs.
2. Define reader, situation, register, and speaker.
3. Mark each paragraph's job in the document.
4. Diagnose specific problems: abstraction, repetition, unsupported significance, vague attribution, templated progression, register mismatch, monotony, or loss of stance.
5. Revise only the failing feature. Avoid a global synonym pass.
6. Read aloud and inspect transitions between paragraphs.
7. Compare the revision with the meaning lock.
8. Run the applicable Layer 3 gate.

## What good revision preserves

- A technical term that is the community's normal precise term.
- A formal connective when the genre and logical relation call for it.
- Repetition used for emphasis, rhythm, instruction, or accessibility.
- Symmetry that reflects the material rather than a template.
- Uncertainty that belongs to the evidence.
- The writer's dialect and cultural voice.

## What deserves another look

- Claims of significance that replace an explanation of what happened.
- Praise without criteria or evidence.
- Vague groups such as “experts” or “many believe.”
- Paragraphs that announce a topic, summarize it generically, then repeat it.
- The same sentence frame or transition used several times in succession.
- Lists made mechanically parallel even when the ideas differ in weight.
- Flourishes that make a concrete subject less specific.
- Citations that do not support the nearby claim.

## Sources and licenses

- Daniel Miessler et al., Fabric `humanize` and `improve_writing`, pinned revision `b682dad740f24e85ce9a48d23babc6780dd476ac`, MIT: https://github.com/danielmiessler/Fabric/tree/b682dad740f24e85ce9a48d23babc6780dd476ac/data/patterns
- WikiProject AI Cleanup contributors, “Signs of AI writing,” revision `1374467046`, CC BY-SA 4.0: https://en.wikipedia.org/w/index.php?oldid=1374467046&title=Wikipedia%3ASigns_of_AI_writing
- Dmitry Kobak, Rita González-Márquez, Emőke-Ágnes Horvát, and Jan Lause, “Delving into LLM-assisted writing in biomedical publications through excess vocabulary,” arXiv:2406.07016v5, CC BY-SA 4.0: https://arxiv.org/abs/2406.07016v5

The repository named `alexander-stewart/chatgpt-words` in the conversion plan was unavailable during implementation. No data or license from it is represented here.

## Adaptation notice

The project-authored reflection questions in this file, `layer2-humanize.md`, `structural-tells-catalog.md`, and `word-awareness-index.md` adapt the categories and cautions of the pinned WikiProject page. The wording, organization, cross-format application, and reflection protocol were changed on 2026-09-14; Wikipedia contributors do not endorse this project. Those four adapted files are distributed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) for the adapted material. The Kobak et al. paper is cited and summarized from version 5; no dataset or substantial paper text is reproduced.
