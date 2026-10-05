# Frontend Design Skill

A vendor-neutral frontend design skill for AI coding agents, focused on
producing interfaces that feel intentional, context-aware, responsive,
accessible, and production-ready.

Instead of pushing every project toward the same generic visual formula,
this skill helps an agent reason about the product, audience, content,
interaction model, and design domain before making frontend decisions.

## Overview

`SKILL.md` provides the shared design philosophy, workflow, quality
standards, implementation expectations, and routing logic for the skill.

The `references/` directory contains specialized guidance for different
types of frontend experiences. An agent can consult only the references
relevant to the current task rather than loading unrelated design
guidance.

``` text
frontend-design-skill/
├── references/
│   ├── applications.md
│   ├── commerce.md
│   ├── editorial.md
│   ├── education.md
│   ├── games.md
│   ├── marketing.md
│   ├── mobile.md
│   ├── portfolio.md
│   ├── science.md
│   └── spatial.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── SKILL.md
```

## Design Philosophy

The skill is built around a simple principle:

> Design for the product in front of you, not for a generic idea of what
> a modern interface should look like.

It encourages agents to make deliberate decisions about hierarchy,
typography, spacing, composition, color, interaction, responsiveness,
accessibility, and implementation.

The guidance favors coherent systems over isolated visual tricks and
discourages repetitive AI-generated patterns when they do not serve the
product.

That includes avoiding reflexive use of generic card grids, excessive
rounded containers, arbitrary gradients, unnecessary glass effects,
decorative pills, meaningless animation, and interchangeable hero
layouts. These patterns are not prohibited; they should simply have a
reason to exist.

## References

The current reference library covers ten frontend design domains:

  -----------------------------------------------------------------------
  Reference                           Focus
  ----------------------------------- -----------------------------------
  `applications.md`                   SaaS products, dashboards, admin
                                      interfaces, productivity tools, and
                                      complex web applications

  `commerce.md`                       E-commerce, retail, marketplaces,
                                      product discovery, shopping, and
                                      transactional interfaces

  `editorial.md`                      Editorial experiences, museums,
                                      cultural institutions, archives,
                                      and content-led interfaces

  `education.md`                      Learning products, educational
                                      tools, simulations, and interactive
                                      teaching experiences

  `games.md`                          Games, playful interfaces, casual
                                      interactive experiences, and
                                      game-oriented UI

  `marketing.md`                      Landing pages, campaigns, product
                                      marketing, launches, and
                                      conversion-oriented websites

  `mobile.md`                         Mobile-first and touch-first
                                      interfaces, compact layouts, and
                                      handheld interaction patterns

  `portfolio.md`                      Creative portfolios, photography,
                                      showcases, case studies, and
                                      visually led personal sites

  `science.md`                        Scientific, space, biotechnology,
                                      research, and data-rich technical
                                      experiences

  `spatial.md`                        3D, spatial, immersive,
                                      canvas-based, and depth-oriented
                                      web experiences
  -----------------------------------------------------------------------

References can be combined when a project genuinely spans multiple
domains. For example, a mobile shopping application may benefit from
both `commerce.md` and `mobile.md`.

## How It Works

The intended workflow is straightforward:

1.  Give the agent access to `SKILL.md`.
2.  Let it understand the product, audience, content, constraints, and
    interaction requirements.
3.  Use the routing guidance in `SKILL.md` to identify relevant
    references.
4.  Consult only the references that materially apply to the task.
5.  Design and implement the interface using the shared principles plus
    domain-specific guidance.
6.  Review the result for visual quality, responsiveness, interaction
    clarity, accessibility, and implementation quality.

The references are supporting knowledge, not independent themes that
should be blindly copied. The final interface should still be shaped by
the actual product.

## Installation

There is no runtime dependency or package installation required. This
repository consists of Markdown instructions intended to be made
available to an AI coding agent.

Clone the repository:

``` bash
git clone https://github.com/itzmzn/frontend-design-skill.git
cd frontend-design-skill
```

Then configure your preferred AI coding environment to use `SKILL.md` as
the primary skill or instruction file and make the `references/`
directory available for contextual reading.

Because agent systems differ in how they discover and load skills, the
exact integration method depends on the tool you use.

## Usage

A request can remain natural and product-focused. For example:

``` text
Design and implement a responsive analytics dashboard for a logistics platform.
Prioritize fast scanning, clear operational status, useful data hierarchy, and
excellent mobile behavior.
```

For this task, the agent can use the core skill together with
`references/applications.md` and, when the interface has substantial
handheld requirements, `references/mobile.md`.

A commerce request might instead route to `references/commerce.md`,
while a campaign site could use `references/marketing.md`.

The goal is not to make users manually choose a reference for every
prompt. Routing exists so the agent can select the appropriate design
knowledge from the nature of the task.

## What This Skill Emphasizes

The guidance is designed to improve several areas where generated
frontend work often becomes repetitive or under-considered:

-   Product-appropriate visual direction rather than default styling.
-   Clear information hierarchy and composition.
-   Deliberate typography and spacing.
-   Responsive behavior designed as part of the interface rather than
    added afterward.
-   Touch and interaction patterns appropriate to the device.
-   Accessible structure and interaction.
-   Meaningful motion instead of animation for its own sake.
-   Components that belong to a coherent visual system.
-   Preservation of existing product behavior when improving an
    established interface.
-   Production-quality frontend implementation rather than static mockup
    thinking.

## What This Repository Is Not

This is not a component library, CSS framework, design system package,
UI kit, or collection of copy-and-paste page templates.

It does not prescribe one visual style for every project.

It also does not require a particular frontend framework or AI provider.
Framework-specific implementation decisions should follow the
requirements and architecture of the project being worked on.

## Principles for Extending the Skill

New guidance should earn its place in the repository.

Prefer improving an existing reference when a topic already belongs
there. A new reference should represent a genuinely distinct design
domain with enough specialized guidance to justify a separate file.

Keep the core skill broadly applicable, keep domain-specific knowledge
in references, and avoid duplicating the same guidance across multiple
files.

See `CONTRIBUTING.md` for the full contribution guidelines.

## Contributing

Contributions are welcome, including corrections, clearer design
guidance, accessibility improvements, stronger domain-specific
recommendations, and fixes for outdated or contradictory information.

Please read `CONTRIBUTING.md` before making substantial changes.

## Changelog

Release history and notable changes are documented in `CHANGELOG.md`.

## License

See `LICENSE` for the terms under which this project is distributed.
