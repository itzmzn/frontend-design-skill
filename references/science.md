---
name: science
description: Design guidance for scientific, laboratory, space, biotech, engineering, telemetry, and analytical interfaces.
---

# Science, Space & Biotech

Scientific interfaces should communicate precision without pretending to be more technical than the underlying data. Units, uncertainty, provenance, state, and comparison matter more than decorative “sci-fi” styling.

## Visual tone

Use disciplined grids, restrained surfaces, fine dividers, and high-contrast data marks. Dark console themes can suit monitoring environments; light laboratory/reporting themes can suit analysis and documentation. Accent colors should map to real variables, series, thresholds, or states.

Avoid decorative pseudo-telemetry. If the system has mission time, sample identifiers, calibration state, or run status, show the real values. Otherwise do not invent them merely to create atmosphere.

## Typography and notation

Use highly legible sans-serif text for controls and explanation, with monospace/tabular numerals for measurements, coordinates, timestamps, sample IDs, and changing values. Keep decimal precision consistent within a column and always show units where interpretation depends on them.

Mathematical and scientific notation should remain semantically correct. Avoid ambiguous abbreviations and make significant figures appropriate to the data rather than visually uniform for its own sake.

## Workspace architecture

Complex analytical tools often benefit from an asymmetric workspace: a compact control column, a large primary visualization, and a secondary tray for time series, logs, comparisons, or tables. A small top utility area can hold real run state, presets, export, and calibration controls.

Keep controls grouped by the model they affect. Parameter inputs need bounds, units, and sensible step sizes. Provide reset/default behavior and make irreversible operations explicit.

## Data visualization

Radar charts can summarize a small set of comparable dimensions, but should not replace a table when exact values matter. Line charts need labeled axes, units, distinguishable series, and tooltips or crosshairs when precise inspection is important. Heatmaps need a visible legend, meaningful scale, and enough cell separation to support inspection.

Do not use rainbow color scales by habit. Choose perceptually useful sequential, diverging, or categorical scales according to the data and preserve accessibility for common color-vision differences.

## State and interaction

Status must never rely on hue alone. Pair indicators with explicit labels or symbols. Fine parameter scrubbers should support keyboard adjustment and, when precision matters, direct numeric entry. Canvas or plot inspection can use crosshairs and coordinate readouts when they serve the task.

Loading, stale-data, disconnected, out-of-range, and error states should be distinguishable. Do not display cached or simulated data as live without labeling it.

## Avoid

Avoid fake mission-control decoration, arbitrary percentages, unlabeled charts, inconsistent precision, hidden units, excessive glow, and visualizations chosen for spectacle rather than analytical value.
