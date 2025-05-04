# The Sims 2
- The Sims 2 is the game of our childhood, and it runs smoothly on Linux.
- Since The Sims 2 is abandonware, it is not legally obtainable. That is why you should either have the cracked file or the DVD to install the game.
- So, let's begin the guide!
## Get Started
- First of all, extract the files from the DVD into a folder and open Lutris.
- Click `(+)` on the top left and go to `Install a Windows game from an executable`.
- Now simply type **The Sims 2** in the `Game name` section and continue until the `Select the setup file` section.
- Now click the `...` button and select your setup file (probably setup.exe). Next, start the installation and let it complete.
- After installation is completed, make sure the game is located correctly. To do so:
  - `The Sims 2 (right click) - Configure - Game Options - Executable`
    - The location is generally `~/Games/the-sims-2/drive_c/Program Files (x86)/The Sims 2 Ultimate Collection/The Sims 2 Mansion and Garden Stuff/TSBin/Sims2EP9.exe` 
### Graphics Rules Maker Setup
- To prevent or fix incompatibility issues, you should download [Graphics Rules Maker](https://www.simsnetwork.com/tools/graphics-rules-maker).
- After downloading GRM, follow these steps:
  - Open Lutris and click `Plus (+)`, then go to `Install a Windows game from an executable`.
  - Name it how you want and continue until `Select installation directory` section. Click the `...` button and select `~/Games/the-sims-2/`, then continue.
  - Now click the `...` button, select your setup file and start the installation. Let it complete as you would do on Windows.
    - At the last step, you should see an option that says `Launch Graphics Rules Maker`. Make sure to untick that box before completing the installation.
  - Make sure the app is located correctly. To do so:
    - `GRM (right click) - Configure - Game Options - Executable`
    - The location is `~/Games/the-sims-2/drive_c/Program Files/Graphics Rules Maker/bin/GraphicsRulesMakerUi.exe`
  - After GRM is installed, you can launch it. However if you have two GPUs, make sure Lutris is running GRM via your **dedicated GPU**, you can check my [Linux Gaming Guide](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Linux-Gaming-Guide.md#hybrid-graphics) to see how to run Lutris games on your dedicated GPU.
  - After GRM is launched, select `The Sims 2` from the `Game` tab. It should detect your Sims folder automatically but if it cannot, try `Mansion and Garden Stuff` folder.
  - Now click `Auto-detect`. If you have an iGPU, change the `Force texture memory` value to **512** or **1024** to your liking.
  - As the last step, click `Save Files...`. Do not forget to perform the same steps for `The Sims 2 Body Shop`.
- Now all you need to do is run The Sims 2! 😊
## Conclusion
This guide was about The Sims 2 installation and optimization! I hope the guide has been useful. Thank you for reading, have a nice day! 🐧
