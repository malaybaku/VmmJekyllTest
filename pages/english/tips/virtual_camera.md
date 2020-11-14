---
layout: page
title: Use Virtual Camera
permalink: /en/tips/virtual_camera
lang_prefix: /en/
---

[Japanese](../../tips/virtual_camera)

# Tips: Use Virtual Camera

Virtual Camera is the feature added in v0.9.9, to use VMagicMirror for web camera supported applications like online meeting.

This feature easily connect VMagicMirror to online meeting systems, etc.

#### When I should use virtual camera?
{: .doc-sec2 }

This feature is no more recommended.

[OBS Studio](https://obsproject.com/download) has introduced virtual camera by standard, from version 26.0.

If you want to use VMagicMirror with virtual camera, please consider installing `OBS Studio`.

You can see [Tips: Use VMagicMirror for Streaming](./streaming) to check the basic setup.

Also this feature will be removed in v1.6.0.


#### Setup for First Time Use
{: .doc-sec2 }

If it is first time to use VMagicMirror virtual camera output, please install virtual camera by following steps.

In `Streaming` tab `Virtual Camera Output` menu, click `*How to setup`.

**NOTE:** When you are using v1.5.0, open Setting Window `Window` tab instead of `Streaming` tab.

{% include docimg.html file="/images/tips/virtual_camera_first_setup.png" %}

Then you will see the instruction dialog, so click `Open Folder` and double-click `Install.bat` in the opened folder.

{% include docimg.html file="/images/tips/virtual_camera_run_bat.png" %}

After the installation, you will see the dialog to notify `DllRegisterServer` operation was successful.

{% include docimg.html file="/images/tips/virtual_camera_success_dialog.png" %}

Close this dialog, and also close the instruction dialog to complete setup.


#### Use Virtual Camera in Application
{: .doc-sec2 }


In `Streaming` tab `Virtual Camera Output`, turn on `Enable Camera Output`.

Then open the target application, and select `Unity Video Capture` as web camera.

Following image is an example in Zoom.

{% include docimg.html file="/images/tips/virtual_camera_camera_select_example.png" %}

If `Unity Video Capture` does not appear in the list, quit and restart the target app.

If the camera still does not appear, try to restart VMagicMirror, Windows. If these does not solve your situation, check if the virtual camera output works in other software.

**NOTE:** Virtual Camera is unavailable in some of the web-camera-supported applications.

If you could select the camera but there is no image, then confirm the image size is set to `640` x `480` in `Virtual Camera Output` menu. 

Also, if the target app has option to set camera resolution, specify the size to `640` x `480`.

When the image is stretched, click `Resize` button in `Virtual Camera Output` menu to adjust VMagicMirror window size to correct output.


#### Limitation about Resolution

The virtual camera in VMagicMirror has fixed resolution of `640` x `480`.

When you set other resolution, the target application might fails to receive the image. In this case, please reset the resolution to `640` x ` 480`.
