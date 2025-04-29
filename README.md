## Game Specific Guides
- **Minecraft** : [Minecraft Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- **Metin2** : [Metin2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md)
- **The Sims 2** : [The Sims 2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
# Cutie Penguins' Linux Gaming Guide
Hello 🤭. In this guide, you will be informed about **how does gaming on Linux work, how to prepare your system for gaming on Linux and optimization suggestions**.
## Before Starting
- Linux gaming is improving in an accelerated way. As the days go by, more gamers keep switching to Linux and in upcoming years, Linux gaming is expected to be noticed even more.
- My beginner friendly guide is useful for everyone who wants to play games on Linux but doesn't know where to start with. After reading the guide, you might want to check my [Game Specific Guides](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#game-specific-guides).
- So, let's begin!
# How Does Linux Gaming Work?
I would like to explain to you how running Windows games on Linux works.
- Firstly, [WINE](https://www.winehq.org/) (a compatibility layer) is directing **Windows library files** into **Linux library files** just like **the compatibility mode in Windows when you want to play an old game on newer Windows versions**.
- Lastly, [DXVK technology](https://github.com/doitsujin/dxvk) is translating **DirectX 8/9/10/11** (Windows-specific graphics library) calls into **Vulkan** (Windows/Linux native graphics library) with WINE to make Windows games run on Linux.
	- **Tools That Perform the Same Purpose as DXVK**
 		- [VKD3D](https://gitlab.winehq.org/wine/vkd3d)**:** translates **DirectX 12** calls into **Vulkan**.
		- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d)**:** translates **DirectX 8/9/10/11** calls into **OpenGL** if you don't have Vulkan driver installed on your device. 
## A Little Warning For NVIDIA Users
- If you have an **NVIDIA GPU**, steps you should apply will be *a bit harder* because NVIDIA doesn't want to support Linux at all. This was [Linus Torvalds' response to NVIDIA for not supporting Linux in case you want to say the same](https://www.youtube.com/watch?v=_36yNWw_07g) :)))
- Also, **do not use Wayland** if you have an **NVIDIA GPU** because it is likely for you to experience glitches or performance issues. Using **X11** is a better option for now.
## Get Started
We only have 3 steps:
- **1-** [Installing Vulkan Drivers](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#1--installing-vulkan-drivers)
- **2-** [Installing Wine and Wine Dependencies](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#2--installing-wine-and-wine-dependencies)
- **3-** [Installing Gaming Software](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#3--installing-gaming-software)
### 1- Installing Vulkan Drivers
- If you are using an **NVIDIA GPU**, the recommended way is to install the **proprietary** driver from your package manager.
- If you are using an **Intel/AMD GPU**, the recommended way is to install the **open-source** driver from your package manager.
- Both ways are explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you don't see your distribution in the link, that means either your distribution's package manager doesn't include Vulkan drivers or Vulkan drivers are preinstalled (only for Mesa (Intel/AMD) drivers) in your system such as [Fedora did for Mesa drivers](https://packages.fedoraproject.org/pkgs/mesa/mesa-vulkan-drivers/).

### 2- Installing Wine and Wine Dependencies
- First of all, if you are going to install your gaming software from [Flathub](https://flathub.org/), you can skip this step as Flatpak will already install them with WINE and its dependencies.
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/WineDependencies.md)

### 3- Installing Gaming Software
- You just completed the hardest steps! Now it is time for the last and the easiest step. Install your favourite gaming software!
- Some gaming software you might be interested in:
	- [Steam](https://store.steampowered.com/): Steam is natively supported on Linux.
 		- Don't forget to enable **Proton** for Steam. To do so, follow the steps below:
   			- `Steam - Settings - Compatibility - Enable Steam Play for all other titles - Restart Steam`
	- [Heroic Games Launcher](https://heroicgameslauncher.com/): Heroic is made for installing and playing your favourite games from **Epic Games and GOG**.
	- [Lutris](https://lutris.net/): Lutris is made for installing and playing your favourite Windows games. You can use other gaming platforms using Lutris but it also helps with playing games and apps that don't belong to a certain platform.
		- You can search for your games in the app to see if there is a script to install and configure your game automatically.
		- You can install your games (including DVD games) manually if you have the setup files.
	- [Protonup-QT](https://davidotek.github.io/protonup-qt/): You can install custom WINE/Proton builds for a better gameplay that are supported by Lutris, Steam and Heroic.
### Notes
- You can install the software from either your **package manager** or **Flatpak**.
- If you're using [CachyOS](https://cachyos.org/) or if you have [CachyOS repositories](https://github.com/CachyOS/linux-cachyos#cachyos-repositories) enabled in your **Arch system**, you can install [cachyos-gaming-applications](https://github.com/CachyOS/CachyOS-PKGBUILDS/blob/master/cachyos-gaming-applications/PKGBUILD) package to install all the necessary gaming components.
- You can check [ProtonDB](https://www.protondb.com) to see whether your Windows games on Steam are playable on Linux.
	- If the game you searched for is ranked as **silver or lower**, that means it is either **not supported** or **unplayable**.
	- You can get optimization tips if other reviewers wrote any. You can also write your own reviews for any Steam game.
# Optimization
## Reducing Screen Resolution and Using The Lowest Graphics Settings
- Playing a game in fullscreen using **FSR** and a lower resolution is probably the most effective way of increasing gaming performance **alongside lowering graphics settings**.
- If you're gaming on an **iGPU**, you can try reducing your monitor's resolution.
	- To explain it better, on my **Intel UHD 620** with **1920x1080** screen resolution, even reducing my monitor resolution to **1600x900** drastically improves performance in games I play in **windowed/borderless** mode. If you are playing all your games in fullscreen mode, only reducing the game's resolution should be enough and easier.
## Using A Performance Kernel
- **For Arch and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **For Fedora and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **For Debian/Ubuntu and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a project that optimizes your gameplay. Generally, gaming software like Lutris have it enabled by default for your games if you have gamemode installed. But on Steam, you have to manually add a command in your games' launch options like in the example:
```
gamemoderun %command%
```
- After installing gamemode, install [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) and move it to `/etc/` via executing the command after opening terminal in the location where the file is located at:
```
sudo mv gamemode.ini /etc/
```
## Performance-Boosting Environment Variables
You can use these options for better performance while gaming:
- `WINEDEBUG=-all`  - It suppresses all debug outputs of WINE
- `mesa_glthread=true` - It improves **OpenGL performance** on **Intel/AMD GPUs**
- `__GL_THREADED_OPTIMIZATIONS=1` - It improves **OpenGL performance** on **NVIDIA GPUs**
- `DXVK_ASYNC=1` - It **doesn't work on Steam games** but it **displays frames without waiting for shaders to be compiled** which works on Lutris and Heroic. However, using async can **get you banned from your online games that you play**. That's why, it is recommended for **offline games only**.
### How Can You Use These Environment Variables?
- **Steam**: You can simply use these commands in your Steam game's launch options, don't forget to add `%command%` at last
- **Lutris**: In `System Options` section of Lutris, there is another section called `Environment Variables`, you should type the variables like in the example:
 - `Key`: WINEDEBUG | `Value`: -all
## Disabling Compositor - X11/Xorg ONLY!!!
**WARNING**: If you're using **Wayland**, you can't disable the compositor. These steps are only available for **X11/Xorg**.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which **destroys visual quality while improving performance**.
- If you're using **KDE**, you can simply disable the compositor using `Shift - Alt - F12` keybind. To reenable, apply the same keybind.
- If you're using **XFCE**, you can disable the compositor following the steps below:
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
## Ways To Run Software On Dedicated GPU
- There are **4 ways** of running your games on your dedicated GPU:
	- **1-** [Terminal Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#1--terminal-method)
 	- **2-** [Desktop Shortcut Method](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/README.md#2--desktop-shortcut-method)
 	- **3-** [Steam Games Method](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#3--steam-games)
  	- **4-** [Lutris/Heroic Games Method](https://github.com/cutiepenguins/Linux-Gaming-Guide?tab=readme-ov-file#4--lutrisheroic-games)
### 1- Terminal Method
Simply, typing the command for your GPU and the package name of your game:
- **Example:**
```
DRI_PRIME=1 prismlauncher
```
### 2- Desktop Shortcut Method
- Create a **.desktop** file on your desktop and follow the next step.
- I'm going to show you an example content to run **Prism Launcher** via dedicated GPU. The line you should pay attention to is the line that starts with `Exec`:
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
- Simply, we're typing `env` first and the command for your GPU. Lastly, the package name of your game/app.
### 3- Steam Games
Add the command for your GPU on your game's launch options and make sure it has `%command%` at last just like in the example:
```
DRI_PRIME=1 %command%
```
- **NOTE**: If you are going to use gamemode and run a game using dedicated GPU, make sure your all the commands are written before `%command%` just like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### 4- Lutris/Heroic Games
- **Lutris**: On the left side bar, point your mouse cursor on `Wine`, click the **gear icon** that appears.
	- Go to `System Options` and turn on the `Advanced` option, now scroll down a bit. You should turn on the `Use Discrete Graphics` option, after that, make sure you've picked your dedicated GPU's API on `Vulkan API` section. That's all you should do! Make sure to save changes.
 - **Heroic**: On your library, right click your game and go to `Settings`, in the opened window, check `Use Dedicated Graphics Card` option. That's all you should do!
# Conclusion
This guide was about Linux gaming. I hope the guide has been useful. Thank you for reading, have a nice day! 🐧

