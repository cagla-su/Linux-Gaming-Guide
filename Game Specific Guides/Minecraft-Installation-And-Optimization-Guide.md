# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#before-starting)
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#get-started)
  - [Installing Prism Launcher](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#installing-prism-launcher)
  - [Installing Java](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#installing-java)
  - [Installing Minecraft](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#installing-minecraft)
- [Optimization](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#optimization)
  - [Optifine Method](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#optifine-method---recommended-for-version-1162-and-earlier)
    - [In-Game Optimized Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#optifine---in-game-optimized-settings)
  - [Sodium Method](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#sodium-method---recommended-for-version-1163-and-later)
    - [Mods That You Need to Use Sodium](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#mods-that-you-need-to-use-sodium)
    - [In-Game Optimized Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#sodium---in-game-optimized-settings)
  - [Essential Performance-Increasing Mods for Sodium](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#essential-performance-increasing-mods-for-sodium)
    - [Optional Performance-Increasing Mods for Sodium](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#optional-performance-increasing-mods-for-sodium)
  - [Quality of Life Mods for Sodium](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#quality-of-life-mods-for-sodium)
  - [Global Quality of Life Resource Packs](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#global-quality-of-life-resource-packs)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md#conclusion)
# Before Starting
> [!NOTE]
> - Minecraft has **two editions** which are **Java** and **Bedrock** editions.
> - Linux natively supports **Java edition**.
> - When it comes to **Bedrock**, Linux can run **Pocket Edition (Android)**. However, Linux cannot run **Bedrock Edition (PC)**.
>  - The reason why is that **Bedrock Edition (PC)** is a **UWP** app which is even **unable to run** through WINE.
>  - So, the only way to play **Bedrock Edition** is to play the **Android version**.
>  - This also means **you should purchase** the game from **Google Play Store**.
>    - If you would like to play **Pocket Edition**, you can install it from [Flathub](https://flathub.org/en/apps/io.mrarm.mcpelauncher) and start playing.
>    - For **Java Edition**, please keep reading the guide. If you are ready, let's begin!
## Get Started
> [!TIP]
> I definitely suggest that you use [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) because it is **open source** and it provides more options than the official Minecraft launcher.
### Installing Prism Launcher
You can install Prism Launcher following [these steps according to your distribution](https://prismlauncher.org/download/?from=button).
### Installing Java
> [!NOTE]
> - Prism Launcher **automatically installs Java** for you.
> - Additionally, Prism Launcher allows you to install **custom Java builds that perform better**.
> - My suggestion is using [Eclipse Temurin](https://adoptium.net). To install Eclipse Temurin, follow the next steps:
>  - `Settings` **-** `Java` **-** `General` **-** `Uncheck "Auto-download Mojang Java"` **-** `Management` **-** `Download` **-** `Adoptium` **-** `Download the latest Java version for the Minecraft version you play`
>  - If you **do not know** which Java version to install, these are the Java versions for **specific Minecraft versions:**
>    - **Minecraft Version 1.16.5 and Earlier -** `Java 8`
>    - **Minecraft Version 1.17-1.20.4 -** `Java 17`
>    - **Minecraft Version 1.20.5-1.21.10 -** `Java 21`
>    - **Minecraft Version 1.21.11 and Later -** `Java 25`
### Installing Minecraft
- Launch Prism Launcher and continue until the **memory allocation** step.
- Next, make sure to change `Maximum memory allocation` value.
> [!WARNING]
> - There is a rumor that if you allocate **half your RAM**, you are going to get **good performance**. However, this is **wrong** because:
> - When you play Minecraft, the game tries to **free up allocated memory** that is no longer used by objects to **avoid memory issues**. This is called **garbage collection**.
>   - However, you **should not** allocate **too much or too little** RAM, because:
>     - If you allocate **too much** RAM, the game will **wait longer** between **garbage collection cycles** and each cycle will **take longer to complete**, that's why you are going to get **bigger lag spikes**.
>     - If you allocate **too little** RAM, the game will **perform garbage collection too often** and this will cause **big lag spikes** again.
>   - When Minecraft uses between `50-75%` of allocated RAM, it is **the ideal value** for **smaller lag spikes**.
>     - I suggest that you experiment different values yourself to find your ideal value. You can check RAM usage by pressing `F3` during the gameplay.
- After completing quick setup, add your Microsoft account in the launcher.
- **Next** : `Add Instance` **-** `Version` **-** `Select the version you desire and scroll down` **-** `Select "Fabric" as the mod loader` **-** `OK`
## Optimization
- `Settings` **-** `Minecraft` **-** `Tweaks` **-** `Enable Feral GameMode` **&** `Use discrete GPU (only if you have two GPUs)`
- **From the same menu** : `Environment Variables` **-** `Add` **-** `MESA_GLTHREAD=true`
<img width="727" height="93" alt="image" src="https://github.com/user-attachments/assets/29cb6b63-e816-4215-9707-db59f48d3b4c" />

> [!NOTE]
> If you are using **NVIDIA**, you should use the `__GL_THREADED_OPTIMIZATIONS=1` environment variable instead.
- You are ready to play Minecraft now.
- However, the performance of the game can still **be increased** through **performance mods** and **optimized in-game settings**.
## Optifine Method - Recommended for Version 1.16.2 and Earlier
> [!NOTE]
> If you want to use Optifine, I suggest that you use **the official Minecraft launcher** instead because it is going to be **hard and meaningless** to use Optifine through Prism Launcher.
- Simply, download [Optifine](https://optifine.net/downloads) for the Minecraft version you would like to play and click `Install` after running the **.jar** file you downloaded.
### Optifine - In-Game Optimized Settings
- `Options`
  - **Video Settings**
    - `Graphics` **:** Fast
    - `Smooth Lighting` **:** ON
    - `Smooth Lighting Level` **:** 50%
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 8 chunks
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
    - `Entity Shadows` **:** OFF
    - **Quality...**
      - `Mipmap Levels` **:** 1
      - `Connected Textures` **:** Fast
      - `Distortion Effects` **:** 60%
      - `FOV Effects` **:** 60%
    - **Details...**
      - `Clouds` **:** OFF
      - `Trees` **:** Fast
      - `Fog` **:** OFF
      - `Rain & Snow` **:** Fast
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
      - `Particles` **:** Decreased
    - **Other...**
      - `Telemetry` **:** OFF
## Sodium Method - Recommended for Version 1.16.3 and Later
`Right click Minecraft instance` **-** `Edit` **-** `Mods` **-** `Download mods`
### Mods That You Need to Use Sodium
- [Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)
- [Sodium](https://modrinth.com/mod/sodium)
- [Sodium Extra](https://modrinth.com/mod/sodium-extra)
### Sodium - In-Game Optimized Settings
- **If you are going to use Zoomify :** `Options` **-** `Controls` **-** `Key Binds` **-** `Fix any conflicting key binds` **-** `Done`
- `Options` **-** `Video Settings`
  - **General**
    - `Render Distance` **:** 6 chunks
    - `Simulation Distance` **:** 8 chunks
    - `VSync` **:** OFF
    - `Max Framerate` **:** Same value as your **monitor's refresh rate**. If your monitor's refresh rate is **lower than 144 Hz**, try either *unlimited* (might cause overheating) or *double your monitor's refresh rate* (e.g., 120 FPS for 60 Hz screen)
    - `Graphics API` **:** Prefer OpenGL - *you can prefer Vulkan as well but you might face mod incompatibilities*
  - **Quality**
    - `Clouds` **:** OFF
    - `Particles` **:** Decreased
    - `Biome Blend` **:** 3x3 Blocks
    - `Entity Distance` **:** 50%
    - `Entity Shadows` **:** OFF
    - `Mipmap Levels` **:** 1x
    - `Texture Filtering` **:** None
## Essential Performance-Increasing Mods for Sodium
- [AsyncParticles](https://modrinth.com/mod/asyncparticles)
- [BadOptimizations](https://modrinth.com/mod/badoptimizations)
- [Better Biome Reblend](https://modrinth.com/mod/bbrb)
- [Concurrent Chunk Management Engine](https://modrinth.com/mod/c2me-fabric)
- [Debugify](https://modrinth.com/mod/debugify)
- [Entity Culling](https://modrinth.com/mod/entityculling)
- [Exordium](https://modrinth.com/mod/exordium)
  - This mod **is not necessary anymore** starting from **version 1.21.10 and later**.
- [Fabric API](https://modrinth.com/mod/fabric-api)
- [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin)
- [Fast IP Ping](https://modrinth.com/mod/fast-ip-ping)
- [FastQuit](https://modrinth.com/mod/fastquit)
- [FerriteCore](https://modrinth.com/mod/ferrite-core)
- [GPUBooster](https://modrinth.com/mod/gputape)
  - If you use **NVIDIA 16xx and newer series**, you can use [Nvidium](https://modrinth.com/mod/nvidium) instead.
- [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast)
- [Krypton](https://modrinth.com/mod/krypton)
- [Lithium](https://modrinth.com/mod/lithium)
- [Mod Menu](https://modrinth.com/mod/modmenu)
- [ModernFix](https://modrinth.com/mod/modernfix)
  - This mod does not support newer versions. In this case, you might want to get its **forked version**: [ModernFix-mVUS](https://modrinth.com/mod/modernfix-mvus)
- [More Culling](https://modrinth.com/mod/moreculling)
- [No Chat Reports](https://modrinth.com/mod/no-chat-reports)
- [NoisiumForked](https://modrinth.com/mod/noisiumforked)
  - The official mod has been **archived**, that's why you should use the **forked version**.
- [Remove Reloading Screen](https://modrinth.com/mod/rrls)
- [RenderScale](https://modrinth.com/mod/renderscale)
  - You should **manually configure** this mod in order to make it work using Mod Menu.
    - `Minecraft` **-** `Options...` **-** `Video Settings...` **-** `RenderScale` **-** `General` **-** `Scale factor`
      - Usually, `50%` is **the most acceptable value** that will not strain the eyes while improving performance. However, you can prefer `60%` as well if 50% strains your eyes.
- [ScalableLux](https://modrinth.com/mod/scalablelux)
### Optional Performance-Increasing Mods for Sodium
- [Alternate Current](https://modrinth.com/mod/alternate-current)
- [Clumps](https://modrinth.com/mod/clumps/versions)
- [Fadeless](https://modrinth.com/mod/fadeless)
- [Fast Item Frames](https://modrinth.com/mod/fast-item-frames)
- [FastChest](https://modrinth.com/mod/fastchest)
- [Let Me Despawn](https://modrinth.com/plugin/lmd)
## Quality of Life Mods for Sodium
> [!NOTE]
> These mods **do not increase performance** but they can **enhance** your **gaming experience**. However, you should keep in mind that some of these mods **might reduce your performance**.
- [AppleSkin](https://modrinth.com/mod/appleskin)
- [Better Advancements](https://modrinth.com/mod/better-advancements)
- [Better Clouds](https://modrinth.com/mod/better-clouds)
  - This mod **might reduce** your in-game **performance**.
- [Better Mount HUD](https://modrinth.com/mod/better-mount-hud)
- [BetterF3](https://modrinth.com/mod/betterf3)
  - If you are using **Exordium** mod, you might want to either not use it or disable the animations of **BetterF3** because **Exordium** reduces the FPS of GUI in order to increase game performance.
- [Chat Heads](https://modrinth.com/mod/chat-heads)
- [Continuity](https://modrinth.com/mod/continuity)
- [e4mc](https://modrinth.com/mod/e4mc)
- [Entity Model Features](https://modrinth.com/mod/entity-model-features)
- [Entity Texture Features](https://modrinth.com/mod/entitytexturefeatures)
  - You can install a resource pack to benefit the effects of **EMF** and **ETF** mods: [Fresh Animations](https://modrinth.com/resourcepack/fresh-animations)
- [Explosive Enhancement](https://modrinth.com/mod/explosive-enhancement)
- [Hold My Items](https://modrinth.com/mod/hold-my-items)
  - This mod **might reduce** your in-game **performance**.
- [Iris Shaders](https://modrinth.com/mod/iris)
- [LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)
- [MinecraftCapes](https://modrinth.com/mod/minecraftcapes)
- [Model Gap Fix](https://modrinth.com/mod/modelfix)
- [Not Enough Animatons](https://modrinth.com/mod/not-enough-animations)
- [Sit](https://modrinth.com/mod/bl4cks-sit)
- [Smooth Scrolling](https://modrinth.com/mod/smooth-scroll)
  - If you want to use this mod, **disable** **Exordium** because **Exordium** reduces the FPS of GUI in order to increase game performance.
- [Subtle Effects](https://modrinth.com/mod/subtle-effects)
  - This mod **might reduce** your in-game **performance**.
- [ViaFabricPlus](https://modrinth.com/mod/viafabricplus)
- [Zoomify](https://modrinth.com/mod/zoomify)
## Global Quality of Life Resource Packs
- [3D Ladders](https://modrinth.com/resourcepack/3d-ladders)
- [Armored Legacy](https://modrinth.com/resourcepack/armored-legacy)
  - Make sure to check this resource pack's description before using as it **requires some dependencies**.
- [Better Boat](https://modrinth.com/resourcepack/better-boat)
- [Better Lanterns](https://modrinth.com/resourcepack/better-lanterns)
- [Better Lily Pads](https://modrinth.com/resourcepack/better-lily-pads_)
- [Better Leaves](https://modrinth.com/resourcepack/better-leaves)
- [Cat Creepers x Fresh Animations](https://modrinth.com/resourcepack/cat-creepers-x-fresh-animations)
  - You should use this resource pack with **Fresh Animations** resource pack.
- [Cubic Sun & Moon](https://modrinth.com/resourcepack/cubic-sun-moon)
- [Extra Flowery GUI](https://modrinth.com/resourcepack/extra-flowery-gui)
- [Fancy Beds](https://modrinth.com/resourcepack/fancy-beds)
- [Flowering Crops](https://modrinth.com/resourcepack/flowering-crops)
- [Fluffy Carpets and Wool](https://modrinth.com/resourcepack/fluffy-carpets)
- [Better Cats x Fresh Animations](https://modrinth.com/resourcepack/better-cats-x-fresh-animations)
  - You should use this resource pack with **Fresh Animations** resource pack.
- [Fresh Skeleton Physics](https://modrinth.com/resourcepack/fresh-skeleton-physics)
  - You should use this resource pack with **Fresh Animations** resource pack.
- [Improved Fences](https://modrinth.com/resourcepack/improved-fences)
- [Multi-Color Flowering Vines](https://modrinth.com/resourcepack/multi-color-flowering-vines)
- [Overdetailed Saplings](https://modrinth.com/resourcepack/overdetailed-saplings)
- [PDB3D's Blocky Armor Stands - Arms Version](https://modrinth.com/resourcepack/blocky-armor-stands)
- [Rainbow XP Bar](https://modrinth.com/resourcepack/rainbow-xp-bar)
- [Remodeled Cactus](https://modrinth.com/resourcepack/remodeled-cactus)
- [Remodeled Doors 3D](https://modrinth.com/resourcepack/remodeled-doors)
- [Simple Grass Flowers](https://modrinth.com/resourcepack/simple-grass-flowers)
- [Torches Reimagined](https://modrinth.com/resourcepack/torches-reimagined)
- [Undopia 3D Sugar Cane](https://modrinth.com/resourcepack/undopia-3d-sugar-cane)
- [Visible Ores](https://modrinth.com/resourcepack/visible-ores)
# Conclusion
This guide was about Minecraft installation and optimization on Linux. I hope the guide has been useful. Thank you for reading, happy gaming!
