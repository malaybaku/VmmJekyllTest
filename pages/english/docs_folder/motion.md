---
layout: page
title: Motion
permalink: /en/docs/motion
lang_prefix: /en/
---

[Japanese](../../docs/motion)

# Motion

`Motion` tab can adjust character's proportion and motion related parameters.

[![Motion Tab](./images/about_settings/img01_018_motion_tab.png)](./images/about_settings/img01_018_motion_tab.png){: data-lightbox="img01_018"}

## Face

Upper part is almost the same as `Streaming` tab in control panel.

Additional check `Auto blink during face tracking` is on by default, and when it is turned off, you can control eye open and close by image processing.

From v0.9.6 `Enable forward / backward motion` check is available. Enabling this check maybe cause your avatar motion unstable, so please test if you plan streaming use.

The item `Default Fun Blend Shape [%]` specifies the default fun expression rate.

As the value increases the character will become always smile, but some character's facial expression will be unnatural when combined to blink or other face motions. In those cases, decrease the value.

The `Eyebrow (Open to Customize)` is very advanced section and normally you do not need modify them. However if you have original VRM and want to move the eyebrow, or in case the eyebrow motion is too big or too small. 

* This section requires the knowledge about `BlendShape` to control VRM facial expression. If you do not know well, please refer to [Virtual Cast Wiki](https://virtualcast.jp/wiki/doku.php?id=%E3%83%A2%E3%83%87%E3%83%AB%E4%BD%9C%E6%88%90:%E3%83%96%E3%83%AC%E3%83%B3%E3%83%89%E3%82%B7%E3%82%A7%E3%82%A4%E3%83%97%E8%A8%AD%E5%AE%9A) and see latter section's image. You will see the name like `mouth_a` or `mouth_b`. This is BlendShape. And you can specify the name of BlendShape to move eyebrow, by sliding each shape in Unity Editor.


## Arm

Setup how to move the arm.

If you turn off `Enable Typing / Mouse Motion`, the the avatar stop to react to typing, mouse pointer move, or gamepad input. If you want to set the avatar always simply standing, turn off this checkbox.

`Waist width [cm]`and `Strength to keep upper arm to body [%]` are the parameters to keep the elbow close to body(, which is subtle but critical for the cute motion).

Please see the following example of default value, close elbow strongly, and open.

[![Arm Side Default](./images/about_settings/img01_020_arm_side_default.png)](./images/about_settings/img01_020_arm_side_default.png){: data-lightbox="img01_020"}

[![Arm Side Close](./images/about_settings/img01_030_arm_side_close.png)](./images/about_settings/img01_030_arm_side_close.png){: data-lightbox="img01_030"}

[![Arm Side Open](./images/about_settings/img01_040_arm_side_open.png)](./images/about_settings/img01_040_arm_side_open.png){: data-lightbox="img01_040"}

`Show Pointer Support` toggles whether the circle shaped mouse emphasize indication should be visible or not.

`Presentation-like motion scale [%]` has effect during `Presentation-like hand` check is on.

The value should be small when the character is enough small compared to the whole monitor size to avoid the right arm always stretched, or vise versa.

`Arm position radius min [cm]` helps to avoid arm going into the body, when large value is set. However too large value makes the arm always stretched.

## Hand

Parameters about hand or finger length and typing motion.

Check those values when the typing motion is done far from the keyboard, or the hand is too float above the keyboard.

**Hint:** After setup natural motion, set large value to `(Press key) Hand height adjust [cm]`, which make comical big typing motion.

[![Large Typing Motion](./images/about_settings/img01_045_large_type_motion.png)](./images/about_settings/img01_045_large_type_motion.png){: data-lightbox="img01_045"}


### Wait motion

Wait motion is breathing like motion.

It might be helpful for some characters to show as if (s)he is floating, with large `Scale [%]` and short `Period [sec]`.
