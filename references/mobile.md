---
name: mobile
description: Design guidance for touch-first mobile web applications, compact workflows, bottom navigation, sheets, trackers, and mobile interaction patterns.
---

# Mobile & Touch-First Applications

Mobile interfaces should optimize reachability, continuity, and task focus. Design for fingers, interrupted attention, small viewports, software keyboards, safe areas, and one-handed use rather than shrinking a desktop layout.

## Ergonomic foundation

Keep common targets around 44px or larger and provide spacing that prevents accidental taps. Place frequent primary actions in comfortable thumb zones when the product permits it. Respect device safe areas and browser chrome.

Do not make critical actions depend on hover. Inputs must remain visible when the software keyboard opens, and fixed elements should not cover fields, validation messages, or system gestures.

## Bottom navigation

Use a bottom tab bar for a small set of persistent top-level destinations, usually three to five. Each tab should combine a familiar icon with a short label unless the icon is universally obvious in context. Active state must be visible without relying on color alone.

Do not use bottom tabs for transient actions or dozens of destinations. Secondary destinations belong in contextual menus, profile/settings, or deeper navigation.

## Top app bar

Keep the mobile header compact. It can contain a back action, concise title, and one or two high-value contextual actions. Avoid duplicating navigation already present in the bottom bar.

Long titles should truncate gracefully rather than pushing controls off screen. Search can expand into a dedicated state when the task requires more space.

## Bottom sheets and action drawers

Use bottom sheets for contextual choices, short forms, filters, confirmation details, and actions that benefit from staying visually connected to the current screen. Give sheets a clear title, dismiss path, sensible maximum height, and scroll behavior when content exceeds the viewport.

Do not stack several sheets or dialogs. Keyboard interaction, focus trapping, and back-button behavior should be predictable.

## Trackers and list layouts

Daily trackers and summary screens should show the current state first, then supporting trends. Large summary numbers need units and time context. Interactive list rows should have one obvious primary action and clear disclosure when they open details.

Use cards selectively. A flat list with dividers is often more space-efficient than a stack of rounded containers.

## Sticky actions

A sticky bottom CTA can work for checkout, booking, form submission, or other decisive actions. Reserve enough content padding so the bar never covers the final fields or content. Keep secondary actions visually subordinate.

## Motion and feedback

Use short transitions to preserve spatial continuity between tabs, sheets, and detail views. Provide immediate pressed and loading feedback. Avoid elaborate page choreography that slows repeated mobile tasks.

## Avoid

Avoid tiny icon-only controls, excessive fixed bars, desktop tables squeezed onto a phone, nested horizontal scrollers, modal-on-modal flows, and decorative cards that consume vertical space without adding structure.
