# Troubleshooting and FAQ

## The controls bar does not appear

- Check that the viewport type is **Cinematic Viewport**. CineViewPlus never activates on a Default viewport.
- Check that the **CineVP** button in the viewport toolbar is on.
- Check that the plugin is enabled in **Edit > Plugins**, and that you restarted the editor.

If the bar still does not appear, the same controls may be in the main viewport toolbar. Please [report it](../SUPPORT.md) with your engine version.

## A keyboard shortcut does nothing

- Click the image first, so the viewport has keyboard focus.
- Check for a conflict in the [Keyboard Shortcuts page](08-keyboard-shortcuts.md#change-a-shortcut).
- If your operating system uses Alt+Shift, for example to switch keyboard layout on Windows, [rebind the shortcut](08-keyboard-shortcuts.md#change-a-shortcut).

## Left click does not select objects

The Pan tool, the Zoom tool or the eyedropper is probably on. Turn it off in the controls bar.

## Alt + left drag does not orbit the camera

This is intended: in an active Cinematic Viewport, it pans the image. Turn CineViewPlus off to orbit with Alt + left drag.

## The image does not update

Check that **Pause** is off.

## The viewport feels slow

- Turn off the **eyedropper** when you do not need it.
- Lower the resolution, or use **Downrez**.
- Lower the **Scalability** level.
- Turn off **Pixel-Exact Zoom** in [Settings](07-settings.md).

## The zoomed image looks blurry

Check that Fixed Res and **Pixel-Exact Zoom** are both on. If **Downrez** is below 1:1, the image is upscaled, so its pixels no longer match the scene's.

## The color values differ from Nuke

The eyedropper reads [display-referred values](06-rulers-and-eyedropper.md#what-the-values-mean), after tone mapping. Scene-linear values are not available.

## Why can't Downrez go below 1:4?

Unreal limits the preview screen percentage to a minimum of 25%.

## Does it affect Movie Render Queue?

No. Movie Render Queue is independent of CineViewPlus.

## Does it affect Play In Editor?

CineViewPlus stands down while Play In Editor runs in the viewport, then reactivates when it ends. The zoom resets at that point.

## Can each viewport have its own resolution?

Not at the moment. All Cinematic Viewports share the same W x H.

## Is the plugin included in my packaged game?

No. CineViewPlus is an editor-only plugin.

## Known limitations

- The resolution is shared across Cinematic Viewports.
- Downrez stops at 25%.
- Color values are display-referred.
- Activation can take up to half a second after switching viewport type.
