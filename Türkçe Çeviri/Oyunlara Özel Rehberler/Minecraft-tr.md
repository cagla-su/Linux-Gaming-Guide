# Minecraft
Minecraft **OpenGL** ile çalışan **Linux uyumlu** bir sandbox oyunudur.
## Başlangıç
Öncelikle, [Prism Launcher](https://github.com/PrismLauncher/PrismLauncher) kullanmanızı öneriyorum çünkü Prism Launcher **açık kaynaktır** ve resmi Minecraft başlatıcısından daha fazla seçenek sunmaktadır.
### Prism Launcher kurulumu
Prism Launcher'ı yükleme adımlarına [buradaki bağlantıdan](https://prismlauncher.org/download/?from=button) ulaşabilirsiniz.
### Java kurulumu
Prism Launcher sizin için Java'yı otomatik olarak kurar.
### Minecraft kurulumu
- Prism Launcher'ı çalıştırın ve **hafıza paylaşımı** adımına kadar devam edin.
- Ardından, `En fazla hafıza paylaşımı` değerini değiştirdiğinizden emin olun. İnternette oyuna RAM'inizin yarısı kadar RAM paylaştırırsanız iyi performans alacağınıza dair bir söylenti var. Fakat bu yanlıştır çünkü:
  - Minecraft oynarken oyun, daha doğrusu Java, hafıza sorunlarını önlemek için nesneler tarafından artık kullanılmayan paylaşılan hafızayı temizlemeye çalışır. Buna **garbage collection (çöp toplama)** denir.
    - Ancak, **çok fazla veya çok az** RAM **paylaştırmamalısınız** çünkü:
      - Eğer **çok fazla** RAM paylaştırırsanız, Java çöp toplama döngüleri arasında daha fazla bekleyecek ve her döngünün tamamlanması daha uzun sürecek. Bundan dolayı daha büyük takılmalarla karşılaşacaksınız.
      - Eğer **çok az** RAM paylaştırırsanız, Java çöp toplama işlemini daha sık gerçekleştirecek ve bu da büyük takılmalara sebep olacak.
    - Minecraft'ın paylaştırılan RAM'in `50-75%`'ini kullanması daha küçük takılmaların olması için ideal bir ölçüdür. Kendi ideal değerinizi bulmanız için farklı değerleri deneyimlemenizi tavsiye ediyorum. Oyun esnasında `F3`'e basarak RAM kullanımını görebilirsiniz.
- Hızlı kurulumu tamamladıktan sonra, başlatıcı içinde Microsoft hesabınızla giriş yapın.
- **Sonra** : `Oturum Ekle` **-** `Sürüm` **-** `Dilediğiniz sürümü seçin ve aşağı kaydırın` **-** `Mod yükleyici olarak "Fabric"i seçin` **-** `Tamam`
## Optimizasyon
- `Ayarlar` **-** `Minecraft` **-** `İnce Ayarlar` **-** `Feral GameMode'u etkinleştir` **&** `Ayrık GPU kullan (yalnızca iki ekran kartınız varsa)`
- `Ayarlar` **-** `Ortam Değişkenleri` **-** `Ekle` **-** `mesa_glthread=true`
<img width="731" height="96" alt="image" src="https://github.com/user-attachments/assets/3cd34257-d1cf-4509-8967-d8499e61318a" />

- NVIDIA kullanıyorsanız, onun yerine `__GL_THREADED_OPTIMIZATIONS=1` ortam değişkenini kullanmalısınız.
- Şu an Minecraft oynamak için hazırsınız. Ancak, oyunun performansı yine de performans modları ve iyileştirilmiş oyun içi ayarlarla arttırılabilir.
## Sodium yöntemi - 1.16.3 ve sonraki sürümler için tavsiye edilir
- `Minecraft oturumunuza sağ tıklayın` **-** `Düzenle` **-** `Modlar` **-** `Modları indir`
- **Tavsiye ettiğim performans modları ve bağımlılıkları**
  - `Almanac`
  - `Alternate Current`
  - `AsyncParticles`
  - `BadOptimizations`
  - `Better Biome Reblend`
  - `Cloth Config`
  - `Clumps`
  - `Concurrent Chunk Management Engine`
  - `Dynamic FPS`
  - `EntityCulling`
  - `Fabric API`
  - `Fabric Language Kotlin`
  - `Fast Item Frames`
  - `FastQuit`
  - `FerriteCore`
  - `Forge Config API Port`
  - `Fzzy Config`
  - `ImmediatelyFast`
  - `Krypton`
  - `Ksyxis`
  - `Let Me Despawn`
  - `Lithum`
  - `Model Gap Fix`
  - `No Telemetry`
  - `Noisium`
  - `OptiGUI`
  - `PacketFixer`
  - `Particle Core`
  - `Puzzles Lib`
  - `Reese's Sodium Options`
  - `Remove Reloading Screen`
  - `Sodium`
  - `Sodium Extra`
### Optifine kullanmadan Optifine özellikleri
Optifine'da performans arttırma hakkında olmayan diğer güzel özellikler vardır. Örneğin **yakınlaştırma, shader kullanabilme, dinamik ışıklandırma ve bağlı dokular (cam vb.)**. Aynı özelliklere Optifine kullanmadan aşağıdaki modlar sayesinde erişebilirsiniz:
- **Yakınlaştırma özelliği -** `Zoomify`
- **Shader kullanabilme özelliği -** `Iris`
- **Dinamik ışıklandırma özelliği -** `LambDynamicLights`
- **Bağlı dokular özelliği -** `Continuity`
### Sodium - oyun içi iyileştirilmiş ayarlar
- **Zoomify kullanıyorsanız :** `Ayarlar` **-** `Kontroller` **-** `Tuş Atamaları` **-** `"Araç Çubuğu Kaydetme Etkinleştiricisi"nin değerini herhangi bir şey yapın` **-** `Bitti`
- `Ayarlar` **-** `Kaynak Paketleri` **-** `"Default Connected Textures" ve "Glass Pane Culling Fix"i sağ tarafa taşıyın` **-** `Bitti`
- `Ayarlar` **-** `Görüntü Ayarları`
  - **Genel**
    - `Görüş Mesafesi` **:** 6 yığın
    - `Simülasyon Mesafesi` **:** 5 yığın
    - `Dikey Senkronizasyon` **:** KAPALI
    - `En Fazla Kare Hızı` **:** **Monitörünüzün yenileme hızıyla** aynı değeri girin. Eğer monitörünüzün yenileme hızı **144 Hz'den düşükse** ya *sınırsız* olarak değiştirin (aşırı ısınmaya yol açabilir) ya da *monitörünüzün yenileme hızının iki katı* bir değer seçin (örneğin 60 Hz ekran için 120 FPS).
  - **Kalite**
    - `Grafikler` **:** Hızlı
    - `Bulutlar` **:** KAPALI
    - `Hava Durumu` **:** Hızlı
    - `Leaves (Yapraklar)` **:** Hızlı
    - `Parçacıklar` **:** Azaltılmış
    - `Biyom Karışımı` **:** 1 block(s)
    - `Varlık Mesafesi` **:** 50%
    - `Varlık Gölgeleri` **:** KAPALI
    - `Çarpıtma Efektleri` **:** 60%
    - `Görüş Açısı Efektleri` **:** 60%
    - `Mipmap Düzeyleri` **:** 1x
## Optifine yöntemi - 1.16.2 ve önceki sürümler için tavsiye edilir
- Optifine kullanmak istiyorsanız **resmi Minecraft başlatıcısını** kullanmanızı tavsiye ediyorum çünkü Optifine'ı Prism Launcher aracılığıyla kullanmak hem zor hem de anlamsız olacaktır.
- Kısaca, oynamak istediğiniz sürümü bir kez çalıştırın ve [Optifine'ın](https://optifine.net/downloads) oynamak istediğiniz Minecraft sürümüyle uyumlu olan bir sürümünü indirin. Son olarak, indirdiğiniz **.jar** dosyasını çalıştırdıktan sonra `Yükle`'ye tıklayın. 
### Optifine - oyun içi iyileştirilmiş ayarlar
- `Ayarlar`
  - **Görüntü Ayarları**
    `Grafikler` **:** Hızlı
    - `Yumuşak Aydınlatma` **:** En Fazla
    - `Pürüzsüz Gölgelendirme` **:** 50%
    - `Görüş Mesafesi` **:** 6 yığın
    - `Simülasyon Mesafesi` **:** 5 yığın
    - `Maks. Kare Hızı` **:** **Monitörünüzün yenileme hızıyla** aynı değeri girin. Eğer monitörünüzün yenileme hızı **144 Hz'den düşükse** ya *sınırsız* olarak değiştirin (aşırı ısınmaya yol açabilir) ya da *monitörünüzün yenileme hızının iki katı* bir değer seçin (örneğin 60 Hz ekran için 120 FPS).
    - **Kalite...**
      - `Mipmap Düzeyleri` **:** 1
      - `Işık Yayan Dokular` **:** KAPALI
      - `Özel Yazı Tipi` **:** KAPALI
      - `Bağlı Dokular` **:** Hızlı
      - `Özel Gökyüzü` **:** KAPALI
      - `Özel Varlık Modelleri` **:** KAPALI
      - `Özel Renkler` **:** KAPALI
      - `Doğal Dokular` **:** KAPALI
      - `Özel Eşyalar` **:** KAPALI
      - `Özel Arayüzler` **:** KAPALI
    - **Detaylar...**
      - `Bulutlar` **:** KAPALI
      - `Ağaçlar` **:** Hızlı
      - `Sis` **:** KAPALI
      - `Atılan Eşyalar` **:** Hızlı
      - `Vinyet` **:** Hızlı
      - `Bataklık Renkleri` **:** KAPALI
      - `Yağmur & Kar` **:** Hızlı
      - `Yıldızlar` **:** İsteğe bağlı
      - `Varlık Gölgeleri` **:** KAPALI
      - `Alternatif Bloklar` **:** KAPALI
      - `Biyom Karışımı` **:** 3x3
    - **Performans...**
      - `Kare Hızını Dengeleme` **:** AÇIK
      - `Hızlı İşleme` **:** AÇIK
      - `Bölgesel İşleme` **:** KAPALI
      - `Akıllı Animasyonlar` **:** AÇIK
      - `Hızlı Hesap` **:** AÇIK
    - **Animasyonlar...**
      - `Doku Animasyonları` **:** KAPALI
      - `Parçacıklar` **:** Azaltılmış
# Son
Bu rehber, Linux'ta Minecraft kurulumu ve optimizasyonu hakkındaydı. Okuduğunuz için teşekkürler, iyi oyunlar! 🐧
