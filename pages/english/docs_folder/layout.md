---
layout: page
title: Layout
permalink: /en/docs/layout
lang_prefix: /en/
---

[Japanese](../../docs/layout)

# Layout

In `Layout` tab you can access to the parameters to adjust surrounding device layout like camera, keyboard, gamepad, etc.

[![Layout Tab](./images/about_settings/img01_050_layout_tab.png)](./images/about_settings/img01_050_layout_tab.png){: data-lightbox="img01_050"}

## Camera

Almost same as `Camera` menu in control panel `Streaming` tab.

In this panel you can also adjust FOV (Field of View).

## Device Layout

Same as `Streaming` tab in control panel.

Available from v0.9.5.

## Keyboard / MIDI

You can change the size and height of the keyboard and mouse pad, along to your character's scale.

This panel also supports the selection of typing effect, as control panel `Streaming` tab.

From v0.9.6 MIDI controller setting is also available here.

VMagicMirror uses MIDI input to change avatar face expression.

If you usually use DAW software or other MIDI-controller-required software, then turn off `Use MIDI Cotnroler for VMagicMirror`, to ensure VMagicMirror does not occupy MIDI devices.

## Gamepad

Gamepad has the feature that the character leans by  stick input. If you have a gamepad, let's check it by moving left stick with default setting!

* In `Lean by stick` list you can select what stick (or direction key) the character should be react.
* `Reverse direction to lean` support to lean reversed direction.

**NOTE:**

In default the gamepad feature is available, but if you do not use it, and the VMagicMirror performance is not good on your machine, then check off `Enable Input Capture` on the top of `Gamepad` menu.
