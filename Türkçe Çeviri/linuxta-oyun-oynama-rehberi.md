# İçindekiler
- [Linux'ta oyun oynama](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#how-linux-gaming-works)
- [Vulkan sürücülerini yükleme](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
- [Oyun oynama yazılımı yükleme](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software)
- [Hibrit grafik sistemi yapılandırması](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#hybrid-graphics-setup)
- [Harici disk yapılandırması](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#external-disk-setup)
- [Optimizasyon tavsiyeleri](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#optimization-tips)
## Oyunlara Özel Rehberler
- ![Metin2](https://github.com/user-attachments/assets/c887fc49-cc62-4450-81ab-7ebdfe0087df) **Metin2 -** [Metin2 Linux rehberi](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Metin2-Installation-And-Optimization-Guide.md)
-  ![Minecraft](https://github.com/user-attachments/assets/3dd086b5-0be3-4cc9-ab2f-e01243845930) **Minecraft -** [Minecraft Linux rehberi](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- ![Sims 2](https://github.com/user-attachments/assets/5e79e395-066b-46df-85a4-a72f73d8aad8) **The Sims 2 -** [The Sims 2 Linux rehberi](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
# Linux'ta oyun oynama rehberi
Merhaba. Bu rehberde **Linux'ta oyunların nasıl çalıştığı**, **sisteminizi Linux'ta oynamaya hazır hale nasıl getirebileceğiniz** ve **Linux sisteminizi daha yüksek performans için nasıl optimize edebileceğiniz** konuları hakkında bilgilendirileceksiniz. Hazırsanız, başlayalım!
## Başlamadan önce
- Linux, oyun oynama konusunda hızlı bir şekilde geliştiriliyor. Her geçen gün, daha fazla kullanıcı Linux'a geçmeye başlıyor. Ayrıca, Linux'un piyasa payı da bu bağlamda artıyor.
- Bu rehber Linux'ta oyun oynamak isteyip nereden başlayacağını bilmeyen herkes için kullanışlı olmayı amaçlıyor.
- Bu rehberi okuduktan sonra içinde oynamak istediğiniz bir oyun varsa, [Oyunlara Özel Rehberleri]() de okumanızı tavsiye ediyorum.
# Linux'ta oyunlar nasıl çalışır?
- Windows oyunlarını Linux'ta oynayabilirsiniz. Ancak, bu **hiçbir Linux uyumlu oyunun olmadığı** anlamına gelmez. **Bazı Linux uyumlu oyunlar** şunlardır: 
	- Minecraft, Terraria, Stardew Valley, Euro Truck Simulator 2 ve fazlası
 	- **Valve oyunları:** Counter-Strike serisi, Team Fortress 2, Dota 2, Portal vb.
- Genellikle Linux uyumlu oyunlar **Vulkan gerektirmediği** takdirde **herhangi bir yapılandırma** gerektirmez. Eğer gerektiriyorsa bu rehberde açıklandığı üzere, Vulkan sürücülerini kurmalısınız.
- Windows oyunları Linux'ta çalışmak için bazı **gerekli araçlar** gerektirir ve bu araçlar şunlardır:
	- [WINE](https://www.winehq.org/) / [Proton](https://github.com/ValveSoftware/Proton) **-** WINE **Windows kütüphane dosyalarını Linux kütüphane dosyalarına** yönlendiren bir uyumluluk katmanıdır. **Windows'taki uyumluluk modu** ile aynı şekilde çalışır. Proton ise Valve tarafından geliştirilen, **WINE'ın çatallanmış halidir** ve özellikle **Steam oyunları** için yapılandırılmıştır.
	- [DXVK](https://github.com/doitsujin/dxvk) **-** DXVK Windows oyunlarını Linux'ta çalıştırmak için **DirectX 8-11** çağrılarını **Vulkan'a** çevirir. DXVK WINE'ın **içinde bulunur**, yani **el ile kurulum yapmak zorunda değilsiniz**.
		- DXVK ile **benzer amaçlar** taşıyan **diğer araçlar** da vardır ve bu araçlar şunlardır:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d) **-** VKD3D, DXVK'in henüz yapamadığı **DirectX 12** çağrılarını **Vulkan'a** çevirme işlevini görür. Oynamaya çalıştığınız oyun **DirectX 12 oyunu** ise bu araç **varsayılan** araçtır. Tıpkı DXVK gibi, VKD3D WINE'ın **içinde bulunur**.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d) **-** WINED3D, **DirectX 8-11** çağrılarını **Vulkan yerine OpenGL'e** çevirir. Sisteminizde **Vulkan sürücüleri yüklü değilse** bu araç **varsayılan** araçtır. Ancak, DirectX çağrıları OpenGL'e çevirileceği için **düşük performans** almanız muhtemeldir çünkü OpenGL **artık geliştirilmiyor**. Tıpkı DXVK ve VKD3D gibi, WINED3D WINE'ın **içinde bulunur**.
```
+------------------+   DirectX: Windows'a özgü grafik kütüphanesi
|       WINE       |   Vulkan: Hem Windows hem de Linux'a özgü grafik kütüphanesi
+------------------+   OpenGL: Hem Windows hem de Linux'a özgü grafik kütüphanesi (artık geliştirilmiyor)
         ||
         ||
+----------------------------++--------------------------+
|          DXVK              ||           VKD3D          |
| (DirectX 8-11 -> Vulkan)   ||   (DirectX 12 -> Vulkan) |
+----------------------------++--------------------------+
            ||
+--------------------------+
|         WINED3D          |
| (DirectX 8-11 -> OpenGL) |
+--------------------------+

```
- WINE, bir oyun oynama yazılımı kurduğunuzda **otomatik olarak** yüklenir.
## NVIDIA kullanıcıları için bir uyarı
- VIDIA **4xxx** ve **5xxx** modelleri için **özel mülkiyet** sürücülerini **aşamalı olarak devre dışı bırakıyor**, çünkü NVIDIA **son çıkan ve gelecekteki kartları için daha fazla açık kaynak** olmaya çalışıyor. Ancak **daha eski kartlar için** hâlâ **özel mülkiyet** sürücüleri kullanmalısınız. Böylece **daha iyi uyumluluk ve performansa** sahip olursunuz. 
- Ayrıca, yukarıda bahsedilen son NVIDIA ekran kartlarından birini kullanmadığınız takdirde **Wayland kullanmamalısınız** çünkü bu durumda **ekranda bozukluklar ve/veya performans sorunları** ile karşılaşabilirsiniz. **X11** kullanmak şimdilik daha iyi bir seçenektir.
# Başlangıç
## Vulkan sürücülerini yükleme
- Bu adım [Lutris'in topluluk rehberinde](https://github.com/lutris/docs/blob/master/InstallingDrivers.md) açıklanmıştır.
- Eğer sayfada kendi Linux dağıtımınızı görmüyorsanız, bu muhtemelen Mesa **(varsayılan Intel/AMD ekran kartı sürücüsü)** Vulkan sürücülerinin önceden yüklenmiş olduğunu anlamına geliyordur.
	- Ancak, dağıtımınızı sayfada görmüyorsanız ve NVIDIA kullanıyorsanız, yükleme adımları için başka bir belge bulmanızı veya sayfada bahsedilen dağıtımlardan birine geçmenizi tavsiye ediyorum.

## Oyun oynama yazılımı yükleme
- Linux uyumlu bazı popüler oyun oynama yazılımları şunlardır:
	- [Steam](https://store.steampowered.com/) **-** Steam, Linux ile uyumludur.
	- [Heroic Games Launcher](https://heroicgameslauncher.com/) **-** Heroic, **Epic Games, GOG ve Prime Gaming** oyunlarını oynamanıza olanak tanıyan hoş bir oyun başlatma platformudur.
	- [Lutris](https://lutris.net/) **-** Lutris, Windows oyunlarını oynamak için hoş bir oyun başlatma platformudur. **Epic Games, Battle.net, Ubisoft vb.** gibi bazı oyun oynama yazılımlarını **direkt olarak** yükleyip çalıştırabilirsiniz fakat ayrıca belirli bir platforma ait olmayan oyunları da Lutris aracılığıyla çalıştırabilirsiniz.
		- Lutris, oldukça büyük miktarda oyun ve yazılım için **topluluk tarafından hazırlanmış betik dosyaları** sunar.
		- Eğer kurulum dosyanız varsa, DVD oyunları da dahil, oyunlarınızı el ile kurabilirsiniz.
	- [ProtonPlus](https://protonplus.vysp3r.com/) **-** ProtonPlus'ı kullanarak daha iyi uyumluluk ve performans için özel WINE/Proton sürümleri yükleyebilirsiniz. Özel WINE/Proton sürümleri Lutris, Steam ve Heroic tarafından desteklenir.
### Notlar
- Bu yazılımları **paket yöneticiniz** veya [Flatpak](https://flatpak.org) aracılığıyla yükleyebilirsiniz.
- Steam oyunlarınızın Linux'ta oynanabilirliğini görebilmek için [ProtonDB'yi](https://www.protondb.com) kullanabilirsiniz.
	- Adını arattığınız oyun **gümüşten daha düşük** bir kademede ise, bu o oyunun **oynanabilir olmadığı** anlamına gelir.
	- Oyununuz için herhangi bir değerlendirme yazılmışsa optimizasyon tavsiyeleri alabilirsiniz. Dilerseniz istediğiniz herhangi bir Steam oyunu için kendi değerlendirmelerinizi de yazabilirsiniz.
# Hibrit grafik sistemi yapılandırması
- Eğer sisteminizde **iki adet ekran kartı** bulunuyorsa, iki ekran kartı için de Vulkan sürücülerinin kurulması ve oyunlarınızın harici ekran kartıyla çalışması için ayarlanması önerilir.
- Harici ekran kartınız **AMD** ise oyunlarınızı harici ekran kartıyla çalıştırmak için gerekli olan komut şudur:
```
DRI_PRIME=1
```
 - Harici ekran kartınız **NVIDIA** ise oyunlarınızı harici ekran kartıyla çalıştırmak için gerekli olan komut şudur:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Oyunları harici ekran kartıyla çalıştırmanın yolları
- Oyunları harici ekran kartınızla çalıştırmanız için **dört yol** vardır:
	- **1 -** [Terminal yolu](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#terminal-method)
 	- **2 -** [Masaüstü kısayol yolu](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#desktop-shortcut-method)
 	- **3 -** [Steam oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games)
  	- **4 -** [Lutris/Heroic oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-lutrisheroic-games)
### Terminal yolu
Kısaca terminali çalıştırın ve örnekteki gibi ekran kartınız için olan komutu çalıştırın:
```
DRI_PRIME=1 prismlauncher
```
### Masaüstü kısayol yolu
- Masaüstünüzde bir **.desktop** dosyası oluşturun.
- Bu, NVIDIA ekran kartıyla Prism Launcher çalıştırmak için oluşturulmuş örnek bir .desktop dosyasının içeriğidir. Dikkat etmeniz gereken satır `Exec` ile başlayan satırdır:
```
[Desktop Entry]
Version=1.0
Type=Application
Name=Prism Launcher
Comment=Prism Launcher
Exec=env __NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia prismlauncher
Icon=/path/to/your/game/icon.png
Terminal=false
Categories=Game;
```
- Kısaca, en başa `env` ve devamına ekran kartınız için olan komutu ekleyin. Son olarak da oyununuzun paket adını ekleyin.
### Steam oyunları için
Add the command for your GPU in your launch options of the games you want to play. Do not forget to add `%command%` at last like in the example:
```
DRI_PRIME=1 %command%
```
- **NOTE**: If you are going to use gamemode and run games through your dedicated GPU, make sure that all the commands are written before `%command%` like in the example:
```
DRI_PRIME=1 gamemoderun %command%
```
### For Lutris/Heroic Games
- **Lutris -** On the left side bar, click the **gear icon** that appears when you point your mouse cursor on `Wine`.
	- `System Options` **-** `Enable Advanced` **-** `Use Discrete Graphics`
 - **Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# External Disk Setup
- If your external disk is **natively** connected, you might be able to use it **out of the box** depending on your Linux distribution. However, if you are using your external disk **through an SSD case (USB)**, you should configure it manually.
- The same steps **should be valid** if your disk is **natively connected** but **you still are not able to use it**.
## Get Started: GParted
- If you would like to format your disk to change its file system from **NTFS** to a **Linux-compatible** one, install `gparted` package using your package manager and follow the next steps, making sure your external disk is unmounted.
	- `Launch GParted` **-** `select your external disk from the top right` **-** `delete all the partitions` **-** `Add`
 	- **Next:** `File system: ext4` **-** `Label: anything you wish` **-** `Add`
  	- **Lastly:** `Apply All Operations`
## How to Configure External Disks on Linux?
- First of all, install `gnome-disk-utility` package using your package manager.
	- Also, if you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, make sure to install `ntfs-3g` package using your package manager.
- After the installation, launch `Disks` app from your application launcher.
- Then, find your external disk from the menu on the left and click this button under `Volumes`.
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- From the menu, click `Take Ownership` and confirm.
- After taking the ownership, open the same menu and click `Edit Mount Options`.
  - Now disable `User Session Defaults` and check `Mount at system startup`.
  - Next, find the box that does not have a label that is under `Symbolic Icon Name` box and make sure you only have these mount options:
  	- `nofail,x-gvfs-show,rw,user,exec`
   - If you are going to use your previous external disk that you were using on Windows, in other words **as NTFS**, additionally include this option:
        - `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
   - Lastly, change `Identify As` value to `/dev/disk/by-label/your-disk` and click OK.
<img width="904" height="493" alt="imagee" src="https://github.com/user-attachments/assets/56cf7ae7-d9f7-42fc-81de-b23b671622d2" />

- Now you are ready to use your external disk! 
# Optimization Tips
## Reducing Game Resolution and Using the Lowest Graphics Settings
- When you reduce the game's resolution, less pixels will be rendered and it will result in less loads on your hardware which leads to higher performance.
- When you play with the lowest graphics settings, less details will be rendered which leads to higher performance.
- Both are going to increase performance while reducing visual quality. You can experiment to find your own balanced settings.
## Using a Performance Kernel
- **For Arch and Derivatives:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **For Fedora and Derivatives:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **For Debian/Ubuntu and Derivatives:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) is a tool that **temporarily** changes your system settings to increase performance during the gameplay. Generally, gaming software like Lutris enable it by default. But on Steam, you have to manually add a command in your game's launch options like in the example:
```
gamemoderun %command%
```
- After installing gamemode, download [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) and move the file to `/etc/` via executing the command below after locating the terminal to your Downloads directory:
```
sudo mv gamemode.ini /etc/
```
## Performance-Increasing Environment Variables
You can use these environment variables for better performance while gaming:
- `WINEDEBUG=-all` **-** It suppresses all debug outputs of WINE. - *low effect on performance*
- `mesa_glthread=true` **-** It improves **OpenGL performance** on **Intel/AMD GPUs**. - *high effect on performance*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** It improves **OpenGL performance** on **NVIDIA GPUs**. - *high effect on performance*
- `DXVK_ASYNC=1` **-** It **does not work on Steam games** but it **displays frames without waiting for shaders to be compiled** which works on Lutris and Heroic. However, using async can **get you banned from online games you play**. That's why, it is only recommended for **offline games**. - *depending on the game, generally low effect on performance*
### How Can You Use These Environment Variables?
- **Steam -** You can simply use these commands in launch options of the games you want to play. Do not forget to add `%command%` at last.
- **Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />

## Disabling Compositor - X11 ONLY!!!
**WARNING**: If you are using **Wayland**, you **cannot** disable the compositor. These steps are only available for **X11**.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which **reduces visual quality while improving performance**.
- This step is explained [in this guide](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)).
# Conclusion
This guide was about Linux gaming. I hope the guide has been useful. Thank you for reading, happy gaming! 🐧


