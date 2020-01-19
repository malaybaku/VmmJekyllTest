---
layout: page
title: Effects
permalink: /en/docs/window
lang_prefix: /en/
---

[Japanese](../../docs/window)

## Effects

note: screenshot will come here..

`Effects` tab supports light, shadow, bloom and wind settings.

Light and shadow has separated orientations, so you can set the light orientation simply for the avatar's looking, while adjust shadow orientation to show it on the back of the avatar.

Also you can adjust the depth offset and orientation of the shadow to , so that your avatar looks near or far to the screen.

Default setting : 

[![Default Depth Shadow](./images/about_settings/img01_070_shadow_depth_default.png)](./images/about_settings/img01_070_shadow_depth_default.png){: data-lightbox="img01_070"}

Example to show distance between screen and the character : 

[![Default Depth Shadow](./images/about_settings/img01_080_shadow_depth_look_far.png)](./images/about_settings/img01_080_shadow_depth_look_far.png){: data-lightbox="img01_080"}

**NOTE:** Please be aware that some VRM character uses `Unlit` type shader, to which the light setting has no effect.

For the wind settings:

* Please setup `VRMSpringBone` beforehand, to enable wind-based motion.
* Wind feature moves all `VRMSpringBone` components, so "only hair (not skirt)" like setting is not supported.
