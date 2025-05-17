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
- **Step 1:** You might prefer using **wine-ge** build that is preinstalled with the client. However, if you want to get better performance specifically on Metin2, I suggest you install the **latest stable custom WINE build** [from the link](https://github.com/Kron4ek/Wine-Builds/releases) and extract the folder to `~/.local/share/lutris/runners/wine/`. The file that has **staging-tkg-ntsync-amd64-wow64** in its name is the one that grants the highest performance.
    - If you are using Lutris from Flatpak, the location is `~/.var/app/net.lutris.Lutris/runners/wine`.
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
### Optimize In-Game Settings
- **System Options**
  - **System Tab**
![image](https://github.com/user-attachments/assets/51d573ae-0719-467b-ae0d-9b0bea7df67e)

    - `View Distance` **:** `1`
    - `Fog` **:** `Off`
    - `Snowfall` **:** `Off`
    - `Snow` **:** `Off`
    - `Target Shadow` **:** `1` - **or** `2` **if you would like**
    - `Private Shops` **:** `5` - **or** `3` **if you would like**
    - `Item Drops` **:** `2`
  - **Game Tab**
    - `Name` **:** `Subjective`
    - `Monster info` **:** `Level (uncheck)`
    - `Animations` **:** `Performance`
    - `Show` **:** **Uncheck** these options:
      - `Chat Line`
      - `Shop name`
      - `Monster Names` - **keep it enabled if you would like**
      - `HP Bar`
# Conclusion
This guide was about Metin2 installation and optimization! I hope the guide has been useful. Thank you for reading, have a nice day! 🐧
