# Before Starting
> [!NOTE]
> - The software we will be using in order to play <img width="16" height="25" alt="GI" src="https://github.com/user-attachments/assets/5b348860-e317-42c5-b684-275fa9187545" /> Genshin Impact on Linux is <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f50ef5c1-e0e0-4ab8-9a38-b687b8f9c08c" /> [AAGL](https://github.com/an-anime-team/an-anime-game-launcher).
> - If you are ready, let's begin!
# Get Started
- First of all, **launch <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f50ef5c1-e0e0-4ab8-9a38-b687b8f9c08c" /> AAGL** and complete installation steps.
> [!NOTE]
> - Once you see the `Launch` button, you are **officially ready to play** <img width="16" height="25" alt="GI" src="https://github.com/user-attachments/assets/5b348860-e317-42c5-b684-275fa9187545" /> Genshin Impact.
> - However, the performance **will not be the same** as Windows. So you might want to keep reading the guide for optimization tips.
## Optimization Tips
### Launcher Settings
> [!NOTE]
> - Launcher settings **may not increase performance** if you have a **strong system**.
> - However if you have a **low-end (weak) system**, slight changes can **enhance** your experience.
- In the launcher, click `Settings` icon next to `Launch` button.
  - Scroll down and go to `Launcher behavior`.
    - If you have at least 16 GB RAM, you can keep it as `Hide`.
    - If you have 12 GB or less RAM, change it to `Close`.
  - Now go to `Components` and make sure that the `Selected version` is a `Spritz-Wine-TKG` build. If not, you can install it from the same page.
  - Scroll down and go to `Gplasync`.
    - Install the latest version and change your `DXVK version` to the one you installed.
- Go back from `Components` and go to `Enhancements` that is on top.
  - Under `Wine` section, change `Synchronization` to `None` and go to `Environment`.
  - In `Environment`, make sure your environment part looks like this:
<img width="612" height="573" alt="image" src="https://github.com/user-attachments/assets/6a70e344-e977-49c5-b146-5bd6f42cd7d8" />

> [!NOTE]
> - If you are **not** using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland, do not include the `env -u DISPLAY %command%` part.
>   - If you are using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland, go back and enable `Borderless window` under `Wine` section if <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland's window decoration discomforts you.

### In-Game Settings
- `Esc` **-** `Settings` **-** `Graphics`
- **For high-end computers** - *Gaming PCs*
<img width="894" height="622" alt="image" src="https://github.com/user-attachments/assets/24f631ef-4cdc-4863-a5b5-fe3102c502fc" />
<img width="894" height="319" alt="image" src="https://github.com/user-attachments/assets/e915c866-72bd-4064-b8b6-f2ea54ecfd9e" />
