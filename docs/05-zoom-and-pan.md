---
title: Zoom and pan
nav_order: 6
---

# Zoom and pan

Zoom and pan apply to the finished image. They do not move the camera and do not trigger any extra rendering. Safe frames, grids and other film overlays follow the image.

## Zoom

- **Scroll wheel:** zooms toward the cursor, by 10% per tick.
- **Alt+=** and **Alt+-:** zoom in or out by 25%.
- **Alt+Shift+T:** zooms to 100%.

Holding the right mouse button while scrolling keeps its usual Unreal function, changing the camera speed.

## Pan

- **Middle mouse drag**
- **Alt + left mouse drag**

> **Note:** in an active Cinematic Viewport, Alt + left drag pans the image instead of orbiting the camera.

<video src="images/pan.mp4" autoplay loop muted playsinline preload="metadata" aria-label="Middle-mouse pan sliding the whole zoomed-out image over the viewport, with the camera unchanged" style="max-width:100%"><a href="images/pan.mp4">Middle-mouse pan sliding the whole zoomed-out image over the viewport, with the camera unchanged</a></video>

## Pan and Zoom tools

These tools are for working without a middle button or a wheel, such as on a trackpad. Only one of the Pan tool, the Zoom tool and the eyedropper can be on at a time: turning one on turns the others off.

- **Pan tool** (Alt+Shift+N): left drag moves the image.
- **Zoom tool** (Alt+Shift+Z): left drag right zooms in, left drag left zooms out, around the point you pressed.

While either tool is on, left clicks do not select objects. Turn the tool off to select again.

<video src="images/zoom-tool.mp4" autoplay loop muted playsinline preload="metadata" aria-label="Zoom tool dragging right then left" style="max-width:100%"><a href="images/zoom-tool.mp4">Zoom tool dragging right then left</a></video>

## Fit

The **Fit** button, **Home** or **Alt+Shift+F** fits the whole image in the panel and recenters it.

## Zoom menu

The zoom percentage button opens a menu:

| Entry | Effect |
|---|---|
| **zoom in / zoom out** | Zooms in or out by 25%, like Alt+= and Alt+- |
| **fit** | Shows the whole image, centered |
| **fit width** | The image width fills the panel, the height may overflow |
| **fit height** | The image height fills the panel, the width may overflow |
| **900% to 11%** | Exact zoom levels, anchored on the center of the view |

Zoom percentages are **pixel-true**: at 100%, one render pixel covers one physical screen pixel, including on Retina and other high-DPI displays. A custom zoom keeps its value when you resize the panel.

![Zoom dropdown open](images/zoom-menu.png)

## Selecting and moving objects

Clicking objects, box selection and gizmos work normally at any zoom, pan and resolution.
