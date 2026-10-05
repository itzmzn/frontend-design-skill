---
name: spatial
description: Design guidance for 3D, WebGL, spatial visualization, product viewers, immersive scenes, and 3D game interfaces.
---

# Spatial & 3D Experiences

Spatial interfaces should let the scene remain primary while keeping essential controls accessible as semantic UI. Performance, camera behavior, lighting, fallback states, and input design are part of the experience—not implementation afterthoughts.

## Use this reference for

3D product viewers, geometry and molecular visualizations, architectural scenes, WebGL experiences, racing and first-person games, orbit/planetary models, and other interactive spatial canvases.

## Viewport and UI layering

Let the 3D canvas fill its intended region without accidental scrollbars or arbitrary framing. Keep headings, navigation, forms, and essential actions in semantic DOM overlays rather than baking important text into canvas pixels.

HUD elements should sit near edges, use enough contrast for the scene beneath them, and avoid blocking the focal area. Frosted or translucent backing can be useful over visually complex scenes, but use it only where readability requires it.

Provide a polished loading state and a graceful fallback when WebGL is unavailable, context is lost, or the device cannot sustain the experience. Handle context loss/restoration where the rendering stack permits it.

## Lighting and materials

For product and educational viewers, a controlled key/fill/rim arrangement can reveal form without flattening surfaces. Physically based materials should use plausible roughness, metalness, transmission, and environment lighting rather than extreme values that create blown highlights.

Atmospheric fog can establish depth in large environments when it matches the scene and does not hide navigational cues.

## Camera and input

Avoid abrupt camera jumps unless they are a deliberate game mechanic. Use damping or interpolation for orbiting, following, and guided transitions. Provide a clear reset/recenter action for inspectable objects.

High-speed experiences can use restrained FOV change, camera lean, particles, or environmental streaks as speed cues. Keep motion comfortable and provide reduced-motion or lower-effects behavior when appropriate.

Support the input methods relevant to the target device: pointer, touch gestures, keyboard, controller, or accessibility alternatives. Do not assume desktop orbit controls will translate cleanly to a phone.

## Typography and visual system

Racing and sci-fi interfaces can use angular or technical display typography for short HUD values, paired with a highly readable UI face. Product and architectural viewers usually benefit from neutral typography and restrained surfaces that let materials and geometry dominate.

## Image and environment briefs

When generating skyboxes, backplates, or static fallbacks, specify horizon placement, lighting direction, scene type, perspective, and aspect ratio so the asset integrates with the camera. Examples include a wet night city for racing, a desert highway at sunset, or a minimal automotive studio with controlled overhead lighting.

## Avoid

Avoid overexposed lighting, control panels that obscure the scene, raw black loading voids, excessive post-processing, camera motion that causes discomfort, and essential text rendered only inside the canvas.
