# İçindekiler
- [Linux'ta oyunlar nasıl çalışır?](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#linuxta-oyunlar-nas%C4%B1l-%C3%A7al%C4%B1%C5%9F%C4%B1r)
- [Vulkan sürücülerini yükleme](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#vulkan-s%C3%BCr%C3%BCc%C3%BClerini-y%C3%BCkleme)
- [Oyun oynama yazılımı yükleme](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#oyun-oynama-yaz%C4%B1l%C4%B1m%C4%B1-y%C3%BCkleme)
- [Hibrit grafik sistemi yapılandırması](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#hibrit-grafik-sistemi-yap%C4%B1land%C4%B1rmas%C4%B1)
- [Harici disk yapılandırması](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#harici-disk-yap%C4%B1land%C4%B1rmas%C4%B1)
- [Optimizasyon tavsiyeleri](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#optimizasyon-tavsiyeleri)
## Oyunlara Özel Rehberler
- ![Metin2](https://github.com/user-attachments/assets/c887fc49-cc62-4450-81ab-7ebdfe0087df) **Metin2 -** [Metin2 Linux rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Metin2-tr.md)
-  ![Minecraft](https://github.com/user-attachments/assets/3dd086b5-0be3-4cc9-ab2f-e01243845930) **Minecraft -** [Minecraft Linux rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Minecraft-tr.md)
- ![Sims 2](https://github.com/user-attachments/assets/5e79e395-066b-46df-85a4-a72f73d8aad8) **The Sims 2 -** [The Sims 2 Linux rehberi](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/The-Sims-2-tr.md)
# Linux'ta oyun oynama rehberi
Merhaba. Bu rehberde **Linux'ta oyunların nasıl çalıştığı**, **sisteminizi Linux'ta oynamaya hazır hale nasıl getirebileceğiniz** ve **Linux sisteminizi daha yüksek performans için nasıl optimize edebileceğiniz** konuları hakkında bilgilendirileceksiniz. Hazırsanız, başlayalım!
## Başlamadan önce
- Linux, oyun oynama konusunda hızlı bir şekilde geliştiriliyor. Her geçen gün, daha fazla kullanıcı Linux'a geçmeye başlıyor. Ayrıca, Linux'un piyasa payı da bu bağlamda artıyor.
- Bu rehber Linux'ta oyun oynamak isteyip nereden başlayacağını bilmeyen herkes için kullanışlı olmayı amaçlıyor.
- Son olarak, Linux kullanırken sistem dilini İngilizce yapmanızda fayda var çünkü genel olarak Türkçe çeviriler eksiktir ve bazı uygulamalarda bazı yazılar Türkçe iken bazı yazılar İngilizce görünebilir.
- Bu rehberi okuduktan sonra içinde oynamak istediğiniz bir oyun varsa, [Oyunlara Özel Rehberleri](https://github.com/cagla-su/Linux-Gaming-Guide/tree/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler) de okumanızı tavsiye ediyorum.
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
- NVIDIA **4xxx** ve **5xxx** modelleri için **özel mülkiyet** sürücülerini **aşamalı olarak devre dışı bırakıyor**, çünkü NVIDIA **son çıkan ve gelecekteki kartları için daha fazla açık kaynak** olmaya çalışıyor. Ancak **daha eski kartlar için** hâlâ **özel mülkiyet** sürücüleri kullanmalısınız. Böylece **daha iyi uyumluluk ve performansa** sahip olursunuz. 
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
	- **1 -** [Terminal yolu](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#terminal-yolu)
 	- **2 -** [Masaüstü kısayol yolu](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#masa%C3%BCst%C3%BC-k%C4%B1sayol-yolu)
 	- **3 -** [Steam oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#steam-oyunlar%C4%B1-i%C3%A7in)
  	- **4 -** [Lutris/Heroic oyunları için](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/linuxta-oyun-oynama-rehberi.md#lutrisheroic-oyunlar%C4%B1-i%C3%A7in)
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
Ekran kartınız için olan komutu oynamak istediğiniz oyunların başlatma seçeneklerine ekleyin. Sonuna örnekteki gibi %command% eklemeyi unutmayın:
```
DRI_PRIME=1 %command%
```
- **NOT**: Eğer gamemode kullanacaksanız ve oyunlarınızı harici ekran kartınızla çalıştıracaksanız, bütün komutların `%command%`'den önce yazıldığından emin olun:
```
DRI_PRIME=1 gamemoderun %command%
```
### Lutris/Heroic oyunları için
- **Lutris -** Sol yan menüde, `Wine` yazan yere fare imlecini götürdükten sonra çıkan ayarlar butonuna tıklayın.
	- `System Options` **-** `Enable Advanced` **-** `Use Discrete Graphics`
 - **Heroic -** `Settings` **-** `Game Defaults` **-** `Other` **-** `Use Dedicated Graphics Card`
# Harici disk yapılandırması
- Harici diskiniz **anakarta doğrudan bağlıysa**, Linux dağıtımınıza bağlı olarak **ek yapılandırma gerektirmeden** çalıştırabilirsiniz. Ancak, harici diskiniz **SSD kutusu (USB)** aracılığıyla bağlıysa onu el ile yapılandırmalısınız.
- Aynı adımlar diskiniz **anakarta doğrudan bağlıysa** fakat **yine de kullanamıyorsanız geçerli olmalıdır**.
## Başlangıç: GParted
- Diskinizin dosya sistemini **NTFS'ten Linux uyumlu olan bir dosya sistemiyle** değiştirmek için biçimlendirmek isterseniz, paket yöneticiniz aracılığıyla `gparted` paketini yükleyin ve harici diskinizin hâla bağlıyken sistem tarafından bağlanmamış olduğundan emin olun.
	- `GParted'ı çalıştırın` **-** `sağ üstten harici diskinizi seçin` **-** `tüm bölümleri silin` **-** `Add`
 	- **Sonra:** `File system: ext4` **-** `Label: istediğiniz herhangi bir başlık` **-** `Add`
  	- **Son olarak:** `Apply All Operations`
## Linux'ta harici diskler nasıl yapılandırılır?
- Öncelikle, paket yöneticiniz aracılığıyla `gnome-disk-utility` paketini yükleyin.
	- Ayrıca, daha önceden Windows'ta kullandığınız harici diskinizi kullanacaksanız, diğer bir deyişle **NTFS olarak** kullanacaksanız, paket yöneticiniz aracılığıyla `ntfs-3g` paketini yükleyin.
- Yükleme bittikten sonra uygulama başlatıcınızdan `Disks` uygulamasını çalıştırın.
- Sonrasında, sol taraftaki menüden harici diskinizi bulun ve `Volumes` kısmının altında bulunan şu butona tıklayın:
<img width="258" height="192" alt="imageee" src="https://github.com/user-attachments/assets/4eee726f-25e2-42d1-9051-22ab18bd08d0" />

- Çıkan menüden `Take Ownership`'e tıklayın ve onaylayın.
- Sahiplik yetkisini aldıktan sonra aynı menüyü açın ve `Edit Mount Options`'a tıklayın.
  - Şimdi `User Session Defaults`'u devre dışı bırakın ve `Mount at system startup`'ı etkin hale getirin.
  - Ardından, `Symbolic Icon Name` kutusunun altında bulunan ve bir başlığı olmayan kutuyu bulup içeriğinde yalnızca bu seçeneklerin olduğundan emin olun:
  	- `nofail,x-gvfs-show,rw,user,exec`
   - Eğer daha önceden Windows'ta kullandığınız harici diskinizi kullanacaksanız, diğer bir deyişle **NTFS olarak** kullanacaksanız, ayrıyeten şu seçeneği de ekleyin:
        - `nofail,x-gvfs-show,rw,user,exec,ntfs-3g`
   - Son olarak, `Identify As` değerini `/dev/disk/by-label/diskinizin-adi` olarak ayarlayıp değişiklikleri kaydedin.
<img width="904" height="493" alt="imagee" src="https://github.com/user-attachments/assets/56cf7ae7-d9f7-42fc-81de-b23b671622d2" />

- Artık harici diskinizi kullanmak için hazırsınız!
# Optimizasyon tavsiyeleri
## Oyun çözünürlüğünü düşürmek ve en düşük grafik ayarlarını kullanmak
- Oyunun çözünürlüğünü düşürdüğünüzde daha az piksel işlenecek ve bu donanımlarınıza daha az yük bindirerek daha yüksek performans almanızı sağlayacak.
- En düşük grafik ayarlarıyla oyun oynadığınızda daha az detay işlenecek ve daha yüksek performans almanızı sağlayacak.
- İkisi de görsel kaliteyi düşürürken performansı arttıracaktır. Kendi dengeli ayarlarınızı bulmak için deneyler yapabilirsiniz.
## Performans çekirdeği kullanmak
- **Arch Linux ve Arch Linux tabanlı Linux dağıtımları için:** [CachyOS Kernel](https://github.com/CachyOS/linux-cachyos)
- **Fedora Linux ve Fedora Linux tabanlı Linux dağıtımları için:** [CachyOS Kernel Port For Fedora](https://copr.fedorainfracloud.org/coprs/bieszczaders/kernel-cachyos/)
- **Debian/Ubuntu Linux ve Debian/Ubuntu Linux tabanlı Linux dağıtımları için:** [XanMod Kernel](https://xanmod.org/)
## Gamemode
- [Gamemode](https://github.com/FeralInteractive/gamemode) siz oyun oynarken performansı arttırmak için sistem ayarlarınızda **geçici olarak** değişiklikler yapan bir araçtır. Genellikle Lutris gibi oyun oynama yazılımları bunu varsayılan olarak etkinleştirir. Fakat Steam'de örnekteki gibi oyununuzun başlatma seçeneklerine bir komut eklemelisiniz:
```
gamemoderun %command%
```
- Gamemode'u yükledikten sonra, [gamemode.ini](https://github.com/FeralInteractive/gamemode/blob/master/example/gamemode.ini) dosyasını indirin ve dosyayı terminalinizi "İndirilenler" dizininde açtıktan sonra `/etc` konumuna taşıyın:
```
sudo mv gamemode.ini /etc/
```
## Performans arttıran çevre değişkenleri
Oyun oynarken daha iyi performans için bu çevre değişkenlerini kullanabilirsiniz:
- `WINEDEBUG=-all` **-** WINE'ın bütün hata ayıklama çıktılarını engeller. - *performansa etkisi düşük*
- `mesa_glthread=true` **-** **Intel/AMD ekran kartlarında OpenGL performansını** arttırır. - *performansa etkisi yüksek*
- `__GL_THREADED_OPTIMIZATIONS=1` **-** **NVIDIA ekran kartlarında OpenGL performansını** arttırır. - *performansa etkisi yüksek*
- `DXVK_ASYNC=1` **-** **Steam oyunlarında işe yaramaz** ancak **gölgelendiricilerin derlenmesini beklemeden kareleri gösterir** ve bu Lutris ile Heroic'te çalışır. Ancak, async kullanmak **oynadığınız çevrimiçi oyunlardan yasaklanmanıza sebep olabilir**. Bu yüzden bu yalnızca **çevrimdışı oyunlar** için önerilir. - *oyuna bağlı olarak performansa etkisi düşük*
### Bu çevre değişkenlerini nasıl kullanabilirsiniz?
- **Steam -** Oynamak istediğiniz oyunların başlatma seçeneklerinde bu komutları kullanabilirsiniz. En sona `%command%` eklemeyi unutmayın.
- **Lutris -** `System Options` **-** `Environment Variables` **-** `Add`
<img width="811" height="278" alt="image" src="https://github.com/user-attachments/assets/fda799aa-a02d-408c-9d0e-54c3a19dca1a" />

## Ekran kompozisyonunu devre dışı bırakmak - YALNIZCA X11 İÇİN!!!
**UYARI**: Eğer **Wayland** kullanıyorsanız, ekran kompozisyonunu devre dışı **bırakamazsınız**. Bu adımlar yalnızca **X11** için geçerlidir.
- A disabled compositor simply means disabled animations and transparency. Also, it causes screen tearing which **reduces visual quality while improving performance**. Devre dışı bırakılmış bir ekran kompozisyonu kısaca devre dışı bırakılmış animasyonlar ve saydamlık demektir. Ayrıca, ekran yırtılmasına sebep olur ve bu **performansı arttırırken görsel kaliteyi düşürür**.
- Bu adım [bu rehberde](https://linux-gaming.kwindu.eu/index.php?title=Compositor_(X11)) anlatılmıştır.
# Son
Bu rehber Linux'ta oyun oynama hakkındaydı. Umarım bu rehber sizin için faydalı olmuştur. Okuduğunuz için teşekkürler, iyi oyunlar! 🐧


