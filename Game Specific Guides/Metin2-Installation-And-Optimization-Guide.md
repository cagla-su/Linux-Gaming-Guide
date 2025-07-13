# Metin2
## Get Started
- First of all, make sure your system is prepared for gaming following [my guide](https://github.com/cutiepenguins/Linux-Gaming-Guide).
- The software that will be guided in this guide is **Lutris**.
- Gameforge Client is buggy on Linux. However, a new tool called [umu-launcher](https://github.com/Open-Wine-Components/umu-launcher) **solves almost all compatibility issues** such as making the **game font better aligned**, letting you **launch as much as game sections you want under the same client** and fixing the bug where **item shop is unable to function after teleporting**. The steps are explained in [optimization section](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md#optimize-metin2).
    - In optimization section, an **alternative** is also explained in case **UMU may not work** on your system. If UMU **does not work** on your system and you have to use the alternative Wine build, you are going to be **unable** to launch more than **two, or sometimes three,** sections under the same client. That's why you should install Gameforge Client **twice** or even **thrice** in Lutris.
## Install Gameforge Client
- `Lutris` **-** `(+)` **-** `Search the Lutris website for installer` **-** `Search and install Gameforge Client script` **-** `Right click Gameforge Client` **-** `Configure` **-** `Game options` **-** `Change "Prefix architecture" value to 64-bit`
- **For different keyboard layouts that do not work properly in game :** `Right click Gameforge Client` **-** `Configure` **-** `System options` **-** `Environment variables` **-** `Add`
<img width="811" height="252" alt="image" src="https://github.com/user-attachments/assets/6573cf94-d306-43cc-b545-6cc5b9d27b0c" />

- You can change **tr_TR** value as your keyboard layout's language code.
- If the environment variable did not work on **Fedora Linux**, try installing `glibc-all-langpacks` package.
## Installing Metin2
- After logging in and downloading the game, the installer will be stuck at a certain value like `97%`. In this case, all you have to do is stop Gameforge Client from Lutris. When you launch the client again, you are going to see that the game is installed successfully.
- Once you launch the game and exit, you will see that your game account is stuck at `in-game` sign. You can ignore it as Gameforge Client allows you to run another section from the same game account.
## Optimize Metin2
- `Right click Gameforge Client` **-** `Runner options` **-** `Change Wine version as "GE-Proton (Latest)"`
    - However, if UMU (`GE-Proton (Latest)`) does not work properly for you, you can prefer [this custom WINE build](https://github.com/Kron4ek/Wine-Builds/releases) instead. If you do not know which file to download, `wine-X.X-staging-tkg-ntsync-amd64-wow64.tar.xz` is the most performant one.
        - After downloading the custom WINE build, extract the file and move the extracted folder to `~/.local/share/lutris/runners/wine/`. Do not forget to change Gameforge Client's WINE version accordingly.
            - If you installed Lutris from Flatpak, the location is `~/.var/app/net.lutris.Lutris/data/lutris/runners/wine/` for you.
- Open your file manager and follow the directory: `~/Games/gameforge-client/drive_c/Program Files/metin2/en-GB/bgm`
    - The `en-GB` folder's name might be something different if you are playing on another server such as Türkiye (`tr-TR`) server.
    - After reaching `bgm` folder, delete everything in the folder permanently without deleting the folder. This will help with performance as the music files that play in the background while playing the game are **CPU-intensive** and might reduce performance.
    - Go back to `en-GB` folder and delete `logo1.avi` and `logo2.avi`.
    - Open `config.exe` once and click `OK`, this will create `metin2.cfg`.
    - Now edit `metin2.cfg` via a text editor.
        - `Width` **:** `1280`
        - `Height` **:** `720`
        - `BPP` **:** `16`
        - `PRE_LOADING_DELAY_TIME` **:** `0`
### Optimized In-Game Settings You Can Apply
- ![a](https://github.com/user-attachments/assets/92f5060c-eadf-4d70-88e8-11dbf212c6a0)
- ![b](https://github.com/user-attachments/assets/d503705a-d671-476c-9c9a-ae381648c421)
- ![c](https://github.com/user-attachments/assets/c3166494-01e0-4963-8fa4-088f05a08863)
- ![d](https://github.com/user-attachments/assets/8a78ec23-24e4-43da-b764-17d8c03f195d)
# Conclusion
This guide was about Metin2 installation and optimization. I hope the guide has been useful. Thank you for reading, happy gaming! 🐧
