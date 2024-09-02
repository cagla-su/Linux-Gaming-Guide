# Metin2
Metin2 is an old MMORPG game. Even though it doesn't have players as much as it used to have in the past, I still play it and found ways to optimize it. I don't think any Linux user is playing Metin2 but I still wanted to document it in case there are people thinking of playing it on Linux.
## Get Started
- First of all, make sure your system is ready for gaming following [my guide](https://github.com/citloveslinux/Linux-Gaming-Guide/blob/main/1-Prepare-Your-System.md).
- Now, we're going to be using **Lutris** to install and play Metin2. There is a Lutris script for **Gameforge Client** which means it is easier to install than you thought, we're going to be using that script.
- However, I suggest you to install Gameforge Client twice using different names for your shop and main accounts because Gameforge Client runs very buggy on Linux and the client simply doesn't launch Metin2 anymore after launching the game several times on the same client which forces you to close the whole client and reopen it. That can be annoying, so to avoid problems, I suggest you to install the client twice.
## Install Gameforge Client
- **Step 1**: Open Lutris (surprisingly)
- **Step 2**: Click on the Plus (+) button on top left of the app.
- **Step 3**: Click on **Search the Lutris website for installer** and type gameforge.
- **Step 4**: Now, install the script.
- **Step 5**: Apply the same steps for the second client I suggested you to install. Simply install it again but make sure you changed the folder name in **Select installation directory** step.
## Installing Metin2
Installing Metin2 is not hard. Simply log in and install Metin2. However, the installer will be stuck at 95%, 97% etc. and in this case, all you have to do is to stop Gameforge Client in Lutris. When you open the client again, you're going to see that the game is installed successfully. Also, once you launch the game and close it, you'll keep seeing "in-game" sign in client because like I said, it is buggy on Linux.
## Optimize Metin2
Optimizing Metin2 is the funniest part 🤭 I have lots of fun during this step.
- **Step 1**: Install **Protonup-QT** and open it. Make sure **Lutris** is chosen in **Install for:** section.
- **Step 2**: Click on **Add version** and choose **DXVK Async** in **Compatibility tool:** section, install the latest version.
- **Step 3**: After DXVK Async is installed, open Lutris and point your mouse on **Wine** on the left sidebar. Click on the gear icon that appeared.
- **Step 4**: Make sure you turned on **Advanced** option. Now change **DXVK version** to **dxvk-gplasync** and go to **System options**. Scroll down a bit and find **Environment variables** section. Make sure you added a variable like in the example and save it:
  - **Key**: DXVK_ASYNC
  - **Value**: 1
- **Step 5**: Click on Gameforge Client in your Lutris library. Click on the triangle next to wine icon next to **Play** button and go to **Wine configuration**.
  - Now in the opened window, go to **Libraries** section.
  - Add new overrides for the library **d3d9, d3dx9_43 and d3dcompiler_47** and edit them all to be set as **Windows (Native)** and save changes.
  - Don't forget to apply the same steps for the second client.
- **Step 6**: Open your file manager and follow the directory:
  - /home/yourname/Games/gameforge-client/drive_c/your-games-location/metin2/en-GB(or another code for your server)/bgm
    - After reaching *bgm* folder, delete everything in the folder permanently, don't delete the folder itself, only delete the files inside. We just deleted music files that run in the background while playing which might use CPU and reduce performance.
    - Now go back to *en-GB* folder and delete *logo1.avi* and *logo2.avi*
    - Open *config.exe* once and hit **OK**, this will create **metin2.cfg**. Now open **metin2.cfg** via a text editor.
    - Change the *Width* value to *1280* and *Height* value to *720*, this is probably smaller than your native resolution which can help improving performance. Next, change *BPP* value to *16* which will run the game with less colors, it will improve the performance **drastically**. Lastly, change *PRE_LOADING_DELAY_TIME* value to *0* and save the file.
    - Don't forget to apply the same steps for the other client.
### Optimize In-Game Settings
You are ready to play after changing some in-game settings for performance.
- **Game Options**
  - **Chat Line**: Hide
  - **Name**: Always
  - **Hit Info**: Hide
  - **Animations**: Performance
  - **Shop name**: Hide
  - **Monster info**: Level (uncheck)
  - **Decoration**: Hide
- **System Options**
  - **Camera**: Subjective
  - **Fog**: Off
  - **Night**: Subjective
  - **Snowfall**: Off
  - **Snow**: Off
  - **Target shadow**: 2
  - **Shadow Quality**: Low
  - **Effects**: 3
  - **Private Shops**: 3
  - **Item Drops**: 2
  - **Pets**: On
  - **NPC Names**: Off
# Conclusion
So, this was my Metin2 installation and optimization guide. I hope the guide helped you to play Metin2 on Linux with optimized settings! Have a nice day! 🤭
