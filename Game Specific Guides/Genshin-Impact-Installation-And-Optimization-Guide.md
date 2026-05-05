# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#before-starting)
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#get-started)
  - [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#optimization-tips)
    - [Launcher Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#launcher-settings)
    - [In-Game Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#in-game-settings)
    - [Other In-Game Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#other-in-game-settings)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#conclusion)
# Before Starting
> [!NOTE]
> - The software we will be using in order to play Genshin Impact on Linux is [AAGL](https://github.com/an-anime-team/an-anime-game-launcher).
> - If you are ready, let's begin!
# Get Started
- First of all, **launch AAGL** and complete installation steps.
> [!NOTE]
> - Once you see the `Launch` button, you are **officially ready to play** Genshin Impact.
> - However, the performance **will not be the same** as Windows. So you might want to keep reading the guide for optimization tips.
# Optimization Tips
## Launcher Settings
> [!NOTE]
> - Launcher settings **may not increase performance** if you have a **strong system**.
> - However if you have a **low-end (weak) system**, slight changes can **enhance** your gaming experience.
- In the launcher, click `Settings` icon next to `Launch` button.
  - Scroll down and go to `Launcher behavior`.
    - If you have **at least 16 GB RAM**, you can keep it as `Hide`.
    - If you have **12 GB or less RAM**, change it to `Close`.
  - Now go to `Components` and make sure that the `Selected version` is a `Spritz-Wine-TKG` build. If not, you can install it from the same page.
  - Scroll down and go to `Gplasync`.
    - Install **the latest** version and change your `DXVK version` to the one you installed.
- Go back from `Components` and go to `Enhancements` that is on top.
  - Under `Wine` section, change `Synchronization` to `None` and go to `Environment`.
  - In `Environment`, make sure your environment part looks like this:
<img width="612" height="573" alt="image" src="https://github.com/user-attachments/assets/6a70e344-e977-49c5-b146-5bd6f42cd7d8" />

> [!NOTE]
> - If you are **not** using Wayland, **do not include** the `env -u DISPLAY %command%` part.
>   - If you are using Wayland, go back and enable `Borderless window` under `Wine` section **if Wayland's window decoration discomforts you**.

## In-Game Settings
- `Settings` **-** `Graphics`

---
### Optimal Visual Quality: For Strong Systems & Gaming Computers
- **Display Mode** `:` `Your native resolution Fullscreen`
- **FPS** `:` `60`
- **V-Sync** `:` `Off`
- **Render Resolution** `:` `1.0`
- **Shadow Quality** `:` `Medium`
- **Visual Effects** `:` `High`
- **SFX Quality** `:` `High`
- **Environment Detail** `:` `Medium`
- **Anti-Aliasing** `:` `FSR2`
- **Volumetric Fog** `:` `On`
- **Reflections** `:` `On`
- **Motion Blur** `:` `Extreme`
- **Bloom** `:` `On`
- **Crowd Density** `:` `High`
- **Co-Op Teammate Effects** `:` `On`
- **Subsurface Scattering** `:` `High`
- **Anisotropic Filtering** `:` `1x`

---
### Balance of Quality and Performance: For Mid-Range Computers
- **Display Mode** `:` `Your native resolution Fullscreen`
- **FPS** `:` `60`
- **V-Sync** `:` `Off`
- **Render Resolution** `:` `0.8`
- **Shadow Quality** `:` `Medium`
- **Visual Effects** `:` `Low`
- **SFX Quality** `:` `Medium`
- **Environment Detail** `:` `Low`
- **Anti-Aliasing** `:` `FSR2`
- **Volumetric Fog** `:` `On`
- **Reflections** `:` `On`
- **Motion Blur** `:` `Medium`
- **Bloom** `:` `On`
- **Crowd Density** `:` `High`
- **Co-Op Teammate Effects** `:` `On`
- **Subsurface Scattering** `:` `Off`
- **Anisotropic Filtering** `:` `1x`

---
### Balance of Quality and Performance: For Low-End Computers with Dedicated GPU
- **Display Mode** `:` `1280x720 Fullscreen`
- **FPS** `:` `60`
- **V-Sync** `:` `Off`
- **Render Resolution** `:` `0.6`
- **Shadow Quality** `:` `Low`
- **Visual Effects** `:` `Lowest`
- **SFX Quality** `:` `Medium`
- **Environment Detail** `:` `Lowest`
- **Anti-Aliasing** `:` `FSR2`
- **Volumetric Fog** `:` `Off`
- **Reflections** `:` `Off`
- **Motion Blur** `:` `Low`
- **Bloom** `:` `On`
- **Crowd Density** `:` `Low`
- **Co-Op Teammate Effects** `:` `On`
- **Subsurface Scattering** `:` `Off`
- **Anisotropic Filtering** `:` `1x`

---
### Balance of Quality and Performance: For Low-End Computers without Dedicated GPU
- **Display Mode** `:` `1280x720 Fullscreen (reduce to 960x540 Windowed if you want to reach near 60 FPS)`
- **FPS** `:` `60 - reduce to 30 if you selected 720p`
- **V-Sync** `:` `Off`
- **Render Resolution** `:` `0.6`
- **Shadow Quality** `:` `Lowest`
- **Visual Effects** `:` `Lowest`
- **SFX Quality** `:` `Low`
- **Environment Detail** `:` `Lowest`
- **Anti-Aliasing** `:` `FSR2`
- **Volumetric Fog** `:` `Off`
- **Reflections** `:` `Off`
- **Motion Blur** `:` `Off`
- **Bloom** `:` `On`
- **Crowd Density** `:` `Low`
- **Co-Op Teammate Effects** `:` `Partially Off`
- **Subsurface Scattering** `:` `Off`
- **Anisotropic Filtering** `:` `1x`

---
### Highest Performance: For Toasters and Low Graphics Enjoyers
- **Display Mode** `:` `1280x720 Fullscreen (reduce to 960x540 Windowed if your system struggles)`
- Click `Compatibility Mode` at the bottom and **do not change anything else**.
## Other In-Game Settings
- `Settings` **-** `Audio` **-** `Dynamic Range` **-** `Limited`
- `Settings` **-** `Other` **-** `Mini-Map Settings` **-** `Fixed`
## Tips for Actual Toaster Users
- For the best performance possible, especially if you **only** have an **integrated GPU**, you should use **CachyOS XFCE with compositor disabled**.
  - In CachyOS, launch `SchedExt GUI Manager` and select `scx_lavd` with `Gaming` scheduler profile. Make sure to **apply changes**.
# Conclusion
This guide was about Genshin Impact installation and optimization! I hope the guide has been useful. Thank you for reading, happy gaming!
