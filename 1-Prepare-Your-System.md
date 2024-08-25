# Prepare Your System
- First of all, I would like to explain to you how running Windows games on Linux works.
	- Simply, WINE (a compatibility layer) is directing Windows library files into Linux library files
	- Second, DXVK technology is translating DirectX (Windows-specific) calls into Vulkan (Windows/Linux native) or OpenGL if you don't have Vulkan drivers to make Windows games run on Linux.
- To prepare our system for gaming on Linux, we have to know what do we need to know first.
	- First thing we need to know is that if you have an NVIDIA GPU, things you should do is *a bit harder* than having and Intel/AMD GPU because NVIDIA doesn't want to support Linux at all. This was [Linus Torvalds' respond to NVIDIA for not supporting Linux](https://www.youtube.com/watch?v=_36yNWw_07g).
	- Second thing we need to know is that you **must have** a Vulkan capable GPU which all modern GPUs already support. So, if you have a very old GPU, there's a chance it doesn't support vulkan which is not good. You can still play windows games on Linux if you don't have a Vulkan capable GPU but in this case, DirectX calls will be translated to OpenGL instead of Vulkan which you'll experience lots of poor performance issues.
- We only need to apply 3 steps:
	- **1-Installing Vulkan Drivers**
	- **2-Installing Wine and Wine Dependencies**
	- **3- Installing Gaming Software :)**
## Installing Vulkan Drivers
- If you are using an NVIDIA GPU, the best performant way is to install the **proprietary** driver from your package manager.
- If you are using an Intel or AMD GPU, the best performant way is to install the **open-source** driver from your package manager.
- Both ways are explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you don't see your distribution in the link, that means either your distribution's package manager does not include vulkan drivers or vulkan drivers are included preinstalled in your system such as [Fedora did for Mesa drivers](https://packages.fedoraproject.org/pkgs/mesa/mesa-vulkan-drivers/).

## Installing Wine and Wine Dependencies
- First of all, if you're going to install your gaming software ([Lutris](https://lutris.net/), [Steam](https://store.steampowered.com/), [Heroic](https://heroicgameslauncher.com/) etc.) from [Flatpak](https://www.flatpak.org/), then you can skip this step as flatpak will already install them with wine and its dependencies.
- This step is explained in [Lutris' Guide](https://github.com/lutris/docs/blob/master/WineDependencies.md)

## Installing Gaming Software
- You just completed the hardest steps! Now it's time for the last and the easiest step. Install your favourite gaming software!
- Some gaming software you might be interested in:
	- **Steam**: Steam is natively supported on Linux
	- **Heroic Games Launcher**: Heroic is made for installing and playing your favourite games in Epic Games and GOG.
	- **Lutris**: Lutris is made for installing and playing your favourite Windows games.
		- You can search for your games in the app to see if there is an already made script to install and configure your game automatically.
		- You can install your games manually. You can also install your games via DVD.
		- You can install your pirated games if you have setup files.
	- **Protonup-QT**: You can install custom Wine/Proton builds for a better gameplay that are supported by Lutris, Steam and Heroic.
	- **ProtonDB (This is not a software)**: ProtonDB is a website where you can check if your Windows games on Steam are playable on Linux.
		- If your game is ranked as silver or lower, that means it is not supported or unplayable
		- You can also get optimization tips if other reviewers wrote any.
		- You can also write your own review for any Steam game after logging in via your Steam account.