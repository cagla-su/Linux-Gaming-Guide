# The Sims 2
- The Sims 2 is the game of our childhood and it is surprisingly running on Linux better than The Sims 3 (The Sims 3 can't even run properly on Windows either, it's a weird version).
- On my previous low end laptop and the laptop I'm currently using, I didn't experience any performance differences and I can say that the game runs with **native performance** on Linux.
- Since The Sims 2 is an abandonware, we can't get it through legal ways. That's why you should either have the cracked file or the DVD to install the game.
- So, let's begin the guide!
## Get Started
- First of all, extract files inside the DVD into a folder and open Lutris.
- Click `Plus (+)` on top left and go to `Install a Windows game from an executable`.
- Now simply type **The Sims 2** on `Game name` section and continue until `Select the setup file` section.
- Now click `...` button and click on your setup file (probably setup.exe) and let the installation begin, complete the installation like how you would do on Windows.
- After installation is completed, make sure to locate the game to the correct file to be able to run the game. To do so:
  - `The Sims 2 (right click) - Configure - Game Options - Executable`
    - The location is generally `~/Games/the-sims-2/drive_c/Program Files (x86)/The Sims 2 Ultimate Collection/The Sims 2 Mansion and Garden Stuff/TSBin/Sims2EP9.exe` 
### Graphics Rules Maker Setup
- To prevent/fix incompatibility issues, we should download [Graphics Rules Maker](https://www.simsnetwork.com/tools/graphics-rules-maker).
- After downloading GRM, follow the next steps:
  - Open Lutris and click `Plus (+)`, then go to `Install a Windows game from an executable`.
  - Give it any name you want and continue until `Select installation directory` section. Click `...` button and choose `~/Games/the-sims-2/`, then continue.
  - Now click `...` button, choose your setup file and let the installation begin, complete the installation like how you would do it on Windows.
    - At the last step, you should see an option that says "Launch Graphics Rules Maker.", make sure to untick that box before completing installation.
  - Don't forget to locate to the correct file to be able to run the app. To do so:
    - `GRM (right click) - Configure - Game Options - Executable`
    - The location is `~/Games/the-sims-2/drive_c/Program Files/Graphics Rules Maker/bin/GraphicsRulesMakerUi.exe`
  - After GRM is installed, we can launch it but if you have 2 GPUs, make sure Lutris is running GRM via your **dedicated GPU**, you can check my [Linux Gaming Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Linux-Gaming-Guide.md#hybrid-graphics) to run Lutris games on your dedicated GPU.
  - After GRM is launched, choose `The Sims 2` from `Game` tab. It should detect your Sims folder automatically but if it can't, try `Mansion and Garden Stuff` folder.
  - Now click `Auto-detect`. If you have iGPU, change `Force texture memory` value to **512** or **1024** to your liking.
  - As the last step, click `Save Files...`. Don't forget to perform the same steps for `The Sims 2 Body Shop`.
- Now all you should do is running The Sims 2! 😊
## Conclusion
This guide was actually a bit short because [Sims 2 Subreddit](https://www.reddit.com/r/sims2/) did a great job while preparing the guide for 3 major operating systems. You can join their subreddit if you're interested. Dag dag Simmers. Have a nice day! 🐧
