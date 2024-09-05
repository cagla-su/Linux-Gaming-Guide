# Minecraft
So, Minecraft is actually a **Linux-native** game that works with OpenGL. We won't get tired while configuring Minecraft. This is going to be fun!
## Get Started
First of all, I definitely suggest you to use [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) because it is **open-source** and provides more options than original launcher.
### Install Prism Launcher
You can install Prism Launcher following [these steps according to your distribution](https://prismlauncher.org/download/linux/), the recommended way is installing it from Flatpak and it will configure everything itself including Java builds.
### Install Java
You should **skip** this step if you chose to install the launcher from **Flatpak**.
- You can install Java following [these steps according to your distribution](https://prismlauncher.org/wiki/getting-started/installing-java/#installing-java-on-linux)
- If you don't see your distribution here, you should install the game from Flatpak.
### Install Minecraft
- When you first launched the launcher, it'll ask you what language would you like to use. After that question, you're going to see a page about Java.
- Make sure to change **Maximum memory allocation**. Some people claim you should allocate half of your RAM but this is not good for **some cases**. If you have at least 32 GB RAM and don't perform RAM intensive tasks, you can allocate half of your RAM. However:
  - If you have **4/6/8/12/16 GB RAM**, I suggest you to allocate **1024 MiB** if you're not going to install heavy mods.
  - First, try **1 GB** allocated RAM, if you face instability, you can try allocating **2048** or **3072 MiB RAM** to configure stability.
- After completing quick setup, add your Microsoft account to connect to your account in the launcher.
- Now we can finally install Minecraft. Let's click on **Add Instance** button on top left and continue:
  - On **Version** section, choose the version you'd like to play and scroll down a bit. You should see a big "**No mod loader is selected.**" warning. There is a **Mod loader** section next to the warning. We're going to choose **Fabric** from there and hit **OK**.
## Optimization
### Before Getting Started
- **OpenGL and Java** are already **better optimized** on Linux. However, we can still boost our GL performance, we're going to add an **environment variable**. I'm not sure about GNOME but on XFCE and KDE, adding an environment variable is possible via these steps:
  - Right click on Prism Launcher and go to **Properties**
    - **For XFCE**: Make sure **command** section looks like this:
      - **For Intel/AMD GPU**: *env mesa_glthread=true prismlauncher %U*
      - **For NVIDIA GPU**: *env __GL_THREADED_OPTIMIZATIONS=1 prismlauncher %U*
    - **For KDE**: Go to **Application** section and make sure **environment variables** section looks like this
      - **For Intel/AMD GPU**: *mesa_glthread=true*
      - **For NVIDIA GPU**: *__GL_THREADED_OPTIMIZATIONS=1*
- Another and an easier way is to run Prism Launcher via terminal using one of the commands for your GPU like this:
  - *mesa_glthread=true prismlauncher*
- Now, let's enable some settings for even better performance in Prism Launcher.
  - Click on **Settings** and go to **Minecraft** section and click on **Tweaks**. Enable **Enable Feral GameMode** (only if you have gamemode installed) and **Use discrete GPU** (only if you have 2 GPUs).
### Performance Mods
- Now, let's install some performance mods! I will be installing mods for **1.20.1** version, that means if you are going to use a newer version of the game, some of those mods **may not** be available for the version you play.
- First of all, click on your Minecraft instance once and then click on **Edit** on the right side bar.
- In the opened page, click on **Mods** on the left side bar and click on **Download mods** on the right side bar and make sure **Modrinth** is selected. We're ready to install some mods!
  - Don't forget to click on **Select mod for download** after selecting each mod.
- These are the mods I suggest you to use for a smoother gameplay:
  - [Alternate Current](https://modrinth.com/mod/alternate-current/version/mc1.20-1.8.0-beta.3)
  - [Async Locator](https://modrinth.com/mod/async-locator/version/1.20-1.3.0)
  - [BadOptimizations](https://modrinth.com/mod/badoptimizations/version/2.1.1)
  - [Bedrodium](https://modrinth.com/mod/bedrodium/version/0.2.2)
  - [Cloth Config](https://modrinth.com/mod/cloth-config/version/11.1.118+fabric)
  - [Concurrent Chunk Management Engine](https://modrinth.com/mod/c2me-fabric/version/0.2.0+alpha.11.5+1.20.1)
  - [Continuity](https://modrinth.com/mod/continuity) - Optional, it provides Optifine's connected textures feature
  - [CoroUtil](https://modrinth.com/mod/coroutil/version/1.20.1-1.3.7)
  - [Cull Less Leaves](https://modrinth.com/mod/cull-less-leaves)
  - [Disable Custom Worlds Advice](https://modrinth.com/mod/dcwa/version/4.1)
  - [Dynamic FPS](https://modrinth.com/mod/dynamic-fps)
  - [Enhanced Block Entities](https://modrinth.com/mod/ebe/version/0.9+1.20)
  - [EntityCulling](https://modrinth.com/mod/entityculling/version/1.6.2-1.20.2)
  - [Exordium](https://modrinth.com/mod/exordium/version/1.2.1-1.20.1)
  - [Fabric API](https://modrinth.com/mod/fabric-api/version/0.92.1+1.20.1)
  - [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin/version/1.10.20+kotlin.1.9.24)
  - [Fast Items](https://modrinth.com/mod/fast-items/version/1.0.0-mc1.20.1)
  - [Faster Random](https://modrinth.com/mod/faster-random/version/4.1.0)
  - [FerriteCore](https://modrinth.com/mod/ferrite-core/version/6.0.1)
  - [Fzzy Config](https://modrinth.com/mod/fzzy-config/version/0.3.1+1.20.1)
  - [Icterine](https://modrinth.com/mod/icterine/version/1.3.0)
  - [ImmediatelyFast](https://modrinth.com/mod/immediatelyfast/version/1.2.14+1.20.4-fabric)
  - [Indium](https://modrinth.com/mod/indium/version/1.0.30+mc1.20.4)
  - [Iris](https://modrinth.com/mod/iris/version/1.7.0+1.20.1) - Optional, it allows you to use shaders
  - [Ksyxis](https://modrinth.com/mod/ksyxis/version/1.2.2)
  - [LazyDFU](https://modrinth.com/mod/lazydfu/version/0.1.3)
  - [Let Me Despawn](https://modrinth.com/plugin/lmd/version/1.2.0)
  - [Lithum](https://modrinth.com/mod/lithium/version/mc1.20.1-0.11.2)
  - [Memory Leak Fix](https://modrinth.com/mod/memoryleakfix/version/v1.1.5)
  - [Mobtimizations](https://modrinth.com/mod/mobtimizations/version/1.20.1-1.0.0)
  - [Mod Menu](https://modrinth.com/mod/modmenu/version/7.2.2)
  - [ModernFix](https://modrinth.com/mod/modernfix/version/5.17.0+mc1.20.1)
  - [More Culling](https://modrinth.com/mod/moreculling/version/0.24.0)
  - [More Culling Extra](https://modrinth.com/mod/morecullingextra/version/v1.1-1.20.1)
  - [No Chat Reports](https://modrinth.com/mod/no-chat-reports/version/Fabric-1.20.1-v2.2.2)
  - [No Report Button](https://modrinth.com/mod/nrb/version/1.5.0)
  - [No Resource Pack Warnings](https://modrinth.com/mod/no-resource-pack-warnings/version/1.3.0)
  - [No Telemetry](https://modrinth.com/mod/no-telemetry/version/1.8.0)
  - [Particle Core](https://modrinth.com/mod/particle-core/version/0.2.3+1.20.1)
  - [Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options/version/mc1.20.1-1.7.2)
  - [Remove Reloading Screen](https://modrinth.com/mod/rrls/version/3.2.0-1.20.1-fabric)
  - [Skip Transitions](https://modrinth.com/mod/skip-transitions/version/v1.3.3+mc1.20.x)
  - [Sodium](https://modrinth.com/mod/sodium/version/mc1.20.1-0.5.8)
  - [Sodium Extra](https://modrinth.com/mod/sodium-extra)
  - [Starlight](https://modrinth.com/mod/starlight/version/1.1.2+1.20) - Optional, it is made for rewriting the light engine to fix lighting performance and lighting errors
  - [ThreadTweak](https://modrinth.com/mod/threadtweak/version/0.1.1+mc1.20.2)
  - [Zoomify](https://modrinth.com/mod/zoomify) - Optional, it allows you to zoom via C keybind.
### In-Game Optimized Settings
- **If you're going to use Zoomify**:
  - Click on **Options** and go to **Controls** - **Key Binds** and scroll down until you see a red key bind.
  - **Save Hotbar Activator** has C button as key bind, change it to something else and hit **Done**
- Go to **Options** and go to **Resource Packs**. Now move **Default Connected Textures** and **Glass Pane Culling Fix** from left section to right section and hit **Done**.
- Go back to **Options** and go to **Video Settings**. These are optimized settings for performance:
  - **General**
    - **Render Distance**: 6 chunks
    - **Max Shadow Distance**: Disabled
    - **Simulation Distance**: 5 chunks
    - **VSync**: Subjective
      - In some cases, VSync can be useful, try it on both conditions and decide which one is better.
  - **Quality**
    - **Graphics**: Fast
    - **Clouds**: OFF
    - **Weather**: Fast
    - **Leaves**: Fancy
    - **Particles**: Decreased
    - **Biome Blend**: 1 block(s)
    - **Entity Distance** 50%
    - **Entity Shadows**: OFF
    - **Distortion Effects**: 60%
    - **FOV Effects**: 60%
    - **Mipmap Levels**: 2x
- We're done!
## Conclusion
So, that was my Minecraft installation and optimization guide! I hope you enjoyed it while reading and I hope the guide can be useful for you. Have a nice day!
