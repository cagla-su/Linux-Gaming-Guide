# Minecraft
Minecraft is a **native Linux** sandbox game that works using **OpenGL**.
## Get Started
First of all, I definitely suggest that you use [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) because it is **open source** and it provides more options than the official Minecraft launcher.
### Install Prism Launcher
You can install Prism Launcher following [these steps according to your distribution](https://prismlauncher.org/download/?from=button).
### Install Java
Prism Launcher automatically installs Java for you.
### Install Minecraft
- When you first launch the launcher, simply continue until the **memory allocation** step.
- Then, make sure to change `Maximum memory allocation` value. There is a rumor that if you allocate half your RAM, you are going to get good performance. However, this is wrong because:
  - When you play Minecraft, the game, or Java, tries to free up allocated memory that is no longer used by objects to avoid memory issues. This is called **garbage collection**.
    - However, you **should not** allocate **too much or too little** RAM, because:
      - If you allocate **too much** RAM, Java will wait longer between garbage collection cycles and each cycle will take longer to complete, that's why you are going to get bigger lag spikes.
      - If you allocate **too little** RAM, Java will perform garbage collection too often and this will cause big lag spikes again.
    - When Minecraft uses between `50-75%` of allocated RAM, it is the ideal value for smaller lag spikes. I suggest that you experiment different values yourself to find your ideal value. You can check RAM usage by pressing `F3` during the gameplay.
- After completing quick setup, add your Microsoft account in the launcher.
- **Next** : `Add Instance` **-** `Version` **-** `Select the version you desire and scroll down` **-** `Select "Fabric" as the mod loader` **-** `OK`
## Optimization
- `Settings` **-** `Minecraft` **-** `Tweaks` **-** `Enable Feral GameMode` **&** `Use discrete GPU (only if you have hybrid graphics setup)`
- `Settings` **-** `Environment Variables` **-** `Add` **-** `mesa_glthread=true`
<img width="731" height="96" alt="image" src="https://github.com/user-attachments/assets/3cd34257-d1cf-4509-8967-d8499e61318a" />

- If you are using NVIDIA, you should use the `__GL_THREADED_OPTIMIZATIONS=1` environment variable instead.
- You are ready to play Minecraft now. However, the performance of the game can still be increased through performance mods and optimized in-game settings.
## Sodium Method - Recommended For Version 1.16.3 and Later
- `Right click Minecraft instance` **-** `Edit` **-** `Mods` **-** `Download mods`
- **Suggested Performance Mods and Dependencies**
  - `Almanac`
  - `Alternate Current`
  - `AsyncParticles`
  - `BadOptimizations`
  - `Better Biome Reblend`
  - `Cloth Config`
  - `Clumps`
  - `Concurrent Chunk Management Engine`
  - `Dynamic FPS`
  - `EntityCulling`
  - `Fabric API`
  - `Fabric Language Kotlin`
  - `Fast Item Frames`
  - `FastQuit`
  - `FerriteCore`
  - `Forge Config API Port`
  - `Fzzy Config`
  - `ImmediatelyFast`
  - `Krypton`
  - `Ksyxis`
  - `Let Me Despawn`
  - `Lithum`
  - `Model Gap Fix`
  - `No Telemetry`
  - `Noisium`
  - `OptiGUI`
  - `PacketFixer`
  - `Particle Core`
  - `Puzzles Lib`
  - `Reese's Sodium Options`
  - `Remove Reloading Screen`
  - `Sodium`
  - `Sodium Extra`
### Optifine Features Without Optifine
In Optifine, there are some nice features that do not aim to increase performance such as **zooming, being able to use shaders, dynamic lighting and connected textures**. You can get the same features without Optifine through the mods below:
- **Zooming Feature -** `Zoomify`
- **Shaders Feature -** `Iris`
- **Dynamic Lighting Feature -** `LambDynamicLights`
- **Connected Textures Feature -** `Continuity`
### Sodium - In Game Optimized Settings
- **If you are going to use Zoomify :** `Options` **-** `Controls` **-** `Key Binds` **-** `Change key bind of "Save Hotbar Activator" to something else` **-** `Done`
- `Options` **-** `Resource Packs` **-** `Move "Default Connected Textures" and "Glass Pane Culling Fix" to the right section` **-** `Done`
- `Options` **-** `Video Settings`
  - **General**
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 5 chunks
    - `VSync` **:** OFF
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
  - **Quality**
    - `Graphics` **:** Fast
    - `Clouds` **:** OFF
    - `Weather` **:** Fast
    - `Leaves` **:** Fast
    - `Particles` **:** Decreased
    - `Biome Blend` **:** 1 block(s)
    - `Entity Distance` **:** 50%
    - `Entity Shadows` **:** OFF
    - `Distortion Effects` **:** 60%
    - `FOV Effects` **:** 60%
    - `Mipmap Levels` **:** 1x
## Optifine Method - Recommended For Version 1.16.2 and Earlier
- If you want to use Optifine, I suggest that you use **the official Minecraft launcher** instead because it is going to be hard and meaningless to use Optifine through Prism Launcher.
- Simply, download [Optifine](https://optifine.net/downloads) for the Minecraft version you would like to play and click `Install` after running the **.jar** file you downloaded.
### Optifine - In-Game Optimized Settings
- `Options`
  - **Video Settings**
    `Graphics` **:** Fast
    - `Smooth Lighting` **:** ON
    - `Smooth Lighting Level` **:** 50%
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 5 chunks
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
    - `Entity Shadows` **:** OFF
    - **Quality...**
      - `Mipmap Levels` **:** 1
      - `Emissive Textures` **:** OFF
      - `Custom Fonts` **:** OFF
      - `Connected Textures` **:** Fast
      - `Custom Sky` **:** OFF
      - `Custom Entity Models` **:** OFF
      - `Random Entities` **:** OFF
      - `Custom Colors` **:** OFF
      - `Natural Textures` **:** OFF
      - `Custom Items` **:** OFF
      - `Custom GUIs` **:** OFF
      - `Distortion Effects` **:** 60%
      - `FOV Effects` **:** 60%
    - **Details...**
      - `Clouds` **:** OFF
      - `Trees` **:** Fast
      - `Fog` **:** OFF
      - `View Bobbing` **:** OFF
      - `Vignette` **:** Fast
      - `Rain & Snow` **:** Fast
      - `Stars` **:** Subjective
      - `Swamp Colors` **:** OFF
      - `Alternate Blocks` **:** OFF
      - `Entity Distance` **:** 50%
      - `Biome Blend` **:** 3x3
    - **Performance...**
      - `Render Regions` **:** OFF
      - `Smart Animations` **:** ON
      - `Smooth FPS` **:** ON
      - `Fast Render` **:** ON
      - `Fast Math` **:** ON
      - `Smooth World` **:** ON
    - **Animations...**
      - `Textures Animated` **:** OFF
      - `Particles` **:** Decreased
    - **Other...**
      - `Telemetry` **:** OFF
# Conclusion
This guide was about Minecraft installation and optimization on Linux. I hope the guide has been useful. Thank you for reading, happy gaming! 🐧
