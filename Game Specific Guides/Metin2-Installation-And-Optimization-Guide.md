# Metin2
## Get Started
- First of all, make sure your system is prepared for gaming following [my guide](https://github.com/cutiepenguins/Linux-Gaming-Guide).
- The software that will be guided in this guide is **Lutris**.
- If you are playing Metin2 mainly with **multiple sections**, you might want to install the client on Lutris **twice** or even **thrice** according to how many sections you are running simultaneously.
    - It is because Gameforge Client runs buggy on Linux. When you launch the game multiple times in the same client, it does not let you launch any more sections which gives you no choice but killing Gameforge Client from Lutris, which also will kill all the running Metin2 sections of the same client. To prevent such issues, installing the client multiple times is helpful. 
## Install Gameforge Client
- **Step 1**: Open `Lutris` (surprisingly)
- **Step 2**: Click the `(+)` button on the top left.
- **Step 3**: Click `Search the Lutris website for installer` and type gameforge.
- **Step 4**: Now, install the `Gameforge Client` script.
- **Step 5**: Apply the same steps for the **second (or/and third)** client(s) I suggested you install. But make sure you changed the folder name in the `Select installation directory` step before the installation of the other client(s).
- **Step 6 - For Turkish Players Only**: For Turkish keyboard layout, you should add an environment variable after installing the client. Otherwise, you will be able to see the special characters like `ğ,ş,İ,ı` texted by other players on your screen but when you try to use the same letters, you will see `g,s,I,i` as the output.
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
    - All you have to do is **right clicking Gameforge Client** in Lutris library and changing **Wine version** to **"GE-Proton (Latest)"** in `Runner options`.
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
