---
title: Settings
nav_order: 8
---

# Settings

Open **Edit > Editor Preferences > Plugins > CineViewPlus**.

![Editor Preferences page for CineViewPlus](images/settings.png)

| Setting | Default | Description |
|---|---|---|
| **Enable CineViewPlus** | On | Turns CineViewPlus off in every viewport. Each viewport also has its own CineVP button |
| **Fixed Resolution** | On | Render at exactly Width x Height |
| **Width** | 1920 | Fixed render width, 1 to 16384 |
| **Height** | 1080 | Fixed render height, 1 to 16384 |
| **Downrez (Screen %)** | 100 | Scene render percentage, 25 to 200 |
| **Pixel-Exact Zoom** | On | Hard square pixels above 100% zoom |
| **Show Rulers** | Off | Rulers along the top and left of the image |

**Fixed Resolution**, **Width**, **Height**, **Downrez** and **Show Rulers** are under **New Viewer Defaults**. They are the starting values for a Cinematic Viewport used for the first time. After that, each viewport keeps its own values, set from its controls bar.

Settings are saved per user and per project, in the project's `Saved/Config` folder. Changes made from a controls bar are saved automatically, for that viewport only. Each viewport keeps its own on/off state, Fixed Resolution, W x H, Downrez and rulers, also after a restart.

## Not saved

These reset for each session: zoom, pan, Pause, the eyedropper, and the Pan and Zoom tools.
