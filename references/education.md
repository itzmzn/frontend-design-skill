---
name: education
description: Design guidance for educational tools, interactive simulations, conceptual visualizers, guided learning, and assessment interfaces.
---

# Education & Interactive Learning

Educational interfaces should make relationships visible. Interaction must reinforce the concept being taught rather than becoming a game layer disconnected from learning.

## Use this reference for

Science process simulations, mathematics and probability visualizers, geometry explorers, hardware assembly guides, guided laboratories, rubric-based assessment, and other interactive teaching tools.

## Learning architecture

A strong simulation often uses two coordinated zones: a large stage for the model or diagram and a smaller control/concept area for parameters, playback, explanation, and current values. On narrow screens, stack these zones while keeping the active concept close to the controls that affect it.

Break complex ideas into stages. Reveal new variables only when the learner has enough context to understand them. A sequence such as resting state → changed condition → observed outcome is easier to reason about than exposing every parameter at once.

## Interaction and feedback

Controls need labels, units, meaningful ranges, and immediate visual consequences. Sliders should have useful ticks or numeric readouts; play/pause/step/reset controls need obvious state; drag-and-drop assembly should show valid targets and clear success or correction feedback.

Connect cause and effect visually. Use arrows, flow, highlighted pathways, changing curves, particle motion, or before/after states only when they explain the underlying process. Keep legends close to the diagram and avoid making learners decode arbitrary colors.

Assessment views should show criteria, level descriptions, evidence, score calculation, and feedback in a way that a learner or teacher can audit. Automated scoring should not appear more certain than the rubric allows.

## Typography and color

Favor highly readable type and strong hierarchy. Educational diagrams can use a restrained palette with consistent semantic colors for variables, pathways, or states. Never rely on color alone; pair it with labels, patterns, shape, or position.

## Visual assets

Generated diagrams or illustrations should isolate the concept, use uncluttered backgrounds, and leave space for labels. Prefer scientifically coherent visual metaphors over decorative “science” imagery. If accuracy matters, verify the depicted relationship before using the asset as instruction.

## Avoid

Do not overwhelm beginners with all controls at once, animate without explanatory purpose, use unlabeled sliders, hide reset/replay actions, or turn a learning surface into a dense dashboard. Avoid feedback that says only “wrong”; show what changed or what concept should be reconsidered.

## Quality check

A learner should be able to identify the current stage, understand what each control changes, observe the result, recover from mistakes, replay the concept, and use the interface without depending on color or precise pointer control.
