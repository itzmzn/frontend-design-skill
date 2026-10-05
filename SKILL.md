---
name: frontend-design
description: >
  A general-purpose frontend design skill for creating distinctive, usable,
  accessible, responsive, production-ready web interfaces across product,
  marketing, commerce, editorial, educational, scientific, mobile, game, and
  spatial experiences.
---

# Frontend Design

Use this skill to turn product requirements into interfaces that feel deliberately designed rather than assembled from fashionable defaults. Build working UI, preserve existing behavior when editing a project, and make visual decisions that suit the product's domain, audience, content, and interaction model.

## Decision order

When constraints compete, resolve them in this order:

1. **Functionality.** Controls must perform their stated action. Do not ship dead buttons, fake controls, placeholder interactions, or invented data behavior.
2. **Legibility and accessibility.** Maintain readable contrast, visible keyboard focus, semantic structure, usable touch targets, and reduced-motion support.
3. **Layout integrity.** Prevent clipping, accidental overflow, unstable wrapping, and broken responsive states. Design desktop surfaces as desktop surfaces rather than centering a narrow mobile card in unused space.
4. **Hierarchy and spatial logic.** Use consistent spacing, proportion, alignment, density, and nested-radius relationships. Outer containers should not feel tighter than their contents.
5. **Aesthetic direction.** Choose typography, color, imagery, shape, and motion because they fit the product—not because they are common in generated interfaces.

## Design principles

### Design for the domain

Establish a visual language before styling individual components. A scientific console, luxury shop, museum archive, casual game, and SaaS workspace should not share the same component treatment merely because they use the same framework.

Give each viewport one dominant visual anchor. Build supporting hierarchy around it instead of allowing several banners, CTAs, cards, and metrics to compete at equal weight. Prefer a few complete sections over many shallow sections.

### Avoid generic generated-UI habits

Do not default to purple gradients, glass panels, excessive rounded cards, glowing borders, floating metric tiles, decorative sparkle icons, or a grid of identical cards. These treatments are valid only when the product context genuinely calls for them.

Static metadata such as dates, categories, read times, statuses, and labels usually works better as quiet text separated by punctuation or spacing. Reserve pills, segmented controls, tabs, and chips for interactions or cases where the enclosure carries real semantic value.

Avoid fake technical decoration: invented latency readouts, fabricated system states, mock compiler text, arbitrary scores, pseudo-version numbers, and code-comment prefixes used only to make an interface look technical. Real operational interfaces may display real telemetry; decorative fiction should not masquerade as product data.

Use whitespace and dividers before adding another container. Avoid cards nested inside cards and keep elevation shallow. Reuse a governing motif—such as a radius scale, divider treatment, offset, or typographic rhythm—without cloning the same component everywhere.

### Typography

Use no more than two primary font families, with an optional monospace face for code or numerical data. Choose display typography for character and body typography for sustained readability. Do not choose a popular UI font merely because it is convenient when the surface needs a distinctive identity.

Keep body copy at a comfortable measure, normally around 65–75 characters for long reading. Use tabular numerals for changing metrics, prices, timers, and aligned numeric columns. Limit simultaneous weights and sizes so hierarchy remains obvious.

### Color and contrast

Build a restrained palette around neutrals, one primary accent, and semantic colors where needed. Color should communicate state or hierarchy, not compensate for weak composition. Never rely on hue alone for success, warning, error, or selection states; pair color with text, shape, iconography, or another cue.

Meet accessible contrast for essential text and controls. Treat subtle borders and muted text as supporting elements, not as an excuse to make information unreadable.

### Interaction and motion

Every interactive element needs clear hover, focus, pressed, selected, disabled, loading, and error behavior when those states apply. Keep common UI feedback fast and predictable. Use motion to explain change, preserve spatial continuity, or provide feedback—not to decorate every element.

Respect `prefers-reduced-motion`. Avoid large entrance sequences that delay access to content, repeated looping animation near reading areas, and motion that changes layout unexpectedly.

