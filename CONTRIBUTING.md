# Contributing to Tanasub Open

Thank you for helping improve Tanasub Open. This repository is a public, self-contained writing system. Contributions should improve its craft guidance, evidence, schemas, templates, documentation, or platform compatibility without introducing a dependency on a hosted or proprietary service.

## Before you begin

- Read [`SKILL.md`](SKILL.md) to understand the router and progressive-disclosure model.
- Check existing issues and pull requests before starting overlapping work.
- Open an issue first when a change alters repository-wide structure, taxonomy, schemas, licensing, or established behavior.
- Report vulnerabilities privately through the repository's **Security** tab. Do not publish vulnerability details in an issue or discussion.

## What belongs here

Suitable contributions include:

- corrections or clearer writing guidance;
- evidence-backed improvements to genres, subgenres, tones, and methodology;
- new or corrected sources, claims, indexes, and research records;
- schema, template, documentation, and platform-adapter improvements;
- fixes for broken links, formatting, terminology, and routing.

Tanasub Open is intentionally content-only. Do not add executable programs, binaries, symlinks, submodules, secrets, generated caches, private traces, proprietary prompts, or implementation details from a proprietary system. The integrity workflow permits Markdown, JSON, CSV, text, the repository licence files, `CODEOWNERS`, and its own workflow file. A contribution requiring another file type needs maintainer agreement before implementation.

Preserve `universal-writing-guide` wherever it is used as the stable skill or platform compatibility identifier.

## Create your contribution

1. Fork the repository on GitHub.
2. Clone your fork and register this repository as `upstream`:

   ```text
   git clone https://github.com/YOUR-USERNAME/Tanasub-open.git
   cd Tanasub-open
   git remote add upstream https://github.com/The-Sangam-of-Thoughts/Tanasub-open.git
   ```

3. Start from the latest `master` and create a focused branch:

   ```text
   git fetch upstream
   git switch master
   git merge --ff-only upstream/master
   git switch -c docs/short-description
   ```

4. Make the smallest coherent change. Avoid unrelated cleanup or broad rewrites.
5. Commit with a clear message and a sign-off:

   ```text
   git add path/to/changed-file.md
   git commit -s -m "Clarify thriller pacing guidance"
   git push -u origin docs/short-description
   ```

6. Open a pull request against `The-Sangam-of-Thoughts/Tanasub-open:master`.

Use a branch prefix that describes the work, such as `docs/`, `fix/`, `genre/`, `tone/`, or `evidence/`.

## Content and evidence standards

- Match the existing terminology, structure, and depth of the file being changed.
- Use exactly one applicable genre or subgenre file and one tone file only when the task calls for them.
- Support substantive factual or craft claims with sources appropriate to their scope.
- Keep quotations brief, accurate, and traceable to a precise source location.
- Distinguish quotation, paraphrase, synthesis, and researcher inference in structured evidence.
- Do not present generated text, automated checks, or author review as independent human review.
- Do not copy protected expression, private data, or material whose licence is incompatible with this repository.
- Update affected indexes, cross-references, coverage records, or attribution files in the same pull request.

Read [`core/methodology/source-policy.md`](core/methodology/source-policy.md), [`core/methodology/research-workflow.md`](core/methodology/research-workflow.md), and [`docs/licensing-scope.md`](docs/licensing-scope.md) when a contribution adds or changes evidence.

## Validate the change

Before opening the pull request:

```text
git diff --check upstream/master...HEAD
git status --short
```

Review every changed file and confirm that only intended files are present. JSON must parse successfully, links and repository paths must resolve, and examples must match the guidance they demonstrate.

Every pull request runs the required **Validate content-only repository** check. It rejects executable file modes, symlinks, submodules, and unexpected file types. Maintainers will not merge a pull request while required checks fail or review discussions remain unresolved.

## Pull request expectations

The pull request description should explain:

- the problem or gap;
- the resulting behavior or guidance;
- the files and scope affected;
- the evidence or sources used, when applicable;
- the validation performed;
- any known limitation or follow-up work.

Keep each pull request focused enough to review as one decision. Maintainers may ask for revisions, narrower claims, stronger attribution, or a smaller scope. Accepted pull requests are squash-merged, and merged branches are deleted automatically.

## Licensing

By contributing, you agree that your contribution may be distributed under the licence applicable to the files you change. Most repository content is MIT-licensed; some adapted material is under CC BY-SA 4.0 or retains an upstream licence. Review [`LICENSE`](LICENSE) and [`LICENSES/README.md`](LICENSES/README.md) before changing licensed or vendored material.

Include attribution and licence information with any permitted third-party material. If the licensing status is unclear, open an issue and wait for a maintainer decision before adding it.

## Security and releases

Follow [`.github/SECURITY.md`](.github/SECURITY.md) for private vulnerability reports. Never place credentials, access tokens, personal data, or exploit details in commits, issues, or pull requests.

Maintainers create official releases after substantial updates using `YYYY.MM.DD.<version>`. Contributors should not create, move, or delete release tags.
