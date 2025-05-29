# Metin2
## Get Started
- First of all, make sure your system is prepared for gaming following [my guide](https://github.com/cutiepenguins/Linux-Gaming-Guide).
- The software that will be guided in this guide is **Lutris**.
- Gameforge Client is very buggy on Linux. However, a new technology called [umu-launcher](https://github.com/Open-Wine-Components/umu-launcher) **solves almost all incompatibility issues** such as **making the game font better aligned, letting you launch as much as game sections you want under the same client and fixing item shop being unable to function after teleporting bug**. The installation steps are explained in [optimization](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md#optimize-metin2) section.
    - In optimization section, an alternative is also explained in case UMU may not work on your system. If UMU does not work on your system and you have to use the alternative Wine build, you are going to be **unable** to launch multiple sections under the same client. That's why you should install Gameforge Client **twice** or even **thrice** in Lutris if that is the case for you.
## Install Gameforge Client
- **Step 1**: Open `Lutris` (surprisingly)
- **Step 2**: Click the `(+)` button on the top left.
- **Step 3**: Click `Search the Lutris website for installer` and type gameforge.
- **Step 4**: Now, install the `Gameforge Client` script.
- **Step 5**: **Right click** Gameforge Client in your Lutris library and go to `Configure`.
    - Now go to `Game options` and change `Prefix architecture` value as **64-bit**.
    - Make sure to save the changes.
- **Step 6**: Apply the same steps for the **second (or/and third)** client(s) I suggested you install. But make sure you changed the folder name in the `Select installation directory` step before the installation of the other client(s).
- **Step 7 - For Turkish Players Only**: For Turkish keyboard layout, you should add an environment variable after installing the client. Otherwise, you will be able to see the special characters like `ğ,ş,İ,ı` texted by other players on your screen but when you try to use the same letters, you will see `g,s,I,i` as the output.
    - What you should do is **right click** Gameforge Client in your Lutris library and go to `Configure`.
        - Now go to `System options` and scroll down a bit until you see the `Environment variables` section.
        - In `Environment variables` section, click `Add` and add the environment variable below:
        - `Key:` **LC_ALL** | `Value:` **tr_TR.UTF-8**
        - Make sure to save the changes.
            - Just a little warning for **Fedora** users. If you are unable to use Turkish letters while playing Metin2 even though you applied all the steps properly, it might be because you have a missing package which you can get executing `sudo dnf install glibc-langpack-tr` command in terminal.
## Installing Metin2
- After logging in and downloading the game, the installer will be stuck at a certain value like `97%`. In this case, all you have to do is stop Gameforge Client from Lutris. When you launch the client again, you are going to see that the game is installed successfully.
- Once you launch the game and exit, you will see that your game account is stuck at `in-game` sign. You can ignore it as Gameforge Client allows you to run another section from the same game account.
## Optimize Metin2
- **Step 1:** When you install the client, a **wine-ge** build will be preinstalled and set as the default runner. However, Lutris now supports [umu-launcher](https://github.com/Open-Wine-Components/umu-launcher) so you might want to switch to it for better compatibility and performance. Do not be confused with its name, you will not be installing an application. UMU is a **built-in feature in Lutris**.
    - All you have to do is **right click Gameforge Client** in Lutris library and changing **Wine version** to **"GE-Proton (Latest)"** in `Runner options`.
    - However, if UMU does not work properly for you, you can prefer [this custom WINE build](https://github.com/Kron4ek/Wine-Builds/releases) instead. If you do not know which file to download, `wine-X.X-staging-tkg-ntsync-amd64-wow64.tar.xz` is the most performant one.
        - After downloading the custom WINE build, extract the file and move the extracted folder to `~/.local/share/lutris/runners/wine/` and change the client's Wine version accordingly.
        - If you installed Lutris from Flatpak, the location is `~/.var/app/net.lutris.Lutris/data/lutris/runners/wine/` for you.
- **Step 2:** Open your file manager and follow the directory:
`~/Games/gameforge-client/drive_c/Program Files/metin2/en-GB/bgm`
    - The `en-GB` folder's name might be something different if you are playing on another server such as Türkiye (`tr-TR`) server.
    - After reaching `bgm` folder, delete everything in the folder permanently without deleting the folder. This will help with performance as the music files that run in the background while playing the game are **CPU-intensive** and might reduce performance.
    - Go back to `en-GB` folder and delete `logo1.avi` and `logo2.avi`.
    - Open `config.exe` once and click `OK`, this will create `metin2.cfg`.
    - Now edit `metin2.cfg` via a text editor.
        - `Width` **:** `1280`
        - `Height` **:** `720`
        - `BPP` **:** `16`
        - `PRE_LOADING_DELAY_TIME` **:** `0`
        - *save the file*
    - Don't forget to apply the same steps for the other client(s).
### Optimized In-Game Settings You Can Apply
- ![a](https://github.com/user-attachments/assets/92f5060c-eadf-4d70-88e8-11dbf212c6a0)
- ![b](https://github.com/user-attachments/assets/d503705a-d671-476c-9c9a-ae381648c421)
- ![c](https://github.com/user-attachments/assets/c3166494-01e0-4963-8fa4-088f05a08863)
- ![d](https://github.com/user-attachments/assets/8a78ec23-24e4-43da-b764-17d8c03f195d)
# Conclusion
This guide was about Metin2 installation and optimization! I hope the guide has been useful. Thank you for reading, have a nice day! 🐧
