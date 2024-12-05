# Metin2
Metin2 is an old MMORPG game. Even though it doesn't have players as much as it used to have in the past, I still play it and found ways to optimize it. I don't think any Linux user is playing Metin2 but I still wanted to document it in case there are people thinking of playing it on Linux.
## Get Started
- First of all, make sure your system is ready for gaming following [my guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Linux-Gaming-Guide.md).
- Now, we're going to be using **Lutris** to install and play Metin2. There is a Lutris script for **Gameforge Client** which means it is easier to install than you thought, we're going to be using that script.
- However, I suggest you to install Gameforge Client **twice** using different names for your shop and main accounts because Gameforge Client runs very **buggy** on Linux and the client simply doesn't launch Metin2 anymore after launching the game several times on the same client which forces you to close the whole client and reopen it. That can be annoying, so to avoid problems, I suggest you to install the client twice.
## Install Gameforge Client
- **Step 1**: Open `Lutris` (surprisingly)
- **Step 2**: Click on the `Plus (+)` button on top left of the app.
- **Step 3**: Click on `Search the Lutris website for installer` and type gameforge.
- **Step 4**: Now, install the script.
- **Step 5**: Apply the same steps for the second client I suggested you to install. Simply install it again but make sure you changed the folder name in `Select installation directory` step.
## Installing Metin2
Installing Metin2 is not hard. Simply log in and install Metin2. However, the installer will be stuck at 95%, 97% etc. and in this case, all you have to do is to stop Gameforge Client in Lutris. When you open the client again, you're going to see that the game is installed successfully. Also, once you launch the game and close it, you'll keep seeing `in-game` sign in client because like I said, it is buggy on Linux.
## Optimize Metin2
Metin2 is not a good optimized game at all. So if you're using **Wayland**, your performance in game will be very poor because WINE on Wayland is **not native** (it will be native soon). That's why, I suggest you to use **X11**.
- **Step 1**: In Lutris, right click on Gameforge Client and go to `Configure`
- **Step 2**: Go to `System options` and enable `Advanced` option on top right. Scroll down a bit and find `Environment variables` section. Make sure you add these variables like in the examples and save it:
  - `Key` **:** `DXVK_HUD` | `Value` **:** `66` - **The value is for 60 hz screen. If your screen refresh rate is different, add some more numbers to it**
  - `Key` **:** `WINEDEBUG` | `Value` **:** `-all`
  - Don't forget to apply the same for the second client if you created one. Also, you can restrict the CPU cores to use for the client you will use for your shop(s) only, so your main game can perform better.
- **Step 3**: Open your file manager and follow the directory:
`/home/yourname/Games/gameforge-client/drive_c/your-games-location/metin2/en-GB(or another code for your server)/bgm`
    - After reaching `bgm` folder, delete everything in the folder permanently, don't delete the folder itself, only delete the files inside. We just deleted music files that run in the background while playing which might **consume much CPU** and reduce performance.
    - Now go back to `en-GB` folder and delete `logo1.avi` and `logo2.avi`.
    - Open `config.exe` once and hit `OK`, this will create `metin2.cfg`. Now open `metin2.cfg` via a text editor.
    - `Width` **:** `1280`
    - `Height` **:** `720`
    - `BPP` **:** `16`
    - `PRE_LOADING_DELAY_TIME` **:** `0`
      - *save the file*
    - Don't forget to apply the same steps for the other client.
### Optimize In-Game Settings
You are ready to play after changing some in-game settings for performance.
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
So, this was my Metin2 installation and optimization guide. I hope the guide helped you to play Metin2 on Linux with optimized settings! Have a nice day! 🤭
