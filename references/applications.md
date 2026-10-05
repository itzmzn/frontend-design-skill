---
name: applications
description: Design guidance for SaaS products, dashboards, admin panels, operational tools, analytics, and other data-rich applications.
---

# Applications & Dashboards

Application interfaces should make repeated work fast, understandable, and trustworthy. Their visual identity can be distinctive, but task clarity, state visibility, and information density come first.

## Use this reference for

SaaS products, admin portals, analytics, finance and operations tools, project systems, CRM-style interfaces, hardware control panels, internal tools, and other products built around persistent navigation, structured data, and repeated workflows.

## Architecture

Use a stable shell: a compact top bar, a sidebar or clear primary navigation when the information architecture requires it, and a main workspace that uses the available desktop width. Keep global navigation visually quieter than the current task.

Tables should behave like tools rather than decorative cards. Keep column alignment stable, use tabular numerals for metrics, align numbers consistently, provide clear row actions, and support horizontal overflow intentionally on smaller screens. Dense tables need readable row height, restrained dividers, and obvious sort/filter state.

Metric summaries should answer a real question. Prefer a small number of meaningful values with context, units, comparison periods, and trend meaning. Do not manufacture “innovation scores,” fake health percentages, or decorative telemetry.

## Workflow and state design

A mature data view should account for populated, empty, loading, error, filtered, and permission-restricted states where relevant. Skeletons should approximate the final geometry so content does not jump dramatically when loaded.

Search and filters must visibly affect the data. Date ranges, segmented filters, and status selectors should have unambiguous active states. Destructive actions need confirmation proportional to their impact; reversible actions should favor undo where practical.

For feature explanations, connect the user's goal to a visible product mechanism and then to the outcome. Pricing pages should describe who each plan is for, the billing cadence, concrete limits, and meaningful differences instead of rows of vague checkmarks.

## Visual system

Use typography optimized for scanning. A clear sans-serif can handle navigation and dense interface text; reserve monospace or tabular figures for timestamps, identifiers, financial values, and changing telemetry. Keep semantic colors consistent: success/normal, warning, and error states must also include labels or symbols so color is not the only signal.

Cards are useful for independent modules, not as the default wrapper for every number and paragraph. Prefer structured grids, grouped fields, dividers, and whitespace over repeated elevated rectangles.

Hardware-inspired or skeuomorphic treatments can work for controls that benefit from physical metaphors, but they should remain legible and functional rather than becoming ornamental dashboards.

## Imagery

Most application screens need little generated imagery. Use portraits only when people are genuinely part of the workflow, and use textures or product renders only when the domain benefits from them. Keep decorative media subordinate to data and controls.

## Avoid

Do not add fake system logs, pinned telemetry tickers, invented worker IDs, decorative latency values, nested card sandwiches, or metrics with no product meaning. Do not hide core actions behind hover-only affordances, and do not reduce a desktop application to a narrow centered panel surrounded by empty space.

## Quality check

Confirm that navigation location is obvious, important numbers align and include units, filters work, tables remain usable at smaller widths, all relevant states exist, destructive actions are safe, keyboard focus is visible, and the workspace prioritizes the user's current task.
