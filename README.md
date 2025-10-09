# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#before-starting)	
 	- [How Does Linux Gaming Work?](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#how-does-linux-gaming-work) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />
  	- [Warning for NVIDIA Users](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?search=1#warning-for-nvidia-users-) <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/675b9126-59e6-4fbf-af53-1a023465daf7" />
	- [Issues of Linux Gaming](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#issues-of-linux-gaming) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?search=1#get-started)
	- [Installing Vulkan Drivers](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
	- [Installing Gaming Software](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
	- [Hybrid Graphics Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#hybrid-graphics-setup) <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/e08c4e5e-47c8-40cc-81f6-cfabb2829198" /> <img width="16" height="32" alt="nvidia" src="https://github.com/user-attachments/assets/13d0a891-100e-45d2-a579-cb3a76a5da06" />
		- [Ways to Run Games through the Dedicated GPU](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#ways-to-run-games-through-the-dedicated-gpu)
	- [External Disk Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#external-disk-setup)
 		- [Get Started: GParted](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#get-started-gparted-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8119e97a-f45c-4859-bbf2-2b9b26b542a5" />
   		- [How to Configure External Disks on Linux?](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-to-configure-external-disks-on-linux)
	- [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#optimization-tips)
 		- [Reducing Game Resolution and Using the Lowest Graphics Settings](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#reducing-game-resolution-and-using-the-lowest-graphics-settings)
   			- [Lossless Scaling](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#lossless-scaling-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" />
  		- [Using a Performance Kernel](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#using-a-performance-kernel)
		- [Gamemode](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#gamemode)
		- [Performance-Increasing Launch Options](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#performance-increasing-launch-options)
			- [How Can You Use These Launch Options?](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-can-you-use-these-launch-options)
		- [Disabling Compositor](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#disabling-compositor---x11-only-)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#conclusion)
## Game-Specific Guides
- <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> **Minecraft -** [Minecraft Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/35809d93-5960-4e2b-bc5d-2639cb667c04" /> **The Sims 2 -** [The Sims 2 Linux Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
## Türkçe Çeviri 🇹🇷
Rehberin [Türkçe çevirisi buradadır](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md). Birebir çeviri değildir fakat içerik aynıdır.
# Linux Gaming Guide
Hello! This guide aims to help you understand **how gaming on Linux works**, **how to prepare your system for gaming** and **how to optimize your system for higher performance**. If you are ready, let's begin!
# Before Starting
- Linux gaming is **swiftly improving**. Every passing day, more users switch to Linux. In this context, the **market share** of Linux gaming is **increasing**.
- This guide aims to be useful for everyone who wants to **play games** on Linux but **does not know** where to start.
- After reading this guide, feel free to check out [Game-Specific Guides](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#game-specific-guides) if any of the listed games interest you.
## How Does Linux Gaming Work?
- You can play **most of the Windows games** on Linux. However, this **does not mean** that there are **no native Linux games**. **Some native Linux games** are:
	- <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/79d93d2e-2f58-4575-b2f9-f7fc66d0b0cd" /> Terraria, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/791afaf0-7f92-486e-8e2b-baeaf54155f9" /> Stardew Valley, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/bf7d4ca4-aedf-460e-819d-6f8d6a8475d3" /> Euro Truck Simulator 2 and more
 	- **Valve games** such as <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/c4e6099e-6a55-488a-b6d8-397bfeec0e20" /> Counter-Strike series, <img width="16" height="25" alt="tf2" src="https://github.com/user-attachments/assets/4efb907f-63e4-41bd-aa55-ca37674d5304" /> Team Fortress 2, <img width="16" height="25" alt="dota" src="https://github.com/user-attachments/assets/b62be047-0b56-4684-b135-80754c18063b" /> Dota 2, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e33b1a9c-fff9-4112-96a6-99499020f84a" /> Portal etc.
- Generally, native Linux games **do not require** any extra steps **unless they do not require Vulkan**. If they do, you need to **install Vulkan drivers** which is explained in this guide.
- Windows games require some **essential tools** in order to run on Linux and these tools are:
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> [WINE](https://www.winehq.org/) / [Proton](https://github.com/ValveSoftware/Proton) **-** WINE is a compatibility layer which directs **Windows library files** into **Linux library files**. It works the same as the **compatibility mode on Windows**.
 		- Proton is Valve's **fork** of <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE and it is **specifically configured for <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam games**.
	- [DXVK](https://github.com/doitsujin/dxvk) **-** DXVK translates **DirectX 8-11** calls into **Vulkan** to make Windows games run on Linux. DXVK is **not included** in <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE but you still **do not need to install DXVK manually** because **most** of the **Linux gaming software** and **custom <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton builds** include DXVK for users.
		- There are some **other tools** that are used for **similar purposes** as DXVK, these tools are:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d) **-** VKD3D translates **DirectX 12** calls into **Vulkan** which DXVK cannot yet. VKD3D **serves as the fallback** if the game you are trying to play is a **DirectX 12 game**. Just like DXVK, VKD3D is **automatically included** in **most** of the **Linux gaming software** and **custom <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton builds**.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d) **-** WINED3D translates **DirectX 8-11** calls into **OpenGL instead of Vulkan**. WINED3D **serves as the fallback** if your system **does not have Vulkan drivers installed**. However, since DirectX calls will be translated into OpenGL, you are likely to experience **poor performance** because OpenGL is **deprecated**. **Unlike** DXVK and VKD3D, WINED3D is **included** in <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE.
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
- You **do not need to manually install** <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE because <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE is installed **automatically** when you install a gaming software such as <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris.
## Warning for NVIDIA Users <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" />
- <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA is **phasing out** the **proprietary** drivers for their **4xxx** and **5xxx** series because <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA is attempting to be **more open source** for their **recent and future cards**. However, **for older cards**, you still have to use **proprietary** drivers for **better compatibility and performance**.
- Also, you **should not use** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland **unless** you use one of the recent <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA GPUs that are mentioned above because it is likely for you to experience **glitches and performance issues**. Using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" /> X11 is a **better option** for now.
## Issues of Linux Gaming
- There are **not too many issues** when it comes to gaming on Linux. However, the **main limitation** is **kernel-level anti-cheat software**. These anti-cheat software **are not able to run** on Linux.
	- The reason why is a kernel-level anti-cheat software that is developed for a Windows game means that the anti-cheat software **requires a kernel called "Windows NT", which is only available for Windows**.
- Some examples of kernel-level anti-cheat software are:
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> **| VANGUARD**
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc19a74e-ff75-40dc-9976-50e61be8c4ab" /> **| Easy Anti-Cheat**
	- <img width="13" height="25" alt="image" src="https://github.com/user-attachments/assets/1d9704a0-13ba-4f8d-ada3-ad438abce41c" /> **| BattlEye**
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/e05603e5-219b-4ecd-8b5f-f1c9ea6ad077" /> **| XIGNCODE3**
	- <img width="16" height="25" alt="nprotect" src="https://github.com/user-attachments/assets/b2840543-d490-4012-85b6-5647ca747dab" /> **| nProtect GameGuard**
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc19a74e-ff75-40dc-9976-50e61be8c4ab" /> **Easy Anti-Cheat** and <img width="13" height="25" alt="image" src="https://github.com/user-attachments/assets/1d9704a0-13ba-4f8d-ada3-ad438abce41c" /> **BattlEye** have **Linux-compatible** versions. That's why some developers **may enable Linux compatibility** with their anti-cheat software **specifically for <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton**.
	- However, **some developers** of games like <img width="13" height="25" alt="fortnite" src="https://github.com/user-attachments/assets/17d24518-9a9e-4fa0-a075-24f88e42fa89" /> Fortnite and <img width="16" height="25" alt="apexlegends" src="https://github.com/user-attachments/assets/1e092ebc-e76d-46b2-90b4-e08d7efcd836" /> Apex Legends **do not enable** Linux support in their anti-cheat configurations. That's why **those games cannot run on Linux**.
- In addition to enabling Linux-compatible configurations, some games only use the **user-mode module** of these anti-cheat software, which **makes them playable** on Linux.
- **Except <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD**, we **cannot** make a **definitive statement** about **playability** of a game that uses one of the anti-cheat software mentioned above.
	- The case is **different for <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD** because **no games** using <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD are able to run on Linux. This is because <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD is only used by the games of <img width="16" height="25" alt="rito" src="https://github.com/user-attachments/assets/06511a6d-3434-4ae0-be6d-a4d5e0f6c8c8" /> Riot Games, which **do not intend to support** Linux players at all.
# Get Started
## Installing Vulkan Drivers
- This step is explained in <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> [Lutris' Community Guide](https://github.com/lutris/docs/blob/master/InstallingDrivers.md).
- If you **cannot see your Linux distribution** in the page, that probably means Mesa **(the default <img width="16" height="25" alt="intel" src="https://github.com/user-attachments/assets/262e5a2c-6c88-4e6f-a0d1-d8428fb16504" /> <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> Intel/AMD GPU driver)** Vulkan drivers are **preinstalled** on your Linux distribution.
	- However, if you **cannot** see your distribution in the page and if you are using <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> **NVIDIA**, I suggest that you find a **different documentation** for installation steps or **switch to one of the distributions** that are mentioned in the page.

## Installing Gaming Software
- Some popular gaming software that are available on Linux are:
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> **|** [Steam](https://store.steampowered.com/)
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **|** [Heroic Games Launcher](https://heroicgameslauncher.com/) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic is a useful game launcher for playing games from **<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7ce5f2d5-e927-4712-ad11-5a4df8281adb" /> Epic Games, <img width="16" height="25" alt="gog" src="https://github.com/user-attachments/assets/552536c7-c66d-42ca-8b43-239bff63d887" /> GOG and <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f18ba3ba-4418-4153-9201-7f2b1ca4b42f" /> Prime Gaming** platforms.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **|** [Lutris](https://lutris.net/) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris is a feature-rich game launcher **for playing Windows games**. You can **directly** install some gaming software platforms such as **<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7ce5f2d5-e927-4712-ad11-5a4df8281adb" /> Epic Games, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/93fec16e-9461-4b36-a47c-8242e6259f94" /> Battle.net, <img width="16" height="25" alt="ubisoft" src="https://github.com/user-attachments/assets/5980423e-e2ca-407a-89a5-183715ac83fc" /> Ubisoft etc.** and run them using Lutris but you can also play games that are not tied to a certain platform.
		- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris provides **community-made installation scripts** for a **large number** of games and software.
		- You can also install your games **manually**, including **DVD games**, if you have the setup files.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/86fe080b-77b7-4bc1-9fa5-1afc7eebc39d" /> **|** [ProtonPlus](https://protonplus.vysp3r.com/) **-** You can install **custom <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton builds** for **better compatibility** and **performance** using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/86fe080b-77b7-4bc1-9fa5-1afc7eebc39d" /> ProtonPlus. Custom <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton builds **are supported** by <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam and <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> **|** [Sober](https://sober.vinegarhq.org) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> Sober is a game launcher for playing <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/26dec68d-79c7-4f82-875a-ab1a21bb11f5" /> **Roblox's** <img width="16" height="25" alt="image-removebg-preview(1)" src="https://github.com/user-attachments/assets/cec27060-1d67-48e1-8f29-a3a5b639fde8" /> Android version on Linux. In the past, it was possible to run the Windows version of <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/26dec68d-79c7-4f82-875a-ab1a21bb11f5" /> Roblox through <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/2e1571a7-9ec9-42eb-8238-c6931941b506" /> **VinegarHQ**. However, it is **borked** now due to the **anti-cheat configuration**. That's why <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> **Sober** is developed by the same team.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> [Prism Launcher](https://prismlauncher.org) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher is a feature-rich game launcher for playing <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> **Minecraft**.
 		- I have a <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> [Minecraft guide](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md) for configuring and optimizing Minecraft, if you are interested.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/92f8c7dc-7a41-4a92-bc71-0d69bd2d22b9" /> [Waydroid](https://waydro.id/) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/92f8c7dc-7a41-4a92-bc71-0d69bd2d22b9" /> Waydroid is is a **container-based compatibility layer** that **allows <img width="16" height="25" alt="image-removebg-preview(1)" src="https://github.com/user-attachments/assets/cec27060-1d67-48e1-8f29-a3a5b639fde8" /> Android to run on Linux**. So you can play <img width="16" height="25" alt="image-removebg-preview(1)" src="https://github.com/user-attachments/assets/cec27060-1d67-48e1-8f29-a3a5b639fde8" /> Android games on Linux using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/92f8c7dc-7a41-4a92-bc71-0d69bd2d22b9" /> Waydroid.
 		- I have a <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/92f8c7dc-7a41-4a92-bc71-0d69bd2d22b9" /> [Waydroid guide](https://github.com/cagla-su/Waydroid-Guide) for your questions in mind, installation and configuration steps, if you are interested.

### ⚠️
- You can install these software through either your **package manager** or [Flatpak](https://flatpak.org).
- You can check <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1ee2ed23-e831-463b-8ada-87e8cd5d4fc7" /> [ProtonDB](https://www.protondb.com) to see whether your <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam games are playable on Linux.
	- If the game you searched is ranked **lower than silver**, that means it is **unplayable**.
	- You can get **optimization tips** if there are any reviews written for your game. If you wish, you can write your own reviews for any <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam game you wish.
# Hybrid Graphics Setup
- If your system has **two GPUs (1 integrated + 1 dedicated)**, it is recommended to **install Vulkan drivers for both hardware** and set games to run through your dedicated GPU.
- To run games using your dedicated <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> **AMD** GPU, use the following command:
```
DRI_PRIME=1
```
 - To run games using your <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/cf335904-bc37-427e-a86d-c7f9df4bd852" /> **NVIDIA** GPU, use the following command:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Ways to Run Games Through the Dedicated GPU
- There are **four ways** of running games through your dedicated GPU:
	- **1 -** [Terminal Method](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#terminal-method-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/ae34a1ca-71fe-4bf4-b1df-ddee947edaf5" />
 	- **2 -** [Desktop Shortcut Method](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#desktop-shortcut-method-%EF%B8%8F) 🖥️
 	- **3 -** [For Steam Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" />
  	- **4 -** [For Lutris & Heroic Games](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-lutris--heroic-games--) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
### Terminal Method <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/814656ce-8cb1-4f5d-bf18-ab56736dc781" />
Simply, launch terminal and execute the command for your GPU like in the example:
```
DRI_PRIME=1 prismlauncher
```
### Desktop Shortcut Method 🖥️
- Create a **.desktop** file on your desktop.
- This is an example .desktop file content to run <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher through an <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA GPU. The line you should pay attention is the line that starts with `Exec`:
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
### For Steam Games <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" />
Add the command for your GPU in the launch options of your games. **Do not forget** to add `%command%` at last like in the example:
```
DRI_PRIME=1 %command%
```
- **⚠️ -** If you are going to **additionally** use other launch options and run games through your dedicated GPU, make sure that all the commands are written **before** `%command%` like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### For Lutris & Heroic Games <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **| Lutris -** On the left side bar, click the **settings icon** that appears when you point your mouse cursor on `Wine`.
	- `System Options` **-** `Enable Advanced` **-** `Use Discrete Graphics`
 - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **| Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# External Disk Setup
- If your external disk is **internally connected**, you might be able to use it **out of the box** depending on your Linux distribution. However, if you are using your external disk **through an SSD case (USB)**, you should configure it manually.
- These steps also apply if your disk is **internally connected** but still **not working properly**.
## Get Started: GParted <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8119e97a-f45c-4859-bbf2-2b9b26b542a5" />
⚠️ - I **strongly suggest** that you **format your disk** to change its file system from **NTFS** to a **Linux-compatible one** because **write support for NTFS** is **experimental** on Linux and it **might corrupt** your drive!!! You have been warned.
- Install `gparted` using your package manager and follow the next steps, **making sure** your external disk is **unmounted** while it is **physically connected**.
	- `Launch GParted` **-** `select your external disk from the top right` **-** `delete all the partitions` **-** `Add`
 	- **Next -** `File system: ext4` **-** `Label: anything you wish` **-** `Add`
  	- **Finally -** `Apply All Operations`
## How to Configure External Disks on Linux?
- First of all, install `gnome-disk-utility` package using your package manager.
	- If you **insist** about using your external disk **as NTFS** anyway, additionally install `ntfs-3g` package using your package manager.
- After the installation, launch `Disks` app from your application launcher.
- Then, find your external disk from the menu on the left and click this button under `Volumes`:
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- From the menu, click `Take Ownership` and confirm.
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
- When you reduce the resolution of a game, **less pixels will be rendered** and it will result in **less loads** on your hardware, leading to **higher performance**.
- When you play with the lowest graphics settings, **less details will be rendered**, leading to **higher performance**.
- Both are going to **increase performance** while **reducing visual quality**. You can experiment to find your own balanced settings.
### Lossless Scaling <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" />
It is possible to play your games in **lower resolutions** while **not losing anything from visual quality** thanks to <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" /> [Lossless Scaling](https://store.steampowered.com/app/993090/Lossless_Scaling/). However, you **must purchase** the app from <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam to be able to use it.
- After purchasing <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" /> Lossless Scaling, you should **install [lsfg-vk](https://github.com/PancakeTAS/lsfg-vk)** to be able to use it on Linux.
	- However, your **GPU must support Vulkan** and your **system must have Vulkan drivers installed** in order to use this feature!
## Using a Performance Kernel
**Up-to-date kernels** generally **perform well** compared to custom performance kernels. However, you can still try a custom performance kernel, in case **it might perform better**.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/943b4b7c-5b29-46aa-b081-b5d5ecc8fec3" /> **| Arch Linux and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/48e91252-38ca-4a48-80b8-57423b90c5da" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/95bc6c6d-7d21-4c3a-ac08-31c85ddf8683" /> **| Fedora Linux and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/a3d38d39-481b-4436-b22b-b877acc4a6ea" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/c56a6d0a-133d-4bcf-a594-f4cd8b58e335" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7960ea90-ac89-4e3a-9839-cd77f9ec2b24" /> **| Debian/Ubuntu Linux and Derivatives:** [XanMod Kernel](https://xanmod.org/) <img width="16" height="25" alt="xanmod" src="https://github.com/user-attachments/assets/d3afbdc8-439a-426b-b5b1-9206f03fea05" />
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a tool that **temporarily changes** your **system configurations** to increase performance during the gameplay.
	- Generally, gaming software like <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris **enable it by default**. But on <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam, you should **manually add a command** in your game's launch options like in the example:
```
gamemoderun %command%
```
## Performance-Increasing Launch Options
You can use these launch options for higher performance while gaming:
- `DXVK_LOG_LEVEL=none` **-** It **suppresses all DXVK logs** to increase performance as gaming software **will not spend time processing and writing log data**. - *Medium impact on performance*
- `WINEDEBUG=-all` **-** It **suppresses all debug outputs of <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE**. - *Low impact on performance*
- `WINE_LARGE_ADDRESS_AWARE=1` **-** It **allows 32-bit applications to consume up to 4 GB RAM instead of 2 GB**. - *Variable impact depending on the game, generally medium.*
- `MESA_GLTHREAD=true` **-** It improves **OpenGL performance** on <img width="16" height="25" alt="intel" src="https://github.com/user-attachments/assets/315abff4-87d6-4779-b38d-08f07b8237a4" /> <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> **Intel/AMD GPUs**. - *High impact on performance*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** It improves **OpenGL performance** on <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/cf335904-bc37-427e-a86d-c7f9df4bd852" /> **NVIDIA GPUs**. - *High impact on performance*
- `DXVK_ASYNC=1` **-** It **displays frames without waiting for shaders to be compiled**. - *Variable impact depending on the game, generally low.*
	- It works on <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris and <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic while it **does not work on <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam games**.
 	- Additionally, using DXVK Async can **get you banned from online games**. That's why, it is only recommended for **offline games**. 
### How Can You Use These Launch Options?
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> **| Steam -** You can simply use these commands in launch options section that is [previously mentioned](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games-).
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **| Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />

- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **| Heroic -** `Settings` **-** `Game Defaults` **-** `ADVANCED` **-** `Environment Variables` **-** `+`
<img width="513" height="180" alt="image" src="https://github.com/user-attachments/assets/557adebe-23e7-4c8b-93e2-0378cb38faae" />

## Disabling Compositor - X11 ONLY!!! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" />
**⚠️ -** If you are using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland, disabling the compositor is **not possible**. These steps are only available for <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" /> X11.
- A disabled compositor **simply means disabled animations and transparency**. Also, it causes screen tearing which **reduces visual quality while improving performance**.
- This step is explained in <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" /> [Linux Gaming wiki](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)).
# Conclusion
This guide was about Linux gaming. Thank you for reading. I hope this guide has helped you prepare your system for gaming on Linux. Happy gaming! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />

