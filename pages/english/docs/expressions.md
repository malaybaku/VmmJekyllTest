---
layout: page
title: Docs
permalink: /en/docs/expressions
lang_prefix: /en/
---

[Japanese](../../docs/expressions)

# Word to Motion

`Word to Motion` is the function to receive word input to change the character's face expression or start built-in motion.

[![Word to Motion Tab](./images/about_settings/img01_100_word_to_motion_tab.png)](./images/about_settings/img01_100_word_to_motion_tab.png){: data-lightbox="img01_100"}

This feature sometimes make your avatar unnatural. In those case, please turn off `Enable Word to Motion` check.

`Word to Motion` consists of word items to define what word to react, and how to react to the word.

You can test how each item work by typing word, or press `Play` button at the left of each item. For example, the above picture shows the case after typing "joy".

**NOTE:** During typing those word, please be careful NOT to insert any control key (Shift, Control, Alt, etc.). Also there are cases the word is not recognized for the too slow typing.

From v0.9.1, gamepad is also supported. Turn on `Use gamepad as launcher` and press buttons in left column to start motion or face expression.

[![Word to Motion by Gamepad](./images/about_settings/img01_105_word_to_motion_by_gamepad.png)](./images/about_settings/img01_105_word_to_motion_by_gamepad.png){: data-lightbox="img01_105"}

The example above shows starting `fun` expression by `Y` button.

**NOTE:** `Use gamepad as launcher` disables gamepad based hand motion. If you prefer to use VMagicMirror for game play streaming, please turn off `Use gamepad as launcher`.


`Up` and `Down` supports re-order of items. Delete button at the right side removes selected item.

You can add and custom the word and reaction for the word by 4 steps.

* Step 1: Press `+` button to add a new item. If you custom existing item, skip it.
* Step 2: Press `Setting` button to open the setting.
* Step 3: In the custom window you can setup motion and face blend shape.
* Step 4: Press `OK` to reflect your customize.

[![Word to Motion Custom](./images/about_settings/img01_110_word_to_motion_custom_flow.png)](./images/about_settings/img01_110_word_to_motion_custom_flow.png){: data-lightbox="img01_110"}

Custom window interface is as following.

[![Word to Motion Custom Window](./images/about_settings/img01_120_word_to_motion_custom_window.png)](./images/about_settings/img01_120_word_to_motion_custom_window.png){: data-lightbox="img01_120"}

* 1: Set the word to start this item. 
* 2: Select motion type for this item. 
    * **NOTE:** In v0.9.0 only 2 built-in motions are supported, so in almost case you will select `None` option.
* 3: Facial expression setting.
    * Turn on `Enable Face Expression` check to play some face expression in this item.
    * `Duration when Body Motion is None [sec]` defines how long the character keep the face.
    * If `Keep face after motion` is on, then character face does not change after the duration.
* 4: BlendShapes. 
    * **NOTE:** In the most cases you should set only one blend shape to non-zero for the appearance.

From v0.9.6, you can also use MIDI controller for input device.

There are 3 steps to use MIDI controller to launch expressions.

https://twitter.com/baku_dreameater/status/1211990346525077504

* Select `Device Assign` to `MIDI Controller` and click edit button at the right of `Keys`.
* You will see `MIDI note assign` window, so press MIDI keys to use, to input MIDI note number for each items. `Note to Change` column is updated by your MIDI input.
* After setting click `OK` to complete setting.

After closing the window, test to press the same notes to check the mapping.

**Hint:**

When you use the expression with `Keep face after motion` option you will need reset motion.

Reset item will be like following, which has all-zero face expression with very short duration.

[![How to Reset Keep Face](./images/about_settings/img01_130_word_to_motion_reset_tips.png)](./images/about_settings/img01_130_word_to_motion_reset_tips.png){: data-lightbox="img01_130"}


## 3.6. Reset Settings to default

v0.9.2 or later version support to reset each settings, by clicking `Reset` button at the top on almost every category in setting window.

Below is an example to reset light settings to default.

[![Reset Setting 1](./images/about_settings/img01_140_reset_setting_before.png)](./images/about_settings/img01_140_reset_setting_before.png){: data-lightbox="img01_140"}

[![Reset Setting 2](./images/about_settings/img01_150_reset_setting_before.png)](./images/about_settings/img01_150_reset_setting_after.png){: data-lightbox="img01_150"}

