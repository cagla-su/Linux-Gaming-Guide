# Things You Should Know Before Starting
- First of all, I would like to explain to you how running Windows games on Linux works.
	- Firstly, [WINE](https://www.winehq.org/) (a compatibility layer) is directing Windows library files into Linux library files
	- Lastly, [DXVK technology](https://github.com/doitsujin/dxvk) is translating DirectX (Windows-specific graphics library) calls into Vulkan (Windows/Linux native graphics library) or OpenGL if you don't have Vulkan drivers to make Windows games run on Linux.
- Now, let's see what we need to know!
	- First thing we need to know is that if you have an **NVIDIA GPU**, things you should do will be *a bit harder* because NVIDIA doesn't want to support Linux at all. This was [Linus Torvalds' response to NVIDIA for not supporting Linux](https://www.youtube.com/watch?v=_36yNWw_07g) :)))
	- Second thing we need to know is that you **must have** a Vulkan capable GPU which all modern GPUs already support. So, if you have a very old GPU, it probably doesn't support Vulkan which is not good for performance.
 	- You can still play windows games on Linux if you don't have a Vulkan capable GPU but in this case, DirectX calls will be translated into OpenGL instead of Vulkan which means you're going to experience lots of performance issues.
## Get Started
- We only need to apply 3 steps:
	- **1- Installing Vulkan Drivers**
	- **2- Installing Wine and Wine Dependencies**
	- **3- Installing Gaming Software :)**
### Installing Vulkan Drivers
- If you are using an **NVIDIA GPU**, the best performant way is to install the **proprietary** driver from your package manager.
- If you are using an **Intel/AMD GPU**, the best performant way is to install the **open-source** driver from your package manager.
- Both ways are explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you don't see your distribution in the link, that means either your distribution's package manager does not include Vulkan drivers or Vulkan drivers are included preinstalled in your system such as [Fedora did for Mesa drivers](https://packages.fedoraproject.org/pkgs/mesa/mesa-vulkan-drivers/).

### Installing Wine and Wine Dependencies
- First of all, if you're going to install your gaming software from [Flatpak](https://www.flatpak.org/), then you can skip this step as Flatpak will already install them with wine and its dependencies.
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/WineDependencies.md)

### Installing Gaming Software
- You just completed the hardest steps! Now it's time for the last and the easiest step. Install your favourite gaming software!
- Some gaming software you might be interested in:
	- [Steam](https://store.steampowered.com/): Steam is natively supported on Linux
	- [Heroic Games Launcher](https://heroicgameslauncher.com/): Heroic is made for installing and playing your favourite games in Epic Games and GOG.
	- [Lutris](https://lutris.net/): Lutris is made for installing and playing your favourite Windows games.
		- You can search for your games in the app to see if there is an already made script to install and configure your game automatically.
		- You can install your games manually. You can also install your games via DVD.
		- You can install your pirated games if you have setup files.
	- **Protonup-QT**: You can install custom Wine/Proton builds for a better gameplay that are supported by Lutris, Steam and Heroic.
### Notes
- You can install these software from either your package manager or Flatpak.
- If you're using [CachyOS](https://cachyos.org/) or if you have [CachyOS repositories](https://github.com/CachyOS/linux-cachyos#cachyos-repositories) enabled in your Arch system, you can install [cachyos-gaming-meta](https://github.com/CachyOS/CachyOS-PKGBUILDS/blob/master/cachyos-gaming-meta/PKGBUILD) package to install all the necessary gaming components.
- You can use [ProtonDB](https://www.protondb.com/) is a website that allows you to check whether your Windows games on Steam are playable on Linux.
	- If your game is ranked as silver or lower, that means it is not supported or unplayable.
	- You can get optimization tips if other reviewers wrote any.
	- You can write your own review for any Steam game after logging in via your Steam account.
