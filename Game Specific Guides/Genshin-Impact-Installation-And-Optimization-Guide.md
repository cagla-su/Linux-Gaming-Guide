# Table of Contents
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#before-starting)
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#get-started)
  - [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#optimization-tips)
    - [Launcher Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#launcher-settings)
    - [In-Game Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#in-game-settings)
    - [Other In-Game Settings](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#other-in-game-settings)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#conclusion)
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
> - However if you have a **low-end (weak) system**, slight changes can **enhance** your gaming experience.
- In the launcher, click `Settings` icon next to `Launch` button.
  - Scroll down and go to `Launcher behavior`.
    - If you have **at least 16 GB RAM**, you can keep it as `Hide`.
    - If you have **12 GB or less RAM**, change it to `Close`.
  - Now go to `Components` and make sure that the `Selected version` is a `Spritz-Wine-TKG` build. If not, you can install it from the same page.
  - Scroll down and go to `Gplasync`.
    - Install **the latest** version and change your `DXVK version` to the one you installed.
- Go back from `Components` and go to `Enhancements` that is on top.
  - Under `Wine` section, change `Synchronization` to `None` and go to `Environment`.
  - In `Environment`, make sure your environment part looks like this:
<img width="612" height="573" alt="image" src="https://github.com/user-attachments/assets/6a70e344-e977-49c5-b146-5bd6f42cd7d8" />

> [!NOTE]
> - If you are **not** using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland, **do not include** the `env -u DISPLAY %command%` part.
>   - If you are using <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland, go back and enable `Borderless window` under `Wine` section **if <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland's window decoration discomforts you**.

### In-Game Settings
- `Esc` **-** `Settings` **-** `Graphics`

- **For the optimal visual quality** - *For gaming PCs and strong systems*
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/2dea7cf5-a2a4-493a-a45f-9a3e517d6f08" />
<img width="894" height="319" alt="image" src="https://github.com/user-attachments/assets/e915c866-72bd-4064-b8b6-f2ea54ecfd9e" />

---
- **For the best performance** - *For low-end devices or highest performance enjoyers*
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/8686b8fc-0e88-41c6-9b96-00500f352eb6" />
<img width="894" height="319" alt="image" src="https://github.com/user-attachments/assets/485e9dd3-1192-4bd5-ba58-2a2604c19f7e" />


- **For a balance of visual quality and performance** - *For mid-range computers*
<img width="894" height="610" alt="image" src="https://github.com/user-attachments/assets/57e32bf1-8296-4bc4-b602-c596692fa488" />
<img width="894" height="322" alt="image" src="https://github.com/user-attachments/assets/851bba7e-10f2-4796-8d23-e39677ec63a1" />


- **For a balance of visual quality and performance V2** - *For computers with slightly strong CPUs without a dedicated GPU such as i5-8265U + Intel UHD 620*
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/90fdaa7e-7ff1-4db2-b1ac-f24cad059efa" />
<img width="894" height="318" alt="image" src="https://github.com/user-attachments/assets/51b84c24-c719-411a-9e0d-1cc8eeedd674" />

### Other In-Game Settings
- `Settings` **-** `Audio` **-** `Dynamic Range` **-** `Limited`
- `Settings` **-** `Other` **-** `Mini-Map Settings` **-** `Fixed`

# Conclusion
This guide was about Genshin Impact installation and optimization! I hope the guide has been useful. Thank you for reading, happy gaming! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />
