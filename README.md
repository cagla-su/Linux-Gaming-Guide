## Table of Contents
- [How Linux Gaming Works](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#how-linux-gaming-works)
- [Installing Vulkan Drivers](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
- [Installing Gaming Software](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software)
- [External Disk Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#external-disk-setup)
- [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#optimization)
## Game-Specific Guides
- ![Metin2](https://github.com/user-attachments/assets/c887fc49-cc62-4450-81ab-7ebdfe0087df) **Metin2 -** [Metin2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md)
-  ![Minecraft](https://github.com/user-attachments/assets/3dd086b5-0be3-4cc9-ab2f-e01243845930) **Minecraft -** [Minecraft Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- ![Sims 2](https://github.com/user-attachments/assets/5e79e395-066b-46df-85a4-a72f73d8aad8) **The Sims 2 -** [The Sims 2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
# Linux Gaming Guide
Hello. In this guide, you will be informed about how **gaming on Linux works**, how to **prepare your system for gaming on Linux** and how to **optimize your Linux system for higher performance**. If you are ready, let's begin!
## Before Starting
- Linux gaming is swiftly improving. Every passing day, more users start switching to Linux. Also, the market share of Linux gaming is increasing in this context.
- This guide aims to be useful for everyone who wants to play games on Linux but does not know where to start.
- After reading this guide, I suggest that you read [Game-Specific Guides](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#game-specific-guides) if you see any game on the list that you desire to play.
# How Linux Gaming Works
- You can play Windows games on Linux. However, this **does not mean** that there **are not any native Linux games**. **Some native Linux games** are:
	- Minecraft, Terraria, Stardew Valley, Euro Truck Simulator 2 and more
 	- **Valve's games:** Counter-Strike series, Team Fortress 2, Dota 2, Portal etc.
- Generally, native Linux games **do not require** any tinkerings **as long as they do not require Vulkan**. If they do, you need to install Vulkan drivers which is explained in this guide.
- Windows games require some **essential tools** in order to run on Linux and these tools are:
	- [WINE](https://www.winehq.org/) / [Proton](https://github.com/ValveSoftware/Proton) **-** WINE is a compatibility layer which directs **Windows library files** into **Linux library files**. It works the same as **the compatibility mode on Windows**. Proton is a **fork of WINE** that is forked by Valve and it is specifically configured for **Steam games**.
	- [DXVK](https://github.com/doitsujin/dxvk) **-** DXVK translates **DirectX 8-11** calls into **Vulkan** to make Windows games run on Linux. DXVK is **included** in WINE, so you **do not have to manually install** DXVK.
		- There are some **other tools** that are used for **similar purposes** as DXVK, these tools are:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d) **-** VKD3D translates **DirectX 12** calls into **Vulkan** which DXVK cannot yet. This is the **default** translation tool if the game you are trying to play is a **DirectX 12 game**. Just like DXVK, VKD3D is **included** in WINE.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d) **-** WINED3D translates **DirectX 8-11** calls into **OpenGL instead of Vulkan**. This is the **default** translation tool if your system **does not have Vulkan drivers installed**. However, since DirectX calls will be translated into OpenGL, you are likely going to get **poor performance** because OpenGL is **deprecated**. Just like DXVK and VKD3D, WINED3D is **included** in WINE.
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
- You **do not have to do anything** to install WINE. WINE is installed **automatically** when you install a gaming software.
## Warning For NVIDIA Users
- NVIDIA is **phasing out** the **proprietary** drivers for their **4xxx** and **5xxx** series because NVIDIA is attempting to be **more open source** for their **recent and future cards**. However, **for older cards**, you still have to use **proprietary** drivers for **better compatibility and performance**.
- Also, you **should not use Wayland** unless you use one of the recent NVIDIA GPUs that are mentioned above because it is likely for you to experience **glitches and/or performance issues**. Using **X11** is a better option for now.
# Get Started
- **1 -** [Installing Vulkan Drivers](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
- **2 -** [Installing Gaming Software](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software)
## Installing Vulkan Drivers
- This step is explained in [Lutris' Community Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you do not see your Linux distribution in the page, that probably means Mesa **(the default Intel/AMD GPU driver)** Vulkan drivers are preinstalled on your Linux distribution.
	- However, if you do not see your distribution in the page and if you are using NVIDIA, I suggest that you find a different documentation for installation steps or switch to one of the distributions that are mentioned in the page.

## Installing Gaming Software
- Some popular gaming software that are available on Linux are:
	- [Steam](https://store.steampowered.com/) **-** Steam is natively supported on Linux.
	- [Heroic Games Launcher](https://heroicgameslauncher.com/) **-** Heroic is a nice game launcher for playing games from **Epic Games, GOG and Prime Gaming**.
	- [Lutris](https://lutris.net/) **-** Lutris is a nice game launcher for playing Windows games. You can **directly** install some gaming software such as **Epic Games, Battle.net, Ubisoft etc.** and run them using Lutris but you can also play games that do not belong to a certain platform.
		- Lutris provides **community-made installation scripts** for huge amount of games and software.
		- You can also install your games manually, including DVD games, if you have the setup files.
	- [ProtonPlus](https://protonplus.vysp3r.com/) **-** You can install custom WINE/Proton builds for better compatibility and performance using ProtonPlus. Custom WINE/Proton builds are supported by Lutris, Steam and Heroic.
### Notes
- You can install these software from either your **package manager** or [Flatpak](https://flatpak.org).
- You can check [ProtonDB](https://www.protondb.com) to see whether your Steam games are playable on Linux.
	- If the game you searched is ranked **lower than silver**, that means it is **unplayable**.
	- You can get optimization tips if there are any reviews written for your game. If you wish, you can write your own reviews for any Steam game you wish.
# External Disk Setup
- If your external disk is **natively** connected, you might be able to use it **out of the box** depending on your Linux distribution. However, if you are using your external disk **through an SSD case (USB)**, you should configure it manually.
- The same steps **should be valid** if your disk is **natively connected** but **you still are not able to use it**.
## Get Started: GParted
- If you would like to format your disk to change its file system from **NTFS** to a **Linux-compatible** one, install `gparted` package using your package manager and follow the next steps, making sure your external disk is unmounted.
	- `Launch GParted` **-** `select your external disk from the top right` **-** `delete all the partitions` **-** `Add`
 	- **Next:** `File system: ext4` **-** `Label: anything you wish` **-** `Add`
  	- **Lastly:** `Apply All Operations`
## How to Configure External Disks on Linux?
- First of all, install `gnome-disk-utility` package using your package manager.
	- Also, if you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, make sure to install `ntfs-3g` package using your package manager.
- After the installation, launch `Disks` app from your application launcher.
- Then, find your external disk from the menu on the left and click this button under `Volumes`.
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- From the menu, click `Take Ownership` and confirm.
- After taking the ownership, open the same menu and click `Edit Mount Options`.
  - Now disable `User Session Defaults` and check `Mount at system startup`.
  - Next, find the box that does not have a label that is under `Symbolic Icon Name` box and make sure you only have these mount options:
  	- `nofail,x-gvfs-show,rw,user,exec`
   - If you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, additionally include this option:
        - `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
   - Lastly, change `Identify As` value to `/dev/disk/by-label/your-disk` and click OK.
<img width="904" height="493" alt="imagee" src="https://github.com/user-attachments/assets/56cf7ae7-d9f7-42fc-81de-b23b671622d2" />

- Now you are ready to use your external disk! 
# Optimization
## Reducing Game Resolution and Using the Lowest Graphics Settings
- When you reduce the game's resolution, less pixels will be rendered and it will result in less loads on your hardware which leads to higher performance.
- When you play with the lowest graphics settings, less details will be rendered which leads to higher performance.
- Both are going to increase performance while reducing visual quality. You can experiment to find your own balanced settings.
## Using a Performance Kernel
- **For Arch and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **For Fedora and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **For Debian/Ubuntu and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a tool that **temporarily** changes your system settings to increase performance during the gameplay. Generally, gaming software like Lutris enable it by default. But on Steam, you have to manually add a command in your game's launch options like in the example:
```
gamemoderun %command%
```
- After installing gamemode, download [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) and move the file to `/etc/` via executing the command below after locating the terminal to your Downloads directory:
```
sudo mv gamemode.ini /etc/
```
## Performance-Increasing Environment Variables
You can use these environment variables for better performance while gaming:
- `WINEDEBUG=-all` **-** It suppresses all debug outputs of WINE. - *low effect on performance*
- `mesa_glthread=true` **-** It improves **OpenGL performance** on **Intel/AMD GPUs**. - *high effect on performance*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** It improves **OpenGL performance** on **NVIDIA GPUs**. - *high effect on performance*
- `DXVK_ASYNC=1` **-** It **does not work on Steam games** but it **displays frames without waiting for shaders to be compiled** which works on Lutris and Heroic. However, using async can **get you banned from online games you play**. That's why, it is only recommended for **offline games**. - *depending on the game, generally low effect on performance*
### How Can You Use These Environment Variables?
- **Steam -** You can simply use these commands in launch options of the games you want to play. Do not forget to add `%command%` at last.
- **Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />

## Disabling Compositor - X11 ONLY!!!
**WARNING**: If you are using **Wayland**, you **cannot** disable the compositor. These steps are only available for **X11**.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which **reduces visual quality while improving performance**.
- This step is explained [in this guide](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)).
# Hybrid Graphics
- If you have **hybrid graphics** setup, it is recommended to install Vulkan drivers for both hardware and set games to run through your dedicated GPU.
- If your dedicated GPU is **AMD**, the necessary command to run games through your dedicated GPU is:
```
DRI_PRIME=1
```
 - If your dedicated GPU is **NVIDIA**, the necessary command to run games through your dedicated GPU is:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Ways to Run Games Through the Dedicated GPU
- There are **4 ways** of running games through your dedicated GPU:
	- **1 -** [Terminal Method](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#terminal-method)
 	- **2 -** [Desktop Shortcut Method](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#desktop-shortcut-method)
 	- **3 -** [For Steam Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games)
  	- **4 -** [For Lutris/Heroic Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-lutrisheroic-games)
### Terminal Method
Simply, launch terminal and execute the command for your GPU like in the example:
```
DRI_PRIME=1 prismlauncher
```
### Desktop Shortcut Method
- Create a **.desktop** file on your desktop.
- This is an example .desktop file content to run Prism Launcher on an NVIDIA GPU. The line you should pay attention is the line that starts with `Exec`:
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
- Simply, you should add `env` first and the command for your GPU. Lastly, the package name of the game.
### For Steam Games
Add the command for your GPU in your launch options of the games you want to play. Do not forget to add `%command%` at last like in the example:
```
DRI_PRIME=1 %command%
```
- **NOTE**: If you are going to use gamemode and run games through your dedicated GPU, make sure that all the commands are written before `%command%` like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### For Lutris/Heroic Games
- **Lutris -** On the left side bar, click the **gear icon** that appears when you point your mouse cursor on `Wine`.
	- `System Options` **-** `Enable Advanced` **-** `Use Discrete Graphics`
 - **Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# Conclusion
This guide was about Linux gaming. I hope the guide has been useful. Thank you for reading, happy gaming! 🐧

