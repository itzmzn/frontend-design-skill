# Contributing to Frontend Design Skill

Thank you for your interest in improving **Frontend Design Skill**.
Contributions that make the guidance clearer, more accurate, more
useful, or more adaptable across frontend projects are welcome.

## What You Can Contribute

Useful contributions include:

-   Improving existing design guidance.
-   Correcting unclear, outdated, contradictory, or technically
    inaccurate instructions.
-   Expanding an existing reference with meaningful patterns, edge
    cases, accessibility considerations, or responsive behavior.
-   Improving the consistency and readability of the documentation.
-   Fixing broken internal references, formatting issues, or examples.
-   Proposing a new design-domain reference when it covers a genuinely
    distinct area that is not already represented.

Avoid adding content solely to increase the size of the repository. New
guidance should solve a real design or implementation problem.

## Repository Structure

The core skill is intentionally simple:

``` text
SKILL.md
references/
├── applications.md
├── commerce.md
├── editorial.md
├── education.md
├── games.md
├── marketing.md
├── mobile.md
├── portfolio.md
├── science.md
└── spatial.md
```

`SKILL.md` contains the shared frontend design principles, workflow,
quality expectations, and reference-routing guidance.

Files under `references/` contain specialized guidance for particular
interface or experience categories.

Keep this separation intact unless a structural change provides a clear
improvement to the project.

## Before Making Changes

Before editing:

1.  Read `SKILL.md` to understand the project's overall design
    philosophy.
2.  Read the relevant reference file in full.
3.  Check whether the proposed guidance already exists elsewhere.
4.  Prefer improving an existing section over introducing duplicate
    instructions.
5.  Preserve useful existing behavior unless there is a clear reason to
    change it.

## Writing Guidelines

Contributions should be written as practical guidance for a capable AI
coding agent.

Use clear, direct, vendor-neutral language. Explain the design reasoning
behind important decisions where useful rather than relying on arbitrary
rules.

Guidance should encourage intentional design, strong hierarchy,
appropriate typography, responsive composition, accessibility, coherent
interaction, and production-quality implementation.

Avoid turning stylistic preferences into universal rules. A pattern that
is inappropriate in one product may be appropriate in another. Prefer
context, purpose, and deliberate decision-making over rigid aesthetic
bans.

## Keep the Skill Vendor-Neutral

The core repository should not depend on a particular AI model, hosted
editor, or proprietary AI development environment.

Do not introduce unnecessary instructions that assume the user is
working specifically with one AI provider or coding agent.

References to normal frontend technologies, frameworks, libraries,
browsers, standards, and development tools are acceptable when they are
relevant to the guidance.

Never commit API keys, access tokens, credentials, private identifiers,
secrets, or other sensitive information.

## Editing `SKILL.md`

Changes to `SKILL.md` should apply broadly across frontend design tasks.

Do not move highly specialized domain guidance into the core file when
it belongs in a reference.

When adding or renaming a reference, update the routing guidance in
`SKILL.md` so an agent can determine when the reference should be
consulted.

The core file should remain useful without requiring every reference to
be loaded.

## Editing References

Each reference should have a clear and distinct purpose.

When modifying a reference:

-   Keep guidance relevant to its domain.
-   Avoid duplicating large sections of `SKILL.md`.
-   Preserve consistency with the project's shared design philosophy.
-   Include domain-specific layout, visual, interaction, responsive, and
    accessibility guidance where relevant.
-   Prefer durable design principles over temporary trends.
-   Keep examples purposeful and technically plausible.

A reference does not need to use exactly the same headings as every
other reference. Its structure should suit the subject while remaining
easy to navigate.

## Adding a New Reference

Before proposing a new reference, make sure the subject cannot
reasonably be covered by an existing file.

A new reference should:

-   Represent a distinct frontend design domain.
-   Contain enough specialized guidance to justify a separate file.
-   Use a concise, descriptive lowercase filename.
-   Avoid unnecessary overlap with existing references.
-   Be added to the appropriate routing section in `SKILL.md`.

Please explain the reason for the new reference in the pull request.

## Technical Accuracy

When a contribution includes implementation guidance or code:

-   Prefer current web standards and stable techniques.
-   Avoid deprecated APIs and packages.
-   Preserve compatibility with the context being discussed.
-   Clearly distinguish requirements from recommendations.
-   Do not present framework-specific behavior as a universal
    web-platform requirement.
-   Keep examples syntactically valid and internally consistent.

If a recommendation is likely to become outdated quickly, consider
whether a durable principle would be more useful.

## Accessibility

Accessibility should be treated as part of design quality rather than an
optional cleanup step.

Contributions should avoid introducing guidance that harms keyboard
navigation, semantic structure, focus visibility, readable contrast,
touch accessibility, motion preferences, or assistive-technology
support.

Accessibility improvements should still respect the purpose and visual
direction of the interface.

## Markdown Style

Keep Markdown easy to read both as source and when rendered on GitHub.

-   Use descriptive headings.
-   Keep heading levels logically nested.
-   Use fenced code blocks with language identifiers when applicable.
-   Use backticks for filenames, paths, properties, and short code
    references.
-   Keep lists concise and meaningful.
-   Avoid unnecessary HTML when Markdown is sufficient.
-   Use relative repository paths for internal references.
-   Avoid excessive decorative formatting.

## Submitting a Contribution

1.  Fork the repository.
2.  Create a focused branch for your change.
3.  Make and review your changes.
4.  Verify Markdown formatting, internal paths, and examples.
5.  Commit with a clear description of the change.
6.  Open a pull request explaining what changed and why.

Keep pull requests focused. Unrelated changes are easier to review when
submitted separately.

## Pull Request Checklist

Before submitting, confirm that:

-   [ ] The contribution has a clear purpose.
-   [ ] Existing relevant files were reviewed first.
-   [ ] The original intent of edited guidance is preserved unless the
    change deliberately improves it.
-   [ ] New content does not unnecessarily duplicate existing guidance.
-   [ ] The wording is vendor-neutral.
-   [ ] Technical claims and code examples have been checked.
-   [ ] Internal filenames and reference paths are correct.
-   [ ] No credentials, secrets, or private information are included.
-   [ ] Markdown renders correctly.
-   [ ] `SKILL.md` routing has been updated if references were added,
    removed, or renamed.

## Issues and Suggestions

For substantial changes, new reference categories, or changes to the
overall design philosophy, opening an issue before a large pull request
is encouraged. This makes it easier to discuss scope and avoid
duplicated work.

Small corrections, documentation improvements, and straightforward fixes
can be submitted directly as pull requests.

## Code of Conduct

Be constructive and respectful when discussing contributions. Critique
ideas and implementations rather than contributors, and keep discussions
focused on improving the project.
