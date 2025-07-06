## Game Specific Guides
-  ![Minecraft](https://github.com/user-attachments/assets/3dd086b5-0be3-4cc9-ab2f-e01243845930) **Minecraft** : [Minecraft Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- ![Metin2](https://github.com/user-attachments/assets/c887fc49-cc62-4450-81ab-7ebdfe0087df) **Metin2** : [Metin2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md)
- ![Sims 2](https://github.com/user-attachments/assets/5e79e395-066b-46df-85a4-a72f73d8aad8) **The Sims 2** : [The Sims 2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
# Linux Gaming Guide
Hello. In this guide, you will be informed about how **gaming on Linux works**, how to **prepare your system for gaming on Linux** and how to **optimize your Linux system for higher performance**. If you are ready, let's begin.
## Before Starting
- Linux gaming is improving in an accelerated way. As the days go by, more users keep switching to Linux and the market share of Linux gaming is increasing.
- My guide is useful for everyone who wants to play games on Linux but does not know where to start.
- After reading the guide, I suggest that you read [Game Specific Guides](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#game-specific-guides).
# How Linux Gaming Works
- You can play Windows games on Linux. However, this does not mean that there are not any Linux native games. **Some** Linux native games are:
	- Minecraft, Terraria etc.
 	- Valve's games: Counter-Strike series, Team Fortress 2, Dota 2, Portal etc.
  	- Stardew Valley
  	- Euro Truck Simulator 2
- Generally, Linux native games do not require any tinkerings as long as they do not require Vulkan. If they do, you need to install Vulkan drivers which will be explained in this guide.
- Windows games require some essential tools in order to run on Linux and these tools are:
	- [WINE](https://www.winehq.org/)**:** WINE is a compatibility layer which directs **Windows library files** into **Linux library files**. It works the same as **the compatibility mode on Windows**.
	- [DXVK](https://github.com/doitsujin/dxvk)**:** DXVK translates **DirectX 8/9/10/11** calls into **Vulkan** calls to make Windows games run on Linux. DXVK is included in WINE, so you do not have to manually install DXVK.
		- There are some other tools that are used for similar purposes as DXVK, and these tools are:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d)**:** VKD3D translates **DirectX 12** calls into **Vulkan** which DXVK cannot. Just like DXVK, VKD3D is included in WINE.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d)**:** WINED3D translates **DirectX 8/9/10/11** calls into **OpenGL** instead of **Vulkan**. This is the default translation tool if your system does not have Vulkan drivers installed. However, since DirectX calls will be translated into OpenGL, you are likely going to get poor performance because OpenGL is deprecated. Just like DXVK and VKD3D, WINED3D is included in WINE.
## A Little Warning For NVIDIA Users
- NVIDIA is phasing out the **proprietary** drivers for their **4xxx** and **5xxx** series because NVIDIA is attempting to be more open source for their recent and future cards. However, for older cards, you still have to use **proprietary** drivers for better compatibility and performance.
- Also, you **should not use Wayland** unless you use the NVIDIA GPUs that are mentioned because it is likely for you to experience glitches and/or performance issues. Using **X11** is a better option for now.
## Get Started
- **1-** [Installing Vulkan Drivers](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#1--installing-vulkan-drivers)
- **2-** [Installing WINE and WINE Dependencies](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#2--installing-wine-and-wine-dependencies)
- **3-** [Installing Gaming Software](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#3--installing-gaming-software)
### 1- Installing Vulkan Drivers
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you do not see your Linux distribution in the page, that probably means Vulkan drivers are preinstalled on your Linux distribution.

### 2- Installing WINE and WINE Dependencies
- First of all, if you are going to install your gaming software from [Flathub](https://flathub.org/), you can skip this step as Flatpak will already install WINE with its dependencies.
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/WineDependencies.md)

### 3- Installing Gaming Software
- Some popular gaming software that are available on Linux are:
	- [Steam](https://store.steampowered.com/): Steam is natively supported on Linux.
 		- Do not forget to enable **Proton** for Steam. To do so, follow the steps below:
   			- `Steam - Settings - Compatibility - Enable Steam Play for all other titles - Restart Steam`
	- [Heroic Games Launcher](https://heroicgameslauncher.com/): Heroic is made for installing and playing your favourite games from **Epic Games and GOG**.
	- [Lutris](https://lutris.net/): Lutris is made for installing and playing your favourite Windows games. You can **directly** install some gaming platforms such as **Epic Games, Battle.net** etc. and run them using Lutris but you can also play games and apps that do not belong to a certain platform using Lutris.
		- Lutris provides community-made installation scripts for a huge amount of games and software.
		- You can also install your games (including DVD games) manually if you have the setup files.
	- [Protonup-QT](https://davidotek.github.io/protonup-qt/): You can install custom WINE/Proton builds for better compatibility and performance. Custom WINE/Proton builds are supported by Lutris, Steam and Heroic.
### Notes
- You can install these software from either your **package manager** or **Flatpak**.
- You can check [ProtonDB](https://www.protondb.com) to see whether your Windows games on Steam are playable on Linux.
	- If the game you searched for is ranked as **silver or lower**, that means it is either **not supported** or **unplayable**.
	- You can get optimization tips if other reviewers wrote any. If you wish, you can write your own reviews for any Steam game you want.
# External Disk Setup
If you want to use an external disk to run your games, it will not be ready for use out of the box. That's why it should be configured before using.
## How to Configure External Disks on Linux?
- First of all, install `gnome-disk-utility` package using your package manager.
- Also, if you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, make sure to install `ntfs-3g` package using your package manager.
- After the installation, launch `Disks` app from your application launcher.
	- Then, find your external disk from the menu on the left and click the button under `Volumes`.
 ![image](https://github.com/user-attachments/assets/5f2a8782-17e1-4b31-bbb6-a8683ed4d660)
	- From the menu, click `Take Ownership` and confirm.
 	- After taking the ownership, open the same menu and click `Edit Mount Options`.
  		- Now disable `User Session Defaults` and tick `Mount at system startup`.
    		- Lastly, find the box that does not have a label which is under `Symbolic Icon Name` box and make sure it includes these mount options:
      			- `nofail,x-gvfs-show,rw,user,exec`
         	- If you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, additionally include this option:
          		- `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
            	- Lastly, change `Identify As` value to `/dev/disk/by-label/your-disk` and click OK.
![image](https://github.com/user-attachments/assets/2a5d5461-2c0b-499b-875c-bc51afcf88a5)
- Now you are ready to use your external disk! 
# Optimization
## Reducing Screen Resolution and Using The Lowest Graphics Settings
- When you reduce the game's resolution, less pixels will be rendered and this will cause less loads on your CPU and GPU which will help with higher performance.
- When you play with the lowest graphics settings, less details will be rendered and this will help with higher performance.
- Both are going to increase performance while reducing visual quality. You can try and find your own balanced settings.
## Using A Performance Kernel
- **For Arch and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **For Fedora and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **For Debian/Ubuntu and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a tool that optimizes your gameplay for higher performance. Generally, gaming software like Lutris have it enabled by default for your games if you have gamemode installed. But on Steam, you have to manually add a command in your games' launch options like in the example:
```
gamemoderun %command%
```
- After installing gamemode, install [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) and move it to `/etc/` via executing the command after opening terminal in the location where the file is located:
```
sudo mv gamemode.ini /etc/
```
## Performance-Increasing Environment Variables
You can use these options for better performance while gaming:
- `WINEDEBUG=-all`  - It suppresses all debug outputs of WINE
- `mesa_glthread=true` - It improves **OpenGL performance** on **Intel/AMD GPUs**
- `__GL_THREADED_OPTIMIZATIONS=1` - It improves **OpenGL performance** on **NVIDIA GPUs**
- `DXVK_ASYNC=1` - It **does not work on Steam games** but it **displays frames without waiting for shaders to be compiled** which works on Lutris and Heroic. However, using async can **get you banned from online games you play**. That's why, it is recommended for **offline games only**.
### How Can You Use These Environment Variables?
- **Steam**: You can simply use these commands in your Steam game's launch options, do not forget to add `%command%` at last
- **Lutris**: In `System Options` section of Lutris, there is another section called `Environment Variables`, you should add the variables like in the example:
![image](https://github.com/user-attachments/assets/97d7ad5d-1bd4-48f2-a543-d9d9ef3166b1)

## Disabling Compositor - X11 ONLY!!!
**WARNING**: If you are using **Wayland**, you **cannot** disable the compositor. These steps are only available for **X11**.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which **reduces visual quality while improving performance**.
- If you are using **KDE**, you can simply disable the compositor using `Shift - Alt - F12` keybind. To reenable, apply the same keybind.
- If you are using **XFCE**, you can disable the compositor following the steps below:
	- `Settings Manager` - `Window Manager Tweaks` - `Compositor` - `Enable Display Compositing (uncheck the box)`
- For other desktop environments and other ways of disabling compositor, you can check [this guide](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11))
# Hybrid Graphics
- If you have an **hybrid graphics** setup, you can install Vulkan drivers for both hardware and set your games to run on your dedicated GPU.
- If your dedicated GPU is **AMD**, the necessary command to run the games on the dedicated GPU is:
```
DRI_PRIME=1
```
 - If your dedicated GPU is **NVIDIA**, the necessary command to run the games on the dedicated GPU is:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Ways to Run Software on the Dedicated GPU
- There are **4 ways** of running your games on your dedicated GPU:
	- **1-** [Terminal Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#1--terminal-method)
 	- **2-** [Desktop Shortcut Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#2--desktop-shortcut-method)
 	- **3-** [Steam Games Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#3--steam-games-method)
  	- **4-** [Lutris/Heroic Games Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#4--lutrisheroic-games-method)
### 1- Terminal Method
Simply, open terminal and execute the command for your GPU like in the example:
- **Example:**
```
DRI_PRIME=1 prismlauncher
```
### 2- Desktop Shortcut Method
- Create a **.desktop** file on your desktop and follow the next step.
- This is an example .desktop file to run Prism Launcher on an NVIDIA GPU. The line you should pay attention to is the line that starts with `Exec`:
```
[Desktop Entry]
Version=1.0
Type=Application
Name=Prism Launcher
Comment=Prism Launcher
Exec=env __NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia prismlauncher %U
Icon=/path/to/your/game/icon.png
Terminal=false
Categories=Game;
```
- Simply, you should add `env` first and the command for your GPU. Lastly, the package name of the game.
### 3- Steam Games Method
Add the command for your GPU in your game's launch options and make sure it has `%command%` at last just like in the example:
```
DRI_PRIME=1 %command%
```
- **NOTE**: If you are going to use gamemode and run a game using dedicated GPU, make sure that all the commands are written before `%command%` just like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### 4- Lutris/Heroic Games Method
- **Lutris**: On the left side bar, point your mouse cursor on `Wine` and click the **gear icon** that appears.
	- Go to `System Options` and enable the `Advanced` option.
 	- Enable the `Use Discrete Graphics` option. After enabling, make sure that you selected your dedicated GPU's API in `Vulkan API` section and save the changes.
 - **Heroic**: In your library, right click your game and go to `Settings`.
 	- In the opened window, check `Use Dedicated Graphics Card` option and save the changes.
# Conclusion
This guide was about Linux gaming. I hope the guide has been useful. Thank you for reading, have a nice day! 🐧

