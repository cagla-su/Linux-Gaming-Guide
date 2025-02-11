# How Does Linux Gaming Work?
I would like to explain to you how running Windows games on Linux works.
- Firstly, [WINE](https://www.winehq.org/) (a compatibility layer) is directing **Windows library files** into **Linux library files** just like **the compatibility mode in Windows when you want to play an old game on newer Windows versions**
- Lastly, [DXVK technology](https://github.com/doitsujin/dxvk) is translating **DirectX** (Windows-specific graphics library) calls into **Vulkan** (Windows/Linux native graphics library) to make Windows games run on Linux.
	- If you don't have Vulkan drivers installed or if your GPU doesn't support Vulkan, **WINED3D** is in use instead of DXVK, it directs **DirectX** calls into **OpenGL**.
## Things We Should Know Before Starting
- First thing we need to know is that if you have an **NVIDIA GPU**, steps you should apply will be *a bit harder* because NVIDIA doesn't want to support Linux at all. This was [Linus Torvalds' response to NVIDIA for not supporting Linux in case you want to say the same thing](https://www.youtube.com/watch?v=_36yNWw_07g) :)))
- Second thing we need to know is that you should have a **Vulkan capable GPU** for the best performance which all modern GPUs already support. So, if you have a very old GPU, it probably doesn't support Vulkan which is not good for performance.
- You can still play windows games on Linux if you don't have a Vulkan capable GPU but in this case, DirectX calls will be translated into **OpenGL instead of Vulkan** via **WINED3D** instead of **DXVK** which means you're going to experience lots of performance issues.
## Get Started
We only need to apply 3 steps:
- **1-** `Installing Vulkan Drivers`
- **2-** `Installing Wine and Wine Dependencies`
- **3-** `Installing Gaming Software :)`
### 1- Installing Vulkan Drivers
- If you are using an **NVIDIA GPU**, the best way is to install the **proprietary** driver from your package manager.
- If you are using an **Intel/AMD GPU**, the best way is to install the **open-source** driver from your package manager.
- Both ways are explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you don't see your distribution in the link, that means either your distribution's package manager does not include Vulkan drivers or Vulkan drivers are included preinstalled (only for Mesa (Intel/AMD) drivers) in your system such as [Fedora did for Mesa drivers](https://packages.fedoraproject.org/pkgs/mesa/mesa-vulkan-drivers/).

### 2- Installing Wine and Wine Dependencies
- First of all, if you're going to install your gaming software from [Flathub](https://flathub.org/), then you can skip this step as Flatpak will already install them with wine and its dependencies.
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/WineDependencies.md)

### 3- Installing Gaming Software
- You just completed the hardest steps! Now it's time for the last and the easiest step. Install your favourite gaming software!
- Some gaming software you might be interested in:
	- [Steam](https://store.steampowered.com/): Steam is natively supported on Linux.
 		- Don't forget to enable **Proton** for Steam. To do so, follow the steps below:
   			- `Steam - Settings - Compatibility - Enable Steam Play for all other titles - Restart Steam`
	- [Heroic Games Launcher](https://heroicgameslauncher.com/): Heroic is made for installing and playing your favourite games in Epic Games and GOG.
	- [Lutris](https://lutris.net/): Lutris is made for installing and playing your favourite Windows games.
		- You can search for your games in the app to see if there is an already made script to install and configure your game automatically.
		- You can install your games manually. You can also install your games via DVD.
		- You can install your pirated games if you have setup files.
	- [Protonup-QT](https://davidotek.github.io/protonup-qt/): You can install custom Wine/Proton builds for a better gameplay that are supported by Lutris, Steam and Heroic.
### Notes
- You can install these software from either your **package manager** or **Flatpak**.
- If you're using [CachyOS](https://cachyos.org/) or if you have [CachyOS repositories](https://github.com/CachyOS/linux-cachyos#cachyos-repositories) enabled in your **Arch system**, you can install [cachyos-gaming-meta](https://github.com/CachyOS/CachyOS-PKGBUILDS/blob/master/cachyos-gaming-meta/PKGBUILD) package to install all the necessary gaming components.
- You can use [ProtonDB](https://www.protondb.com) to check whether your Windows games on Steam are playable on Linux.
	- If your game is ranked as **silver or lower**, that means it is **not supported or unplayable**.
	- You can get optimization tips if other reviewers wrote any.
	- You can write your own review for any Steam game after logging in via your Steam account.
# Optimization
## Reducing Screen Resolution
- Playing a game in fullscreen using **FSR** and a lower resolution is probably the most effective way of increasing gaming performance alongside lowering graphics options.
- **ATTENTION!** For gamers who game using iGPU, reducing your monitor's resolution is a better option for you. Your iGPU will render less pixels and colors when you reduce your monitor's screen resolution. PC users with dedicated GPUs won't feel the difference because their GPUs are made to be performant. So for them, reducing game's resolution is enough but iGPU gamers, especially laptop users, will feel the difference a lot.
	- To explain it better, I am using a **Thinkpad T490** with **Intel UHD 620** with **1920x1080** screen resolution and I play **Minecraft** on **1136x640** screen resolution. Using the same game resolution, I get **almost 2x better performance** when I set my monitor resolution as **1280x720**. Plus, I see windows with low resolutions bigger since my GPU is rendering less pixels on the screen which helps with sight issues.
## Using A Performance Kernel
- **For Arch and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **For Fedora and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **For Debian/Ubuntu and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a project that optimizes your gameplay. Generally, gaming software like Lutris have it enabled by default for your games if you have gamemode installed but on Steam, you have to manually add a command on your games' launch options like in the example:
```
gamemoderun %command%
```
- After installing gamemode, install [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) and move it to `/etc/` via executing the command after opening terminal in the location where the file is located in:
```
sudo mv gamemode.ini /etc/
```
## Performance-Boosting Environment Variables
You can use these options for better performance while gaming:
- `WINEDEBUG=-all`  - It suppresses all debug output of wine
- `mesa_glthread=true` - It improves **OpenGL performance** on **Intel/AMD GPUs**
- `__GL_THREADED_OPTIMIZATIONS=1` - It improves **OpenGL performance** on **NVIDIA GPUs**
- `DXVK_ASYNC=1` - It **doesn't work on Steam games** but it **displays frames without waiting for shaders to be compiled** which works on games from other platforms.
### How Can We Use These Environment Variables?
- **Steam**: You can simply use these commands in your Steam game's launch options, don't forget to add `%command%` at last
- **Lutris**: On `System Options` section of Lutris, there is another section called `Environment Variables`, you should type the variables like in the example:
 - `Key`: WINEDEBUG | `Value`: -all
## Disabling Compositor - X11/Xorg ONLY!!!
**WARNING**: If you're using **Wayland**, you can't disable compositor. The steps are only available for **X11/Xorg**.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which destroys visual quality while improving performance.
- If you're using **KDE**, you can simply disable compositor using `Shift - Alt - F12` keybind. To reenable it, apply the same keybind.
- If you're using **XFCE**, you can disable compositor following the steps below:
	- `Settings Manager` - `Window Manager Tweaks` - `Compositor` - `Enable Display Compositing (uncheck the box)`
- For other desktop environments and other ways of disabling compositor, you can check [this guide](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11))
# Hybrid Graphics
- Hybrid graphics setup is not an issue on Linux at all.
- If you have an **Intel/AMD + NVIDIA** setup, you can install Vulkan drivers for both hardware and set your games to run on your dedicated GPU.
- If your dedicated GPU is **AMD**, the necessary command to run the games on the dedicated GPU is:
```
DRI_PRIME=1
```
 - If your dedicated GPU is **NVIDIA**, the necessary command to run the games on the dedicated GPU is:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Ways To Run Software On Dedicated GPU
- If you're using **GNOME**, you can simply right click on the icon of the game you'd like to run on your dedicated GPU, you should see an option to run it with discrete graphics.
- If you're **not** using **GNOME**, here are **4 ways** of running your games on your dedicated GPU:
	- **1-** `Terminal Way`
 	- **2-** `Desktop Shortcut Way`
 	- **3-** `Steam Games`
  	- **4-** `Lutris/Heroic Games`
### 1- Terminal Way
Simply, typing the command for your GPU and the package name of your game:
- **Example:**
```
DRI_PRIME=1 prismlauncher
```
### 2- Desktop Shortcut Way
- Create a **.desktop** file on your desktop and follow the next step.
- I'm going to show you an example content to run **Prism Launcher** via dedicated GPU. Make sure your file also has the line that starts with `Exec` to look like this:
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
- Simply, we're typing `env` first and then the command for your GPU, lastly, package name of your game/app.
### 3- Steam Games
Add the command for your GPU on your game's launch options and make sure it has `%command%` at last just like in the example:
```
DRI_PRIME=1 %command%
```
- **NOTE**: If you're going to use gamemode and run your game on your dedicated GPU, make sure your gamemode command is written before `%command%` just like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### 4- Lutris/Heroic Games
- **Lutris**: On the left side bar, point your mouse cursor on `Wine`, click on the **gear icon** that appeared.
	- Go to `System Options` and turn on the `Advanced` option, now scroll down a bit. You should turn on the `Use Discrete Graphics` option, after that, make sure you've picked your dedicated GPU's API on `Vulkan API` section. That's all you should do! Make sure to save changes.
 - **Heroic**: On your library, right click on your game and go to `Settings`, in the opened window, check `Use Dedicated Graphics Card` option. That's all you should do!
# Conclusion
After reading this guide, you might want to check [game-specific installation and optimization guides](https://github.com/cutiepenguins/Linux-Gaming-Guide/tree/main/Game%20Specific%20Guides) in case you'd like to play one of those games. Thank you for reading, have a nice day! 🐧
