# Minecraft
Minecraft is a **Linux-native** game that works using **OpenGL**.
## Get Started
First of all, I definitely suggest you use [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) because it is **open-source** and provides more options than the original launcher.
### Install Prism Launcher
You can install Prism Launcher following [these steps according to your distribution](https://prismlauncher.org/download/linux/).
### Install Java
Prism Launcher now allows you to install Java inside the app instead of installing it manually. To do so, follow the steps below:
- `Settings - Java - Management - Download - Adoptium - Install the latest builds of all 3 Java versions`
  - After installing Java, if Minecraft does not launch, change your Minecraft instance's Java version to the relevant one.
    - **For 1.20.5 and above:** Java 21
    - **From 1.18 to 1.20.4:** Java 17
    - **For 1.17 and 1.17.1:** Java 16 - but in the app, there is no Java 16 in Adoptium, so you might want to install another Java build if you want to play the specific version.
    - **For 1.16.5 and below:** Java 8
### Install Minecraft
- When you first launch the launcher, it will ask you what language you would like to use. After that question, you are going to see a page about Java.
- Make sure to change `Maximum memory allocation`. Some people claim you should allocate half your RAM but this is not good for **some cases**. If you have at least 32 GB RAM and if you do not perform memory-intensive tasks, you can allocate half your RAM. However:
  - If you have RAM between **4-16 GB**, I suggest you allocate **2048 MiB** if you are not going to install heavy mods or shaders. However, you should allocate at least **3072 MiB** RAM if you are going to use Optifine without mods.
- After completing quick setup, add your Microsoft account to connect to your account in the launcher.
- Now we can finally install Minecraft. Click `Add Instance` button on the top left and continue:
  - In `Version` section, select the version you would like to play and scroll down a bit. You should see a big "**No mod loader is selected.**" warning. There is a `Mod loader` section next to the warning. Select `Fabric` from there and click `OK`.
## Optimization
- Click `Settings`, go to `Minecraft` section and click `Tweaks`. Enable `Enable Feral GameMode` (you need to install gamemode package first) and `Use discrete GPU` (only if you have two GPUs).
- Next, from `Settings` menu, go to `Environment Variables` and click `Add`.
  - Type `mesa_glthread` in **Name** and `true` in **Value** sections.
    - If you are using NVIDIA, you should type `__GL_THREADED_OPTIMIZATIONS` in **Name** and `1` in **Value** sections instead.
- Generally these steps are enough to play a better Minecraft. However, we can still increase performance with mods.
## Sodium Method - Recommended For Version 1.16.3 And Later
- First, right click your Minecraft instance and click `Edit`.
- In the opened page, click `Mods` from the left side bar and click `Download mods` from the right side bar.
- **Suggested Performance Mods and Dependencies**
  - `Cloth Config`
  - `Concurrent Chunk Management Engine`
  - `Debugify`
  - `Dynamic FPS`
  - `EntityCulling`
  - `Fabric API`
  - `Fabric Language Kotlin`
  - `FastQuit`
  - `FerriteCore`
  - `ImmediatelyFast`
  - `Lithum`
  - `ModernFix`
  - `More Culling`
  - `No Chat Reports`
  - `No Telemetry`
  - `OptiGUI`
  - `Reese's Sodium Options`
  - `Remove Reloading Screen`
  - `Sodium`
  - `Sodium Extra`
- There are lots of other performance boosting mods. However, the mods above can **significantly** increase performance while other mods do not at all. That is why installing the mods above is generally enough.
### Optifine Features Without Optifine
In Optifine, there are some cool features that are not about increasing performance such as **zooming, being able to use shaders, dynamic lighting and connected textures**. We can get the same features without Optifine through the mods below:
- **Zooming Feature -** `Zoomify`
- **Shaders Feature -** `Iris`
- **Dynamic Lighting Feature -** `LambDynamicLights`
- **Connected Textures Feature -** `Continuity`
### Sodium - In Game Optimized Settings
- **If you are going to use Zoomify**:
  - Click `Options`, go to `Controls` - `Key Binds` and scroll down until you see a red key bind.
  - `Save Hotbar Activator` has C button as a key bind, change it to something else and click `Done`
- Go to `Options` and `Resource Packs`. Now move `Default Connected Textures` and `Glass Pane Culling Fix` from the left section to the right section and click `Done`.
- Go back to `Options` and `Video Settings`. These are the optimized settings for performance:
  - **General**
    - `Render Distance`: 6 chunks
    - `Max Shadow Distance`: Disabled
    - `Simulation Distance`: 5 chunks
    - `VSync`: OFF
    - `Max Framerate`: Same number as your monitor's refresh rate (for 60 hz screens, change the value to 70)
  - **Quality**
    - `Graphics`: Fast
    - `Clouds`: OFF
    - `Weather`: Fast
    - `Leaves`: Fast
    - `Particles`: Decreased
    - `Biome Blend`: 1 block(s)
    - `Entity Distance`: 50%
    - `Entity Shadows`: OFF
    - `Distortion Effects`: 60%
    - `FOV Effects`: 60%
    - `Mipmap Levels`: 1x
## Optifine Method - Recommended For Version 1.16.2 And Earlier
- For Optifine, you should install **Forge** mod loader instead of **Fabric**.
- First of all, install [Optifine](https://optifine.net/downloads) for the Minecraft version you would like to play.
- Next, right click your Minecraft instance and click `Edit`.
- In the opened page, click `Mods` from the left side bar and drag **Optifine file** into the page.
### Optifine - In Game Optimized Settings
- Go to options
  - **Video Settings**
    `Graphics`: Fast
    - `Smooth Lighting`: ON
    - `Smooth Lighting Level`: 50%
    - `Render Distance`: 6 chunks
    - `Simulation Distance`: 5 chunks
    - `Max Framerate`: Same number as your monitor's refresh rate (for 60 hz screens, change the value to 70)
    - `Entity Shadows`: OFF
    - **Quality...**
      - `Mipmap Levels`: 1
      - `Emissive Textures`: OFF
      - `Custom Fonts`: OFF
      - `Connected Textures`: Fast
      - `Custom Sky`: OFF
      - `Custom Entity Models`: OFF
      - `Random Entities`: OFF
      - `Custom Colors`: OFF
      - `Natural Textures`: OFF
      - `Custom Items`: OFF
      - `Custom GUIs`: OFF
      - `Distortion Effects`: 60%
      - `FOV Effects`: 60%
    - **Details...**
      - `Clouds`: OFF
      - `Trees`: Fast
      - `Fog`: OFF
      - `View Bobbing`: OFF
      - `Vignette`: Fast
      - `Rain & Snow`: Fast
      - `Stars`: Subjective
      - `Swamp Colors`: OFF
      - `Alternate Blocks`: OFF
      - `Entity Distance`: 50%
      - `Biome Blend`: 3x3
    - **Performance...**
      - `Render Regions`: OFF
      - `Smart Animations`: ON
      - `Smooth FPS`: ON
      - `Fast Render`: ON
      - `Fast Math`: ON
      - `Smooth World`: ON
    - **Animations...**
      - `Redstone Animated`: OFF
      - `Rain Splash`: OFF
      - `Lava Animated`: OFF
      - `Dripping Water/Lava`: OFF
      - `Textures Animated`: OFF
      - `Particles`: Decreased
    - **Other...**
      - `Telemetry`: OFF
## Conclusion
This guide was about Minecraft installation and optimization! I hope the guide has been useful. Thank you for reading, have a nice day! 🐧
