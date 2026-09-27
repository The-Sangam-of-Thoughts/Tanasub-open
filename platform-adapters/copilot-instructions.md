# GitHub Copilot repository-instructions adapter

## Install

Copy the instruction block below into `.github/copilot-instructions.md` at the root of the repository where Copilot will work. GitHub documents this as the repository-wide instruction path in [Adding repository custom instructions](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/add-custom-instructions/add-repository-instructions).

```markdown
For writing tasks, first read `SKILL.md` and follow its file router. Load exactly one suitable Layer 0 file. Add Layer 1 only for narrative, persuasion, hooks, rhythm, or headlines; add Layer 2 for the voice pass; run Layer 3 for final QA. Select one genre or subgenre file only when the requested form needs it. Load one file from `tones/` only when the brief names an emotional attitude (for example philosophical, comedic, elegiac). Tone colors the voice; it never overrides the genre's emotional engine. Use `tones/_index.md` to choose. Open deeper references only to resolve a specific need. Do not load the whole repository. Minimize context with no hard token cap or loss of detail needed for correctness. Never present automated checks as human review or platform acceptance.
```
