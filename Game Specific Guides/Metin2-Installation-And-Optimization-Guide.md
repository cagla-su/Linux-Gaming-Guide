# Metin2
Metin2 is an old legendary MMORPG game.
## Get Started
- First of all, make sure your system is prepared for gaming following [my guide](https://github.com/cutiepenguins/Linux-Gaming-Guide).
- Now, we are going to be using **Lutris** to install and play Metin2. There is a Lutris script for **Gameforge Client** which means it is easier to install than it is expected.
- However, if you are playing Metin2 mainly with **multiple sections**, you might want to install the client **twice** or even **thrice** according to how many sections you are running simultaneously.
    - It is because Gameforge Client runs buggy on Linux. When you launch the game more than twice on the same client, it doesn't let you launch any more clients due to the bug.
## Install Gameforge Client
- **Step 1**: Open `Lutris` (surprisingly)
- **Step 2**: Click the `Plus (+)` button on the top left.
- **Step 3**: Click `Search the Lutris website for installer` and type gameforge.
- **Step 4**: Now, install the `Gameforge Client` script.
- **Step 5**: Apply the same steps for the **second (or/and third)** client I suggested you to install. Simply install it again but make sure you changed the folder name in the `Select installation directory` step.
## Installing Metin2
Installing Metin2 is not hard. Simply log in and install Metin2. However, the installer will be stuck at 95%, 97% etc. and in this case, all you have to do is stop Gameforge Client from Lutris. When you launch the client again, you are going to see that the game is installed successfully. Also, once you launch the game and shut it down, you will see that your game account is stuck at `in-game` sign due to the bug.
## Optimize Metin2
- **Step 1:** You might prefer using **wine-ge** build that is preinstalled with the client. However, if you want to get better performance specifically on Metin2, I suggest you to install the **latest stable custom WINE build** [from the link](https://github.com/Kron4ek/Wine-Builds/releases) and extract the folder to `~/.local/share/lutris/runners/wine/`.
    - If you are using Lutris from Flatpak, the location is `~/.var/app/net.lutris.Lutris/runners/wine`.
- **Step 2:** Open your file manager and follow the directory:
`~/Games/gameforge-client/drive_c/your-games-location/metin2/en-GB(or another code for your server)/bgm`
    - After reaching `bgm` folder, delete everything in the folder permanently, don't delete the folder itself, only delete the files inside. You just deleted the music files that run in the background while playing which are **CPU-intensive** and might reduce performance.
    - Now go back to `en-GB` folder. Then, delete `logo1.avi` and `logo2.avi`.
    - Open `config.exe` once and click `OK`, this will create `metin2.cfg`. Now open `metin2.cfg` via a text editor.
    - `Width` **:** `1280`
    - `Height` **:** `720`
    - `BPP` **:** `16`
    - `PRE_LOADING_DELAY_TIME` **:** `0`
      - *save the file*
    - Don't forget to apply the same steps for the other client(s).
### Optimize In-Game Settings
You are ready to play after changing some in-game settings for high performance.
- **System Options**
  - **System Tab**
    - `View Distance` **:** `1`
    - `Fog` **:** `Off`
    - `Snowfall` **:** `Off`
    - `Snow` **:** `Off`
    - `Target Shadow` **:** `1` - **or** `2` **if you'd like**
    - `Private Shops` **:** `5` - **or** `3` **if you'd like**
    - `Item Drops` **:** `2 - Yang enabled`
  - **Game Tab**
    - `Name` **:** `Subjective`
    - `Monster info` **:** `Level (uncheck)`
    - `Animations` **:** `Performance`
    - `Show` **:** **Uncheck** these options:
      - `Chat Line`
      - `Shop name`
      - `Monster Names` - **keep it enabled if you'd like**
      - `HP Bar`
# Conclusion
I hope this guide helped you to play Metin2 on Linux with optimized settings! Have a nice day! 🐧
