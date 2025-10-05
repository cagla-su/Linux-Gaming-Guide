# İçindekiler
- [Before Starting](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#before-starting)	
 	- [How Does Linux Gaming Work?](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#how-does-linux-gaming-work) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />
  	- [Warning for NVIDIA Users](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?search=1#warning-for-nvidia-users-) <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/675b9126-59e6-4fbf-af53-1a023465daf7" />
	- [Issues of Linux Gaming](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#issues-of-linux-gaming) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />
- [Get Started](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?search=1#get-started)
	- [Installing Vulkan Drivers](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-vulkan-drivers)
	- [Installing Gaming Software](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#installing-gaming-software) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
	- [Hybrid Graphics Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#hybrid-graphics-setup) <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/e08c4e5e-47c8-40cc-81f6-cfabb2829198" /> <img width="16" height="32" alt="nvidia" src="https://github.com/user-attachments/assets/13d0a891-100e-45d2-a579-cb3a76a5da06" />
		- [Ways to Run Games through the Dedicated GPU](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#ways-to-run-games-through-the-dedicated-gpu)
	- [External Disk Setup](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#external-disk-setup)
 		- [Get Started: GParted](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#get-started-gparted-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8119e97a-f45c-4859-bbf2-2b9b26b542a5" />
   		- [How to Configure External Disks on Linux?](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-to-configure-external-disks-on-linux)
	- [Optimization Tips](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#optimization-tips)
 		- [Reducing Game Resolution and Using the Lowest Graphics Settings](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#reducing-game-resolution-and-using-the-lowest-graphics-settings)
   			- [Lossless Scaling](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#lossless-scaling-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" />
  		- [Using a Performance Kernel](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#using-a-performance-kernel)
		- [Gamemode](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#gamemode)
		- [Performance-Increasing Launch Options](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#performance-increasing-launch-options)
			- [How Can You Use These Launch Options](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#how-can-you-use-these-launch-options)
		- [Disabling Compositor](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#disabling-compositor---x11-only-)
- [Conclusion](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#conclusion)
## Oyunlara özel rehberler
- <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> **Minecraft -** [Minecraft Linux Rehberi](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Minecraft-Installation-And-Optimization-Guide.md)
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/35809d93-5960-4e2b-bc5d-2639cb667c04" /> **The Sims 2 -** [The Sims 2 Linux Rehberi](https://github.com/cutiepenguins/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/The-Sims-2-Installation-And-Optimization-Guide.md)
# Linux'ta oyun oynama rehberi
Esenlikler. Bu rehber size **Linux'ta oyunların nasıl çalıştığını, sisteminizi oyun oynamak için nasıl hazırlayabileceğinizi** ve **sisteminizi daha yüksek performans için nasıl en iyi hâle getirebileceğinizi** anlama konusunda yardımcı olmayı amaçlayan bir rehberdir. Hazırsanız, başlayalım!
# Başlamadan önce
- Linux'ta oyun oynama dünyası **hızla gelişiyor**. Her geçen gün, daha fazla kullanıcı Linux'a geçiyor. Bu bağlamda da Linux'un **pazar payı** da **artıyor**.
- Bu rehber, Linux'ta **oyun oynamak** isteyen fakat **nereden başlayacağını** bilmeyen herkes için faydalı olmayı amaçlıyor.
- Eğer bu rehberi okuduktan sonra içinde bulunan herhangi bir oyun ilginizi çektiyse [Oyunlara özel rehberler] bölümüne de bakmanızı tavsiye ederim.
- Son olarak, bu rehberde bazı uygulama içi ayarlardan bahsedildi ve bu ayarların hepsi İngilizce olarak verildi. Bunun sebebi ise Linux masaüstü ortamlarının büyük kısmının Türkçeye tamamen çevrilmiş olmasına rağmen Türkçe çeviri desteğinin diğer yazılımlarda tam olmamasıdır. Size tavsiyem sisteminizi İngilizce olarak kullanmanızdır.
## Linux'ta oyunlar nasıl çalışır?
- Linux'ta **Windows oyunlarının birçoğunu** oynayabilirsiniz. Fakat, bu **Linux ile doğrudan uyumlu hiçbir oyunun mevcut olmadığı anlamına gelmez**. Bazı **Linux ile doğrudan uyumlu oyunlar** şunlardır:
  - <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/79d93d2e-2f58-4575-b2f9-f7fc66d0b0cd" /> Terraria, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/791afaf0-7f92-486e-8e2b-baeaf54155f9" /> Stardew Valley, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/bf7d4ca4-aedf-460e-819d-6f8d6a8475d3" /> Euro Truck Simulator 2 vb.
 	- **Valve oyunları -** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/c4e6099e-6a55-488a-b6d8-397bfeec0e20" /> Counter-Strike series, <img width="16" height="25" alt="tf2" src="https://github.com/user-attachments/assets/4efb907f-63e4-41bd-aa55-ca37674d5304" /> Team Fortress 2, <img width="16" height="25" alt="dota" src="https://github.com/user-attachments/assets/b62be047-0b56-4684-b135-80754c18063b" /> Dota 2, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e33b1a9c-fff9-4112-96a6-99499020f84a" /> Portal vb.
- Genellikle Linux ile doğrudan uyumlu oyunlar, **Vulkan gerektirmedikleri takdirde** hiçbir **ek adım gerektirmez**. Eğer gerektiriyorlarsa, bu rehberde açıklandığı üzere **Vulkan sürücülerini kurmalısınız**.
- Windows oyunları Linux'ta çalışabilmek için bazı **temel araçlara** ihtiyaç duyarlar ve bu araçlar şunlardır:
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> [WINE](https://www.winehq.org/) / [Proton](https://github.com/ValveSoftware/Proton) **-** WINE, **Windows kütüphane dosyalarını Linux kütüphane dosyalarına** aktaran bir uyumluluk katmanıdır. Windows'taki **uyumluluk modu** ile aynı şekilde çalışır.
 		- Proton, <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE'ın Valve tarafından **çatallanmış** halidir ve **özel olarak <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam oyunları için tasarlanmıştır**.
	- [DXVK](https://github.com/doitsujin/dxvk) **-** DXVK, Windows oyunlarını Linux'ta çalıştırmak için **DirectX 8-11** çağrılarını **Vulkan'a** çevirir. DXVK <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE'a **dahil edilmemiştir** fakat yine de **DXVK'i elle kurmak zorunda değilsiniz** çünkü **Linux'ta oyun oynama yazılımlarının** ve **özel <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton yapılarının birçoğu** kullanıcılar için DXVK'i dahil eder.
		- **Benzer amaçlar** için kullanılan **başka araçlar** da vardır ve o araçlar şunlardır:
 			- [VKD3D](https://gitlab.winehq.org/wine/vkd3d) **-** VKD3D, DXVK'in henüz yapamadığı **DirectX 12** çağrılarını **Vulkan'a** çevirme işlemini yapar. Oynamaya çalıştığınız oyun bir **DirectX 12 oyunuysa** VKD3D **varsayılan olarak devreye girer**. Tıpkı DXVK gibi, VKD3D de **Linux'ta oyun oynama yazılımlarının** ve **özel <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton yapılarının birçoğunda kendiliğinden dahildir**.
			- [WINED3D](https://gitlab.winehq.org/wine/wine/-/tree/master/dlls/wined3d) **-** WINED3D **DirectX 8-11** çağrılarını **Vulkan yerine OpenGL'e** çevirir. Sisteminizde **Vulkan sürücüleri yüklü değilse** WINED3D **varsayılan olarak devreye girer**. Fakat DirectX çağrıları OpenGL'e çevrileceği için **düşük performans** almanız olasıdır çünkü OpenGL **artık geliştirilmiyor**. DXVK ve VKD3D'nin **aksine**, WINED3D <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE'a **dahildir**.
```
+------------------+   DirectX: Windows'a özgü grafik kütüphanesi
|       WINE       |   Vulkan: Hem Windows hem de Linux ile doğrudan uyumlu grafik kütüphanesi
+------------------+   OpenGL: Hem Windows hem de Linux ile doğrudan uyumlu grafik kütüphanesi (artık geliştirilmiyor)
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
- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE'ı elle yüklemenize gerek yoktur çünkü <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE siz <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris gibi bir oyun oynama yazılımı yüklediğinizde **kendiliğinden yüklenir**.
## NVIDIA kullanıcıları için uyarı <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" />
- <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA, **4xxx** ve **5xxx** serileri için **özel mülkiyet** sürücülerini **aşamalı olarak terk ediyor** çünkü <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA **yeni çıkan ve gelecekte çıkacak olan kartları** için **daha fazla açık kaynak** olmaya çalışıyor. Ancak, **eski kartlarda daha iyi uyumluluk ve performans için** hâlâ **özel mülkiyet** sürücüleri kullanmalısınız.
- Ayrıca, yukarıda bahsedilen güncel <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA ekran kartlarından birini kullanmıyorsanız <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland kullanmamalısınız çünkü bu durumda **görsel bozukluklar ve performans sorunları** ile karşılaşmanız olasıdır. Şimdilik <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" /> X11 kullanmak **daha iyi bir seçenektir**.
## Linux'ta oyun oynamanın zorlukları
- There are **not too many issues** when it comes to gaming on Linux. Linux'ta oyun oynarken **pek fazla sorun yoktur**. Ancak, **esas sorun çekirdek seviyesinde çalışan anti-hile yazılımlarıdır**. Bu anti-hile yazılımları **Linux'ta çalışamazlar**.
	- Sebebi ise bir Windows oyunu için geliştirilmiş çekirdek seviyesinde çalışan bir anti-hile yazılımının **"Windows NT" adı verilen bir çekirdek gerektirmesi** ve bu çekirdeğin **yalnızca Windows için mevcut olmasıdır**.
- Bazı çekirdek seviyesinde çalışan anti-hile yazılımları şunlardır:
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> **| VANGUARD**
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc19a74e-ff75-40dc-9976-50e61be8c4ab" /> **| Easy Anti-Cheat**
	- <img width="13" height="25" alt="image" src="https://github.com/user-attachments/assets/1d9704a0-13ba-4f8d-ada3-ad438abce41c" /> **| BattlEye**
	- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/e05603e5-219b-4ecd-8b5f-f1c9ea6ad077" /> **| XIGNCODE3**
	- <img width="16" height="25" alt="nprotect" src="https://github.com/user-attachments/assets/b2840543-d490-4012-85b6-5647ca747dab" /> **| nProtect GameGuard**
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/fc19a74e-ff75-40dc-9976-50e61be8c4ab" /> **Easy Anti-Cheat** ve <img width="13" height="25" alt="image" src="https://github.com/user-attachments/assets/1d9704a0-13ba-4f8d-ada3-ad438abce41c" /> **BattlEye'ın Linux ile uyumlu sürümleri mevcuttur**. Bu yüzden, bu anti-hile yazılımlarını kullanan bazı bazı oyun geliştiricileri **<img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton için özel olarak Linux uyumluluğunu etkinleştirebilirler**.
	- Ancak, <img width="13" height="25" alt="fortnite" src="https://github.com/user-attachments/assets/17d24518-9a9e-4fa0-a075-24f88e42fa89" /> Fortnite ve <img width="16" height="25" alt="apexlegends" src="https://github.com/user-attachments/assets/1e092ebc-e76d-46b2-90b4-e08d7efcd836" /> Apex Legends gibi oyunların geliştiricileri kendi anti-hile yapılandırmalarında **Linux desteğini etkinleştirmeyebilirler**. Bu yüzden **bu oyunlar Linux'ta çalışamazlar**.
- Linux uyumluluğunu etkinleştirmeye ek olarak bazı oyunlar bu çekirdek seviyesinde çalışan anti-hile yazılımlarının **yalnızca kullanıcı modu modülünü** kullanabilir, ve bu da o oyunları **Linux'ta oynanabilir kılar**.
- <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> **VANGUARD** haricinde, yukarıda bahsedilen çekirdek seviyesinde çalışan anti-hile yazılımlarını kullanan oyunların **oynanabilirlikleri hakkında kesin bir ifadede bulunamayız**.
	- Durum <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD için farklıdır çünkü <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/4f90b991-8cca-481c-8324-a9b497fd8687" /> VANGUARD yalnızca <img width="16" height="25" alt="rito" src="https://github.com/user-attachments/assets/06511a6d-3434-4ae0-be6d-a4d5e0f6c8c8" /> Riot Games'in oyunlarında kullanılır, ve <img width="16" height="25" alt="rito" src="https://github.com/user-attachments/assets/06511a6d-3434-4ae0-be6d-a4d5e0f6c8c8" /> Riot Games Linux'ta oyun oynayanları **desteklemeye niyetli bir şirket değildir**.
# Başlangıç
## Vulkan sürücülerini yükleme
- Bu adım <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> [Lutris'in topluluk rehberinde](https://github.com/lutris/docs/blob/master/InstallingDrivers.md) açıklanmıştır.
- Eğer sayfada **kendi Linux dağıtımınızı göremiyorsanız**, bu muhtemelen Mesa **(varsayılan <img width="16" height="25" alt="intel" src="https://github.com/user-attachments/assets/262e5a2c-6c88-4e6f-a0d1-d8428fb16504" /> <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> Intel/AMD ekran kartı sürücüsü)** Vulkan sürücülerinin Linux dağıtımınızla birlikte **önceden yüklenmiş** olduğu anlamına gelir.
	- Ancak, eğer sayfada **kendi Linux dağıtımınızı göremiyorsanız** ve <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> **NVIDIA** kullanıyorsanız, **farklı bir rehber** bulmanızı veya sayfada bahsedilen **diğer dağıtımlardan birine geçmenizi** tavsiye ederim.

## Oyun oynama yazılımı yükleme
- Linux'ta mevcut olan bazı bilinen oyun oynama yazılımları şunlardır:
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> **|** [Steam](https://store.steampowered.com/)
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **|** [Heroic Games Launcher](https://heroicgameslauncher.com/) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic, **<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7ce5f2d5-e927-4712-ad11-5a4df8281adb" /> Epic Games, <img width="16" height="25" alt="gog" src="https://github.com/user-attachments/assets/552536c7-c66d-42ca-8b43-239bff63d887" /> GOG ve <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f18ba3ba-4418-4153-9201-7f2b1ca4b42f" /> Prime Gaming** platformlarındaki oyunları oynamak için tasarlanmış oldukça yararlı bir oyun oynama yazılımdır.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **|** [Lutris](https://lutris.net/) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris **Windows oyunlarını oynamak için** tasarlanmış, özellik bakımından zengin olan bir oyun oynama yazılımıdır. Lutris aracılığıyla **<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7ce5f2d5-e927-4712-ad11-5a4df8281adb" /> Epic Games, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/93fec16e-9461-4b36-a47c-8242e6259f94" /> Battle.net, <img width="16" height="25" alt="ubisoft" src="https://github.com/user-attachments/assets/5980423e-e2ca-407a-89a5-183715ac83fc" /> Ubisoft vb.** gibi oyun oynama yazılımı platformlarını **doğrudan** yükleyebilirsiniz ama aynı zamanda herhangi bir platforma ait olmayan oyunları ve uygulamaları da yükleyip oynayabilirsiniz.
		- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris, **büyük bir ölçüde** oyun ve yazılım için **topluluk tarafından oluşturulmuş kendiliğinden yükleme dosyaları** da sunar.
		- **DVD oyunları** da dahil olmak üzere, eğer elinizde kurulum dosyanız varsa, oyunlarınızı **elle de** kurabilirsiniz. 
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/86fe080b-77b7-4bc1-9fa5-1afc7eebc39d" /> **|** [ProtonPlus](https://protonplus.vysp3r.com/) **-** **Daha iyi uyumluluk ve performans** için <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> **özel WINE/Proton yapılarını** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/86fe080b-77b7-4bc1-9fa5-1afc7eebc39d" /> ProtonPlus aracılığıyla yükleyebilirsiniz. Özel <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE/Proton yapıları <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam ve <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic tarafından **desteklenmektedir**.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> **|** [Sober](https://sober.vinegarhq.org) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> Sober, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/26dec68d-79c7-4f82-875a-ab1a21bb11f5" /> **Roblox'un** <img width="16" height="25" alt="image-removebg-preview(1)" src="https://github.com/user-attachments/assets/cec27060-1d67-48e1-8f29-a3a5b639fde8" /> Android versiyonunu Linux'ta oynamaya olanak tanıyan bir oyun oynama yazılımıdır. Geçmişte <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/2e1571a7-9ec9-42eb-8238-c6931941b506" /> **VinegarHQ** aracılığıyla <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/26dec68d-79c7-4f82-875a-ab1a21bb11f5" /> Roblox'un Windows versiyonunu oynamak mümkündü. Fakat şu anda **bu destek anti-hile yapılandırması yüzünden kesildi**. Bu yüzden aynı geliştirici ekibi <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cdfc27d4-44f6-4a7a-810a-70ebfde3c440" /> **Sober'ı** geliştirdi.
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> [Prism Launcher](https://prismlauncher.org) **-** <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher, <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> **Minecraft** oynamak için tasarlanmış, özellik açısından zengin bir oyun oynama yazılımıdır. <img width="16" height="25" alt="mc" src="https://github.com/user-attachments/assets/b48ac714-01b3-4aaf-bb00-348e811eb0d5" /> Minecraft'ı yapılandırmak ve performans bakımından en iyi hâle getirmek için yazdığım bir rehberim var. Rehbere [buradan ulaşabilirsiniz](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Minecraft-tr.md).

### ⚠️
- Bu yazılımları **kendi paket yöneticinizden** veya [Flatpak](https://flatpak.org)'ten yükleyebilirsiniz.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam oyunlarınızın Linux'ta oynanabilir olup olmadığını görmek için <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1ee2ed23-e831-463b-8ada-87e8cd5d4fc7" /> [ProtonDB](https://www.protondb.com)'ye bakabilirsiniz.
	- Arattığınız oyun **silver (gümüş) veya daha aşağıda bir kademede** derecelendirilmişse, bu o oyunun **oynanamaz** olduğu anlamına gelir.
	- Oyununuz için herhangi bir değerlendirme yapılmışsa **en iyi hâle getirme tavsiyeleri** alabilirsiniz. İsterseniz, dilediğiniz <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam oyunu hakkında kendi değerlendirmelerinizi de yazabilirsiniz.
# Çift grafikli sistem yapılandırması
- Eğer sisteminizde **iki ekran kartı (1 dahili + 1 harici) varsa**, **her iki donanım için de Vulkan sürücülerini kurmanızı** ve oyunları harici ekran kartınızla çalıştırmanızı tavsiye ederim.
- Oyunları harici <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> **AMD** ekran kartıyla çalıştırmak için aşağıdaki komutu kullanın:
```
DRI_PRIME=1
```
 - Oyunları <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/cf335904-bc37-427e-a86d-c7f9df4bd852" /> **NVIDIA** ekran kartıyla çalıştırmak için aşağıdaki komutu kullanın:
```
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia
```
## Oyunları harici ekran kartıyla çalıştırmanın yolları
- Oyunları harici ekran kartıyla çalıştırmanın **dört yolu** vardır:
	- **1 -** [Terminal yöntemi](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#terminal-method-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/ae34a1ca-71fe-4bf4-b1df-ddee947edaf5" />
 	- **2 -** [Masaüstü kısayolu yöntemi](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main?tab=readme-ov-file#desktop-shortcut-method-%EF%B8%8F) 🖥️
 	- **3 -** [Steam oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-steam-games-) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" />
  	- **4 -** [Lutris & Heroic oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide?tab=readme-ov-file#for-lutris--heroic-games--) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
### Terminal yöntemi <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/814656ce-8cb1-4f5d-bf18-ab56736dc781" />
Kısaca, terminali çalıştırın ve örnekte olduğu gibi ekran kartınız için olan komutu çalıştırın:
```
DRI_PRIME=1 prismlauncher
```
### Masaüstü kısayolu yöntemi 🖥️
- Masaüstünüzde **.desktop** uzantılı bir dosya oluşturun.
- Bu örnek .desktop dosya içeriği <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/f75e206c-3d24-4e00-9d40-ce190c27b9b3" /> NVIDIA ekran kartıyla <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/d627b381-7fa3-4f3e-850a-7d0644116c7b" /> Prism Launcher'ı çalıştırmaktadır. Odaklanmanız gereken satır `Exec` ile başlayan satırdır:
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
- Kısaca, en başa `env` yazmalı ve ardından da **ekran kartınız için olan komutu** yazmalısınız. Son olarak da oyununuzun paket adını yazmalısınız.
### Steam oyunları için <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" />
Örnekte olduğu gibi oyunlarınızın başlatma seçeneklerine ekran kartınız için olan komutu ekleyin. En sona `%command%` yazmayı **unutmayın**:
```
DRI_PRIME=1 %command%
```
- **⚠️ -** Eğer **ek olarak** diğer başlatma seçeneklerini kullanacaksanız ve oyunları harici ekran kartınızla çalıştıracaksanız, tüm komutların örnekte olduğu gibi `%command%` **yer tutucusundan önce** yazıldığından emin olun:
```
DRI_PRIME=1 gamemoderun %command%
```
### Lutris & Heroic oyunları için <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **| Lutris -** Soldaki kısımda `Wine` yazan yere fare imlecinizi götürdükten sonra beliren **ayarlar simgesine** tıklayın.
	- `System Options` **-** `Enable Advanced` **-** `Use Discrete Graphics`
 - <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **| Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# Harici disk yapılandırması
- Harici diskiniz **anakarta bağlıysa**, Linux dağıtımınıza bağlı olarak onu doğrudan kullanabilme ihtimaliniz vardır. Ancak, eğer harici diskinizi **bir SSD kutusu (USB) aracılığıyla** kullanıyorsanız, onu elle yapılandırmalısınız.
- Bu adımlar diskiniz **anakarta bağlı olduğu hâlde düzgün bir şekilde çalışmıyorsa** da geçerlidir.
## Başlangıç: GParted <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/8119e97a-f45c-4859-bbf2-2b9b26b542a5" />
⚠️ - **Kesinlikle ve kesinlikle** diskinizin dosya sistemini **NTFS yerine Linux ile uyumlu başka bir dosya sistemi** olarak değiştirmenizi tavsiye ediyorum çünkü Linux'ta **NTFS için write (yazma) desteği hâlâ deneyseldir** ve bu **diskinizi bozabilir!!!** Bu konuda uyarıldınız.
- Paket yöneticinizi kullanarak `gparted` paketini yükleyin ve harici diskinizin **fiziksel olarak bağlıyken yazılım tarafında bağlı olmadığından emin olarak** sıradaki adımları takip edin:
	- `GParted'ı çalıştırın` **-** `sağ üstten harici diskinizi seçin` **-** `tüm dizinleri silin` **-** `Add`
 	- **Sonra -** `File system: ext4` **-** `Label: istediğiniz herhangi bir başlık` **-** `Add`
  	- **Son olarak -** `Apply All Operations`
## Linux'ta harici diskler nasıl yapılandırılır?
- Öncelikle paket yöneticinizi kullanarak `gnome-disk-utility` paketini yükleyin.
	- Eğer harici diskinizi **NTFS olarak kullanma konusunda ısrar ediyorsanız**, ek olarak paket yöneticinizi kullanarak `ntfs-3g` paketini yükleyin.
- Yükleme sonrasında uygulama başlatıcınızı kullanarak `Disks` uygulamasını çalıştırın.
- Ardından, soldaki menüden harici diskinizi bulun ve `Volumes` kısmının altında bulunan şu tuşa tıklayın.
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- O menüde bulunan `Take Ownership` seçeneğine tıklayıp onay verin.
- Sahiplik yetkisini aldıktan sonra aynı menüyü açın ve `Edit Mount Options` seçeneğine tıklayın.
  - Şimdi `User Session Defaults` seçeneğini devre dışı bırakın ve `Mount at system startup` seçeneğini etkinleştirin.
  - Sonrasında `Symbolic Icon Name` kutusunun altında bulunan ve herhangi bir başlığı olmayan kutuyu bulun ve içinde yalnızca şu başlatma seçeneklerinin olduğundan emin olun:
  	- `nofail,x-gvfs-show,rw,user,exec`
   - Harici diskinizi **NTFS olarak** kullanacaksanız, ek olarak örnekteki gibi `ntfs-3g` seçeneğini de dahil etmelisiniz:
        - `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
   - Son olarak, `Identify As` değerini `/dev/disk/by-label/your-disk` olarak değiştirin ve OK'e tıklayın.
<img width="904" height="493" alt="imagee" src="https://github.com/user-attachments/assets/56cf7ae7-d9f7-42fc-81de-b23b671622d2" />

- Artık harici diskinizi kullanmak için hazırsınız!
# Performans arttırma yöntemleri
## Reducing Game Resolution and Using the Lowest Graphics Settings Oyun çözünürlüğünü düşürme ve en düşük grafik ayarlarını kullanma
- Bir oyunun çözünürlüğünü düşürdüğünüzde **daha az piksel işlenir** ve bu da donanımlarınızda **daha az yük** oluşturarak **daha yüksek performans** almanızı sağlar.
- En düşük grafik ayarlarında oyun oynadığınız zaman **daha az detay işlenir** ve bu da **daha yüksek performans** almanızı sağlar.
- İki yöntem de **görsel kaliteyi düşürürken performansı arttırır**. Kendi dengeli ayarlarınızı bulabilmek için deneyimlemeler yapabilirsiniz.
### Lossless Scaling <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" />
<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" /> [Lossless Scaling](https://store.steampowered.com/app/993090/Lossless_Scaling/) sayesinde oyunlarınızı **görsel kalite kaybı olmadan daha düşük çözünürlüklerde** oynayabilirsiniz. Ancak, uygulamayı kullanabilmek için <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam'den **satın almalısınız**.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/074227ed-e80f-4dea-a770-4866500c5931" /> Lossless Scaling'i satın aldıktan sonra onu Linux'ta kullanabilmek için [lsfg-vk](https://github.com/PancakeTAS/lsfg-vk)'i kurmalısınız.
	- Ancak, bu özelliği kullanabilmek için **ekran kartınızın Vulkan'ı desteklemesi** ve **sisteminizde Vulkan sürücülerinin yüklenmiş olması** şart!
## Performans çekirdeği kullanmak
**Güncel çekirdekler** özel performans çekirdekleriyle kıyaslandıklarında genellikle **düzgün performans** gösterirler. Ancak, **sizde daha iyi performans gösterebileceği ihtimaline karşılık olarak** özel performans çekirdeklerini deneyebilirsiniz.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/943b4b7c-5b29-46aa-b081-b5d5ecc8fec3" /> **| Arch Linux ve çeşitleri:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/48e91252-38ca-4a48-80b8-57423b90c5da" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/95bc6c6d-7d21-4c3a-ac08-31c85ddf8683" /> **| Fedora Linux ve çeşitleri:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/) <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/a3d38d39-481b-4436-b22b-b877acc4a6ea" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/c56a6d0a-133d-4bcf-a594-f4cd8b58e335" /> <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/7960ea90-ac89-4e3a-9839-cd77f9ec2b24" /> **| Debian/Ubuntu Linux ve çeşitleri:** [XanMod Kernel](https://xanmod.org/) <img width="16" height="25" alt="xanmod" src="https://github.com/user-attachments/assets/d3afbdc8-439a-426b-b5b1-9206f03fea05" />
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) oyun esnasında performansı arttırmak için **sistem yapılandırmasında geçici değişiklikler yapan** bir araçtır.
	- Genellikle, <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris gibi oyun oynama yazılımları bunu **kendiliğinden etkinleştirirler**. Fakat <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> Steam'de oyununuzun başlatma seçeneklerine örnekte olduğu gibi **elle bir komut eklemelisiniz**:
```
gamemoderun %command%
```
## Performans arttıran başlatma seçenekleri
Oyun oynarken daha yüksek performans almak için bu başlatma seçeneklerini kullanabilirsiniz:
- `DXVK_LOG_LEVEL=none` **-** **Tüm DXVK günlüklerinin üretimini durdurur**. - *Performansa etkisi orta derecededir*
- `WINEDEBUG=-all` **-** <img width="10" height="25" alt="image" src="https://github.com/user-attachments/assets/465d07fc-c39e-4193-8182-f82eb9fa3464" /> WINE'ın tüm hata ayıklama çıktılarının üretimini durdurur**. - *Performansa etkisi düşüktür*
- `WINE_LARGE_ADDRESS_AWARE=1` **-** **32-bit uygulamalarının 2 GB yerine 4 GB RAM'e kadar bellek kullanabilmelerine** olanak tanır. - *Oyuna bağlı olarak etkisi değişkendir, genellikle orta derecededir*
- `MESA_GLTHREAD=true` **-** <img width="16" height="25" alt="intel" src="https://github.com/user-attachments/assets/315abff4-87d6-4779-b38d-08f07b8237a4" /> <img width="16" height="32" alt="image" src="https://github.com/user-attachments/assets/bea33d54-3560-4d14-a706-6a4edef4e8a6" /> **Intel/AMD ekran kartlarının OpenGL performansını** arttırır. - *Performansa etkisi yüksektir*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** <img width="16" height="28" alt="nvidia" src="https://github.com/user-attachments/assets/cf335904-bc37-427e-a86d-c7f9df4bd852" /> **NVIDIA ekran kartlarının OpenGL performansını** arttırır. - *Performansa etkisi yüksektir*
- `DXVK_ASYNC=1` **-** **Gölgelendiricilerin derlenmesini beklemeden kareleri gösterir**. - *Oyuna bağlı olarak etkisi değişkendir, genellikle düşüktür*
	- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> Lutris ve <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> Heroic'te <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> **Steam oyunlarında çalışmaz**.
 	- Ek olarak, DXVK Async kullanmak **çevrimiçi oyunlardan yasaklanmanıza sebep olabilir**. Bu yüzden bunu yalnızca **çevrimdışı oyunlarda** kullanmanız tavsiye edilir.
### Bu başlatma seçeneklerini nasıl kullanabilirsiniz?
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/e593fe4c-a595-40e2-b2fd-bcd6cb743c7e" /> **| Steam -** Bu komutları daha önceden bahsedildiği üzere başlatma seçeneklerinde kullanabilirsiniz.
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/1e14870a-70af-4e70-833b-6703dd9e9701" /> **| Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />
- <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/cf4a5ae3-5348-4199-bf47-21a1c2efe2df" /> **| Heroic -** `Settings` **-** `Game Defaults` **-** `ADVANCED` **-** `Environment Variables` **-** `+`
<img width="513" height="180" alt="image" src="https://github.com/user-attachments/assets/557adebe-23e7-4c8b-93e2-0378cb38faae" />

## Kompozitörü devre dışı bırakma - YALNIZCA X11 İÇİN GEÇERLİDİR!!! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" />
**⚠️ -** Eğer <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland kullanıyorsanız, kompozitörü devre dışı bırakmak **mümkün değildir**. Bu adımlar yalnızca <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/3dd1cec2-812d-4367-856a-0c008cbd7ede" /> X11 için geçerlidir.
- Devre dışı bırakılmış bir kompozitör kısaca devre dışı bırakılmış animasyonlar ve şeffaflık demektir. Ayrıca, kompozitörü devre dışı bırakmak ekran yırtılmasına sebep olur, bu da **performansı arttırırken görsel kaliteyi azaltır**.
- Bu adım <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" /> [Linux Gaming Wiki'de](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)) açıklanmıştır.
# Kapanış
Bu rehber Linux'ta oyun oynama hakkındaydı. Okuduğunuz için teşekkürler. Umarım bu rehber sisteminizi Linux'ta oyun oynamaya hazır hâle getirme konusunda yardımcı olmuştur. İyi oyunlar! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />

