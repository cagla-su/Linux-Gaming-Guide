# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#before-starting)	
 	- [How Does Linux Gaming Work?](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#how-does-linux-gaming-work)
	- [Issues of Linux Gaming](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#issues-of-linux-gaming)
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?search=1#get-started)
	- [Installing Vulkan Drivers](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
	- [Installing Gaming Software](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software)
	- [Hybrid Graphics Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#hybrid-graphics-setup)
		- [Ways to Run Games through the Dedicated GPU](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#ways-to-run-games-through-the-dedicated-gpu)
	- [External Disk Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#external-disk-setup)
 		- [Get Started: GParted](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#get-started-gparted)
   		- [How to Configure External Disks on Linux?](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-to-configure-external-disks-on-linux)
	- [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#optimization-tips)
 		- [Reducing Game Resolution and Using the Lowest Graphics Settings](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#reducing-game-resolution-and-using-the-lowest-graphics-settings)
   			- [Lossless Scaling](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#lossless-scaling)
  		- [Using a Performance Kernel](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#using-a-performance-kernel)
		- [Gamemode](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#gamemode)
		- [Performance-Increasing Launch Options](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#performance-increasing-launch-options)
			- [How Can You Use These Launch Options?](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-can-you-use-these-launch-options)
		- [Disabling Compositor](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#disabling-compositor---x11-only)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#conclusion)
## Game-Specific Guides
- **Genshin Impact -** [Genshin Impact Linux Guide](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md)
	- 🇹🇷 **Türkçe Çevirisi -** [Genshin Impact Linux Rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md)
- **Minecraft -** [Minecraft Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
	- 🇹🇷 **Türkçe Çevirisi -** [Minecraft Linux Rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Minecraft-tr.md)
- **The Sims 2 -** [The Sims 2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
	- 🇹🇷 **Türkçe Çevirisi -** [The Sims 2 Linux Rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/The-Sims-2-tr.md)
## Türkçe Çeviri 🇹🇷
> [!NOTE]
> Rehberin [Türkçe çevirisi buradadır](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md). Birebir çeviri değildir fakat içerik aynıdır.
# Linux Gaming Guide
- Hello! This guide aims to help you understand **how gaming on Linux works**, **how to prepare your system for gaming** and **how to optimize your system for higher performance**.
- If you are ready, let's begin!
# Before Starting
> [!NOTE]
> - Linux gaming is **swiftly improving**. Every passing day, more users switch to Linux. In this context, the **market share** of Linux gaming is **increasing**.
> - This guide aims to be useful for everyone who wants to **play games** on Linux but **does not know** where to start.
> - After reading this guide, feel free to check out [Game-Specific Guides](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#game-specific-guides) if any of the listed games interest you.
## How Does Linux Gaming Work?
- You can play **most of the Windows games** on Linux. However, this **does not mean** that there are **no native Linux games**. **Some native Linux games** are:
	- Minecraft, Terraria, Stardew Valley, Euro Truck Simulator 2 and more
 	- **Valve games** such as Counter-Strike series, Team Fortress 2, Dota 2, Portal etc.
- Generally, native Linux games **do not require** any extra steps **unless they do not require Vulkan**. If they do, you need to **install Vulkan drivers** which is explained in this guide.
- Windows games require some **essential tools** in order to run on Linux and these tools are:
	- [WINE](https://www.winehq.org/) / [Proton](https://github.com/ValveSoftware/Proton) **-** WINE is a compatibility layer which directs **Windows library files** into **Linux library files**. It works the same as the **compatibility mode on Windows**.
 		- Proton is Valve's **fork** of WINE and it is **specifically configured for Steam games**.
	- [DXVK](https://github.com/doitsujin/dxvk) **-** DXVK translates **DirectX 8-11** calls into **Vulkan** to make Windows games run on Linux. DXVK is **not included** in WINE but you still **do not need to install DXVK manually** because **most** of the **Linux gaming software** and **custom WINE/Proton builds** include DXVK for users.
		- There are some **other tools** that are used for **similar purposes** as DXVK, these tools are:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d) **-** VKD3D translates **DirectX 12** calls into **Vulkan** which DXVK cannot yet. VKD3D **serves as the fallback** if the game you are trying to play is a **DirectX 12 game**. Just like DXVK, VKD3D is **automatically included** in **most** of the **Linux gaming software** and **custom WINE/Proton builds**.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d) **-** WINED3D translates **DirectX 8-11** calls into **OpenGL instead of Vulkan**. WINED3D **serves as the fallback** if your system **does not have Vulkan drivers installed**. However, since DirectX calls will be translated into OpenGL, you are likely to experience **poor performance** because OpenGL is **deprecated**. **Unlike** DXVK and VKD3D, WINED3D is **included** in WINE.
```
+------------------+   DirectX: Windows-specific graphics library
|       WINE       |   Vulkan: Both Windows & Linux native graphics library
+------------------+   OpenGL: Both Windows & Linux native graphics library (deprecated)
         ||
         ||
+----------------------------++--------------------------+
|          DXVK              ||           VKD3D          |
| (DirectX 8-11 -> Vulkan)   ||   (DirectX 12 -> Vulkan) |
+----------------------------++--------------------------+
            ||
+--------------------------+
|         WINED3D          |
| (DirectX 8-11 -> OpenGL) |
+--------------------------+

```
> [!NOTE]
> You **do not need to manually install** WINE because WINE is installed **automatically** when you install a gaming software such as Lutris.

> [!WARNING]
> - NVIDIA is **phasing out** the **proprietary** drivers for their **4xxx** and **5xxx** series because NVIDIA is attempting to be **more open source** for their **recent and future cards**.
> - However, **for older cards**, you still have to use **proprietary** drivers for **better compatibility and performance**.
> - Also, you **should not use** Wayland **unless** you use one of the recent NVIDIA GPUs that are mentioned above because it is likely for you to experience **glitches and performance issues**. Using X11 is a **better option** for now.
## Issues of Linux Gaming
- There are **not too many issues** when it comes to gaming on Linux. However, the **main limitation** is **kernel-level anti-cheat software**. These anti-cheat software **are not able to run** on Linux.
	- The reason why is a kernel-level anti-cheat software that is developed for a Windows game means that the anti-cheat software **requires a kernel called "Windows NT", which is only available for Windows**.
- Some examples of kernel-level anti-cheat software are:
	- **VANGUARD**
	- **Easy Anti-Cheat**
	- **BattlEye**
	- **XIGNCODE3**
	- **nProtect GameGuard**
- **Easy Anti-Cheat** and **BattlEye** have **Linux-compatible** versions. That's why some developers **may enable Linux compatibility** with their anti-cheat software **specifically for WINE/Proton**.
	- However, **some developers** of games like Fortnite and Apex Legends **do not enable** Linux support in their anti-cheat configurations. That's why **those games cannot run on Linux**.
- In addition to enabling Linux-compatible configurations, some games only use the **user-mode module** of these anti-cheat software, which **makes them playable** on Linux.
- **Except VANGUARD**, we **cannot** make a **definitive statement** about **playability** of a game that uses one of the anti-cheat software mentioned above.
	- The case is **different for VANGUARD** because **no games** using VANGUARD are able to run on Linux. This is because VANGUARD is only used by the games of Riot Games, which **do not intend to support** Linux players at all.
# Get Started
## Installing Vulkan Drivers
> [!NOTE]
> - If you are using **NVIDIA**, please follow [Lutris' Community Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
> - If you use **Intel/AMD**, you get your Vulkan drivers **preinstalled** when you install a **gaming software** such as **Steam** using your package manager.
## Installing Gaming Software
- Some popular gaming software that are available on Linux are:
	- [Steam](https://store.steampowered.com/)
	- [Heroic Games Launcher](https://heroicgameslauncher.com/) **-** Heroic is a useful game launcher for playing games from **Epic Games, GOG and Prime Gaming** platforms.
	- [Lutris](https://lutris.net/) **-** Lutris is a feature-rich game launcher **for playing Windows games**. You can **directly** install some gaming software platforms such as **Epic Games, Battle.net, Ubisoft etc.** and run them using Lutris but you can also play games that are not tied to a certain platform.
		- Lutris provides **community-made installation scripts** for a **large number** of games and software.
		- You can also install your games **manually**, including **DVD games**, if you have the setup files.
	- [AAGL](https://github.com/an-anime-team/an-anime-game-launcher) **-** AAGL (An Anime Game Launcher) is a feature-rich game launcher for playing **Genshin Impact**, which **disables telemetry** and **applies patches automatically** to keep the game working after updates.
	- [ProtonPlus](https://protonplus.vysp3r.com/) **-** You can install **custom WINE/Proton builds** for **better compatibility** and **performance** using ProtonPlus. Custom WINE/Proton builds **are supported** by Lutris, Steam and Heroic.
	- [Sober](https://sober.vinegarhq.org) **-** Sober is a game launcher for playing **Roblox's** Android version on Linux. In the past, it was possible to run the Windows version of Roblox through **VinegarHQ**. However, it is **borked** now due to the **anti-cheat configuration**. That's why **Sober** is the new way of playing Roblox on Linux.
	- [Prism Launcher](https://prismlauncher.org) **-** Prism Launcher is a feature-rich game launcher for playing **Minecraft**.
 		- I have a [Minecraft guide](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md) for configuring and optimizing Minecraft, if you are interested.
	- [Waydroid](https://waydro.id/) **-** Waydroid is is a **container-based compatibility layer** that **allows Android to run on Linux**. So you can play Android games on Linux using Waydroid.
 		- I have a [Waydroid guide](https://github.com/cagla-su/Waydroid-Guide) for your questions in mind, installation and configuration steps, if you are interested.
> [!TIP]
> - You can install these software through either your **package manager** or [Flatpak](https://flatpak.org).
> - You can check [ProtonDB](https://www.protondb.com) to see whether your Steam games are playable on Linux.
>   - If the game you searched is ranked **lower than silver**, that means it is **unplayable**.
>	- You can get **optimization tips** if there are any reviews written for your game. If you wish, you can write your own reviews for any Steam game you wish.
# Hybrid Graphics Setup
- If your system has **two GPUs (1 integrated + 1 dedicated)**, it is recommended to **install Vulkan drivers for both hardware** and set games to run through your dedicated GPU.
- To run games using your dedicated **AMD** GPU, use the following command:
```
DRI_PRIME=1
```
 - To run games using your **NVIDIA** GPU, use the following command:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Ways to Run Games Through the Dedicated GPU
- There are **four ways** of running games through your dedicated GPU:
	- **1 -** [Terminal Method](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#terminal-method-)
 	- **2 -** [Desktop Shortcut Method](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#desktop-shortcut-method-%EF%B8%8F)
 	- **3 -** [For Steam Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games-)
  	- **4 -** [For Lutris & Heroic Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-lutris--heroic-games--)
### Terminal Method
Simply, launch terminal and execute the command for your GPU like in the example:
```
DRI_PRIME=1 prismlauncher
```
### Desktop Shortcut Method
- Create a **.desktop** file on your desktop.
- This is an example .desktop file content to run Prism Launcher through an NVIDIA GPU. The line you should pay attention is the line that starts with `Exec`:
```
[Desktop Entry]
Version=1.0
Type=Application
Name=Prism Launcher
Comment=Prism Launcher
Exec=env __NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia prismlauncher
Icon=/path/to/your/game/icon.png
Terminal=false
Categories=Game;
```
- Simply, you should add `env` first and the **command for your GPU**. Finally, the package name of the game.
### For Steam Games
Add the command for your GPU in the launch options of your games. **Do not forget** to add `%command%` at last like in the example:
```
DRI_PRIME=1 %command%
```
> [!NOTE]
> If you are going to **additionally** use other launch options and run games through your dedicated GPU, make sure that all the commands are written **before** `%command%` like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### For Lutris & Heroic Games
- **Lutris -** On the left side bar, click the **settings icon** that appears when you point your mouse cursor on `Wine`.
	- `System Options` **-** `Enable Advanced` **-** `Display` **-** `GPU`
 - **Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# External Disk Setup
> [!NOTE]
> - If your external disk is **internally connected**, you might be able to use it **out of the box** depending on your Linux distribution. However, if you are using your external disk **through an SSD case (USB)**, you should configure it manually.
> - These steps also apply if your disk is **internally connected** but still **not working properly**.
## Get Started: GParted
> [!CAUTION]
> - I **strongly suggest** that you **format your disk** to change its file system from **NTFS** to a **Linux-compatible one** because **write support for NTFS** is **experimental** on Linux and it **might corrupt** your drive!!! You have been warned.
- Install `gparted` using your package manager and follow the next steps, **making sure** your external disk is **unmounted** while it is **physically connected**.
	- `Launch GParted` **-** `select your external disk from the top right` **-** `delete all the partitions` **-** `Add`
 	- **Next -** `File system: ext4 (or xfs, if you wish)` **-** `Label: anything you wish` **-** `Add`
  	- **Finally -** `Apply All Operations`
## How to Configure External Disks on Linux?
- First of all, install `gnome-disk-utility` package using your package manager.
	- If you **insist** about using your external disk **as NTFS** anyway, additionally install `ntfs-3g` package using your package manager.
- After the installation, launch `Disks` app from your application launcher.
- Then, find your external disk from the menu on the left and click this button under `Volumes`:
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- From the menu, click `Take Ownership (Recursive)` and confirm.
- After taking the ownership, open the same menu and click `Edit Mount Options`.
  - Now disable `User Session Defaults` and check `Mount at system startup`.
  - Next, find the box that does not have a label that is under `Symbolic Icon Name` box and make sure you only have these mount options:
  	- `nofail,x-gvfs-show,rw,user,exec`
   - If you are going to use your external disk **as NTFS**, you should additionally include `ntfs-3g` option like in the example:
        - `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
   - Finally, change `Identify As` value to `/dev/disk/by-label/your-disk` and click OK.
<img width="904" height="493" alt="imagee" src="https://github.com/user-attachments/assets/56cf7ae7-d9f7-42fc-81de-b23b671622d2" />

- Now you are ready to use your external disk(s)! 

# Optimization Tips
## Reducing Game Resolution and Using the Lowest Graphics Settings
> [!TIP]
> - When you reduce the resolution of a game, **less pixels will be rendered** and it will result in **less loads** on your hardware, leading to **higher performance**.
> - When you play with the lowest graphics settings, **less details will be rendered**, leading to **higher performance**.
> - Both are going to **increase performance** while **reducing visual quality**. You can experiment to find your own balanced settings.
### Lossless Scaling
It is possible to play your games in **lower resolutions** while **not losing anything from visual quality** thanks to [Lossless Scaling](https://store.steampowered.com/app/993090/Lossless_Scaling/). However, you **must purchase** the app from Steam to be able to use it.
- After purchasing Lossless Scaling, you should **install [lsfg-vk](https://github.com/PancakeTAS/lsfg-vk)** to be able to use it on Linux.
	- However, your **GPU must support Vulkan** and your **system must have Vulkan drivers installed** in order to use this feature!
## Using a Performance Kernel
- **Arch Linux and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **Fedora Linux and Derivatives:** [CachyOS Kernel Port For Fedora](https://github.com/CachyOS/copr-linux-cachyos)
- **Debian/Ubuntu Linux and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a tool that **temporarily changes** your **system configurations** to increase performance during the gameplay.
> [!NOTE]
> - Generally, gaming software like Lutris **enable it by default**.
> - However on Steam, you should **manually add a command** in your game's launch options like in the example:
```
gamemoderun %command%
```
## Performance-Increasing Launch Options
You can use these launch options for higher performance while gaming:
- `DXVK_LOG_LEVEL=none` **-** It **suppresses all DXVK logs** to increase performance as gaming software **will not spend time processing and writing log data**. - *Medium impact on performance*
- `WINEDEBUG=-all` **-** It **suppresses all debug outputs of WINE**. - *Low impact on performance*
- `WINE_LARGE_ADDRESS_AWARE=1` **-** It **allows 32-bit applications to consume up to 4 GB RAM instead of 2 GB**. - *Variable impact depending on the game, generally medium.*
- `MESA_GLTHREAD=true` **-** It improves **OpenGL performance** on **Intel/AMD GPUs**. - *High impact on performance*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** It improves **OpenGL performance** on **NVIDIA GPUs**. - *High impact on performance*
### How Can You Use These Launch Options?
- **Steam -** You can simply use these commands in launch options section that is [previously mentioned](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games-).
- **Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />

- **Heroic -** `Settings` **-** `Game Defaults` **-** `ADVANCED` **-** `Environment Variables` **-** `+`
<img width="513" height="180" alt="image" src="https://github.com/user-attachments/assets/557adebe-23e7-4c8b-93e2-0378cb38faae" />

## Disabling Compositor - X11 ONLY!!!
> [!WARNING]
> If you are using Wayland, disabling the compositor is **not possible**. These steps are only available for X11.
- A disabled compositor **simply means disabled animations and transparency**. Also, it causes screen tearing which **reduces visual quality while improving performance**.
- This step is explained in [Linux Gaming wiki](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)).
# Conclusion
This guide was about Linux gaming. Thank you for reading. I hope this guide has helped you prepare your system for gaming on Linux. Happy gaming!