### Responsive behavior

Design responsiveness as a change in composition, not a simple shrink operation. Preserve task priority as space decreases: collapse secondary navigation, reflow multi-column layouts, simplify supporting metadata, and keep primary actions reachable.

Touch-first surfaces should generally provide targets around 44px or larger. Sticky controls must not cover content or stack into competing fixed layers. Test narrow phones, wider phones, tablets, common laptop widths, and large desktop canvases when the product supports them.

### Navigation and top bars

Keep global navigation stable and easy to scan. Brand, primary destinations, and high-value actions should have clear priority. Avoid turning every navigation link into a filled capsule. If a top bar is sticky, reserve its space and ensure menus, dialogs, and other overlays layer correctly around it.

### Content and quantitative claims

Use concrete, plausible content that demonstrates the intended interface. Do not invent impressive statistics, customer counts, ratings, scientific results, or performance claims unless the task explicitly calls for mock data and it is clearly presented as such.

Social proof should be credible and proportionate. A clean testimonial or verified metric is stronger than a wall of fabricated badges.

## Imagery and generated assets

Prefer project-owned assets or generated assets over fragile hot-linked image URLs. Match image aspect ratio, lighting, composition, and subject matter to the exact slot in the interface. Product imagery should preserve product clarity; editorial imagery should support the narrative; decorative imagery should not compete with the primary task.

When generating several assets, define the complete set first so visual direction remains consistent. Give each asset a clear role, aspect ratio, subject, framing, and art direction. Avoid vague prompts such as “futuristic AI background.”

Always provide a graceful fallback when an image or rich visual cannot load. Do not leave broken-image icons or empty black rendering areas in finished UI.

## Implementation workflow

1. Inspect the existing project, framework, design system, assets, and behavior before editing.
2. Identify the product domain, primary user task, target viewport, content density, and visual tone.
3. Load only the relevant reference file(s) listed below.
4. Establish hierarchy, layout, typography, palette, component language, and responsive behavior before polishing details.
5. Implement real interactions and preserve existing contracts unless the user asks to change them.
6. Add complete UI states: loading, empty, populated, error, disabled, and selected states where applicable.
7. Review keyboard access, focus visibility, touch targets, contrast, semantics, and reduced-motion behavior.
8. Check multiple viewport sizes and remove accidental overflow, awkward wrapping, and redundant fixed surfaces.
9. Perform a final visual pass for alignment, spacing, typography, image treatment, consistency, and unnecessary decoration.

## Reference routing

Consult only references that materially apply to the task. Combine references when a product genuinely spans domains.

- `references/applications.md` — SaaS products, dashboards, admin tools, operational software, data-heavy interfaces.
- `references/commerce.md` — stores, catalogs, marketplaces, product detail pages, carts, and checkout.
- `references/education.md` — learning tools, simulations, guided exploration, assessment, and interactive diagrams.
- `references/editorial.md` — museums, archives, cultural institutions, long-form publishing, reports, and catalogues.
- `references/games.md` — 2D and casual games, HUDs, game states, feedback loops, and overlays.
- `references/marketing.md` — landing pages, launches, campaigns, product storytelling, conversion flows, and pricing.
- `references/mobile.md` — touch-first mobile web applications, bottom navigation, sheets, trackers, and compact workflows.
- `references/portfolio.md` — photography, creative portfolios, case studies, team/student showcases, and media-first sites.
- `references/science.md` — scientific, laboratory, space, biotech, engineering, telemetry, and analytical interfaces.
- `references/spatial.md` — 3D/WebGL experiences, spatial visualizers, product viewers, and 3D games.

## Final review

Before considering the interface complete, verify that the primary task works; content hierarchy is obvious; interactive states are real; typography and spacing are consistent; desktop space is used intentionally; mobile controls are reachable; essential text meets contrast needs; focus states are visible; motion respects user preference; no fabricated technical clutter has slipped in; imagery has a fallback; and the result looks appropriate for this product rather than like a reusable demo template.
