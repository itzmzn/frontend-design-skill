---
name: games
description: Design guidance for 2D and casual games, including game states, HUDs, controls, feedback loops, and overlays.
---

# 2D & Casual Games

Game UI exists to support the loop: understand the goal, act, receive feedback, recover, and continue. Visual personality matters, but it must not obscure play.

## Use this reference for

Arcade and casual games, puzzles, card/board adaptations, platformers, simple racing or action games, educational games, score challenges, and browser-based 2D experiences.

## State architecture

Define explicit states such as loading, title, tutorial, playing, paused, round complete, game over, and results. Transitions between them should be deterministic. Input intended for gameplay must not leak through menus or overlays.

A title screen needs a clear primary action and access to essential settings. Pause should freeze or safely suspend the loop. Results should explain score, progress, rewards, and the next action without forcing the player to hunt for replay or continue.

## HUD discipline

Keep the playfield dominant. Show only information needed during the current moment: score, health/lives, timer, objective, lap/progress, or inventory when relevant. Place persistent HUD elements near edges and protect the center of action.

Use large, glanceable values and stable positions. Do not wrap every value in a separate floating card. Mobile controls need generous targets and should avoid covering important gameplay zones.

## Feedback loop

Every meaningful action should produce immediate feedback through movement, sound, particles, scale, shake, color, or score change—but use intensity proportionally. Reserve stronger effects for rare or important events so routine actions do not exhaust the visual language.

Animation timing should support responsiveness. Input feedback should feel immediate; transitions can be more expressive. Provide reduced-motion alternatives where the surrounding platform expects them.

## Visual system

Typography can be more expressive than in productivity software, but score and timer values must remain readable at a glance. Build a limited palette that distinguishes player, hazards, rewards, and neutral scenery. Use iconography consistently and accompany unfamiliar icons with labels or onboarding.

## Asset direction

When generating backgrounds, characters, props, or textures, define a consistent art direction first: camera angle, line style, lighting, palette, level of detail, and sprite proportions. Assets from different visual languages quickly make a game feel incoherent.

## Avoid

Do not block the playfield with instruction panels, mix several unrelated art styles, use long unskippable transitions, hide pause/restart controls, or rely on tiny desktop-sized targets on touch screens. Do not add fake HUD telemetry that has no gameplay purpose.
