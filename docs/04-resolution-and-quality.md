# Resolution and quality

## Fixed Res

**Fixed Res** (Alt+Shift+X) controls how the image is rendered.

- **On:** the viewport renders at exactly W x H at any panel size, with the Downrez percentage applied.
- **Off:** standard Unreal behavior. The render follows the panel size and your editor screen percentage is restored. Zoom, pan and object selection keep working.

Turning Fixed Res back on shows the image centered at a pixel-true 100%.

Fixed Res is not always the slower option, nor always the faster one. A large panel can contain more pixels than your W x H, and a small panel fewer.

While CineViewPlus is active with Fixed Res on, the screen percentage comes from Downrez, so the editor's automatic screen percentage cannot silently lower the image quality. Your own value returns when you turn Fixed Res or CineViewPlus off.

## Setting the resolution

Type a value in **W** or **H** and press Enter, or drag the field and release.

- The viewport updates when you press Enter or release the drag, not during the drag.
- Dragging stops at 8192. Values up to 16384 must be typed.
- The resolution is shared by all Cinematic Viewports.

## Resolution readout

The readout shows the render size, then the size the image covers on your screen:

```
1920x1080 → 1440x810
```

Hover it for details: render size, displayed size, window size, zoom and screen percentage. With Downrez active, the tooltip also shows the internal scene render size.

## Downrez

Downrez renders the scene at a fraction of the fixed resolution and upscales it into the same image size, for faster previews.

| Preset | Screen percentage | Scene size for 1920 x 1080 |
|---|---|---|
| 1:1 | 100% | 1920 x 1080 |
| 1:2 | 50% | 960 x 540 |
| 1:3 | 33% | 634 x 356 |
| 1:4 | 25% | 480 x 270 |

The **Custom** field in the menu accepts any value from 25 to 100. Unreal does not allow a preview screen percentage below 25%. Downrez only applies while Fixed Res is on.

![Downrez dropdown open](images/downrez-menu.png)

## Scalability

This menu sets all engine scalability groups to **Low**, **Medium**, **High**, **Epic** or **Cinematic**, like **Quick Settings > Engine Scalability**. The button shows **Custom** when the groups are at different levels.

> **Note:** this changes and saves your editor's scalability settings. It affects the whole editor, not only this viewport.

## Pause

**Pause** (Alt+Shift+Space) stops continuous rendering and freezes the image, including while Sequencer is open. The image still refreshes on demand. Your Realtime setting is left untouched and applies again when you unpause or turn CineViewPlus off.

## Pixel-Exact Zoom

With Fixed Res on and the zoom above 100%, each render pixel is displayed as a hard square rather than a smoothed image, so you can inspect aliasing and edges.

This copies each frame into an extra texture, only while the image is shown above 100%.

| Resolution | Extra video memory |
|---|---|
| 1080p | about 8 MB |
| 4K | about 33 MB |
| 8K | about 133 MB |

You can turn it off in [Settings](07-settings.md).

![Same edge at 733%, Pixel-Exact Zoom on and off](images/pixel-exact-compare.png)
