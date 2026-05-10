# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md#before-starting)
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md#get-started)
  - [Graphics Rules Maker Setup](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md#graphics-rules-maker-setup)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md#conclusion)

# Before Starting
> [!NOTE]
> - You can now purchase **The Sims™ 2: Legacy Collection** from various gaming platforms **without the need of any tweaks**. However, this guide is written for **The Sims 2: Ultimate Collection**.
> - **The Sims 2: Ultimate Collection** is abandonware, which means it is **legally unobtainable**. So, you should either have the **setup file** or **the DVD** to install the game.
> - If you are ready, let's begin!
# Get Started
- First of all, **extract the files** from your DVD into a folder and **launch Lutris**.
- `(+)` **-** `Install a Windows game from an executable` **-** `Game name: The Sims 2` **-** `Continue until the "Select the setup file" step` **-** `Select the setup file` **-** `Complete the installation`
- After **the installation has completed**, make sure the game is **located correctly**. To do so, open Lutris and:
  - `Right click The Sims 2` **-** `Configure` **-** `Game Options` **-** `Executable`
    - The location is generally `~/Games/the-sims-2/drive_c/Program Files (x86)/The Sims 2 Ultimate Collection/The Sims 2 Mansion and Garden Stuff/TSBin/Sims2EP9.exe` 
## Graphics Rules Maker Setup
- To **prevent or fix compatibility issues**, you should install [Graphics Rules Maker](https://www.simsnetwork.com/tools/graphics-rules-maker).
- After downloading Graphics Rules Maker, launch Lutris and follow the steps below:
  - `Select The Sims 2` **-** `Click the triangle icon next to WINE icon below` **-** `Run EXE inside Wine prefix` **-** `Select the GRM setup file and launch the app after installation`
<img width="299" height="390" alt="image" src="https://github.com/user-attachments/assets/62907f66-32be-4911-93c3-6aac8aa4d8cf" />


  - `Game: The Sims 2` **-** `Auto-detect` **-** `Force texture memory: 2048 (Intel GPUs only, do not touch it if you use NVIDIA/AMD)` **-** `Save Files`
  - `Game: The Sims 2 Body Shop` **-** `Same steps above` **-** `Save Files`
> [!NOTE]
> - If you have **two GPUs**, make sure Lutris is running Graphics Rules Maker through your **dedicated GPU**, you can check my [Linux Gaming Guide](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#hybrid-graphics-setup) to see how to play games through your dedicated GPU.
>    - I suggest that you read **the whole guide** for optimization tips.
- Now you are ready to play The Sims 2!
# Conclusion
This guide was about The Sims 2 installation and optimization! I hope the guide has been useful. Thank you for reading, happy gaming!
