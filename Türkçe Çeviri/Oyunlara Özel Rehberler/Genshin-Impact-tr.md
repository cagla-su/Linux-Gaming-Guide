# İçindekiler
- [Başlamadan Önce](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flamadan-%C3%B6nce)
- [Başlangıç](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flang%C4%B1%C3%A7)
  - [Performans Arttırma Tavsiyeleri](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#performans-artt%C4%B1rma-tavsiyeleri)
    - [Başlatıcı Ayarları](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flat%C4%B1c%C4%B1-ayarlar%C4%B1)
    - [Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#oyun-i%CC%87%C3%A7i-ayarlar)
    - [Diğer Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#di%C4%9Fer-oyun-i%CC%87%C3%A7i-ayarlar)
    - [Aşırı Eski Bilgisayar Kullanıcıları için Tavsiyeler](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#a%C5%9F%C4%B1r%C4%B1-eski-bilgisayar-kullan%C4%B1c%C4%B1lar%C4%B1-i%C3%A7in-tavsiyeler)
- [Kapanış](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#kapan%C4%B1%C5%9F)
# Başlamadan Önce
> [!NOTE]
> - Linux'ta Genshin Impact oynamak için kullanacağımız yazılım [AAGL](https://github.com/an-anime-team/an-anime-game-launcher)'dir.
> - Hazırsanız, başlayalım!
# Başlangıç
- Öncelikle, **AAGL'i başlatın** ve yükleme adımlarını tamamlayın.
> [!NOTE]
> - `Çalıştır` tuşunu gördüğünüzde, **resmi olarak** Genshin Impact **oynamak için hazırsınız** demektir.
> - Ancak, oyunun performansı Windows'takiyle **aynı olmayacaktır**. Bu yüzden performans arttırma tavsiyeleri için rehberin devamını okumak isteyebilirsiniz.
## Performans Arttırma Tavsiyeleri
### Başlatıcı Ayarları
> [!NOTE]
> - Eğer **güçlü bir sisteminiz** varsa başlatıcı ayarları **performansınızı arttırmayabilir**.
> - Ancak **zayıf bir sisteminiz** varsa, küçük değişiklikler oyun deneyiminizi **güçlendirebilir**.
- Başlatıcıdan `Çalıştır` tuşunun yanında bulunan `Ayarlar` simgesine tıklayın.
  - Aşağı kaydırın ve `İstemci davranışı`na gidin.
    - Eğer **en az 16 GB RAM'e** sahipseniz, bu değeri `Gizle` olarak tutabilirsiniz.
    - Eğer **12 GB veya daha az RAM'e** sahipseniz, bu değeri `Kapat` olarak değiştirin.
  - Şimdi `Bileşenler`e gidin ve `Seçilmiş versiyon`un bir `Spritz-CachyOS` yapısı olduğundan emin olun. Eğer değilse, aynı sayfadan yükleyebilirsiniz.
  - Aşağı kaydırın ve `Gplasync`'e gidin.
    - **En son** sürümü yükleyin ve `DXVK sürümü`nüzü yüklediğiniz sürüm olarak değiştirin.
- `Bileşenler`den geriye gidin ve yukarıda bulunan `Geliştirmeler` kısmına gidin.
  - `Wine` bölümünün altından `Eşleme` değerini `Boş` olarak değiştirin.
  - Son olarak, eğer **Wayland** kullanıyorsanız, `WineWayland kullan` seçeneğini etkinleştirin.
    - Wayland'in pencere süslemeleri sizi rahatsız ediyorsa, `Kenarlıksız Pencere`yi etkinleştirin.
  - `Ortam` bölümüne gidin ve ayarlarınızın böyle göründüğünden emin olun:
<img width="570" height="591" alt="image" src="https://github.com/user-attachments/assets/02af318b-7ae7-4838-8925-f813c4cde389" />

## Oyun İçi Ayarlar
- `Ayarlar` **-** `Grafikler`

---
### En Uygun Görsel Kalite: Güçlü Sistemler ve Oyun Oynama Bilgisayarları için
- **Görüntüleme Modu** `:` `Kendi Ekran Çözünürlüğünüz Tam Ekran`
- **FPS** `:` `60`
- **Dikey Senkronizasyon** `:` `Kapalı`
- **Modelleme Çözünürlüğü** `:` `1.0`
- **Gölge Kalitesi** `:` `Orta`
- **Görsel Efektler** `:` `Yüksek`
- **Efekt Kalitesi** `:` `Yüksek`
- **Çevre Ayrıntısı** `:` `Orta`
- **Anti-Aliasing** `:` `FSR2`
- **Hacimsel Işıklandırma** `:` `Açık`
- **Yansımalar** `:` `On`
- **Hareket Bulanıklığı** `:` `Ekstrem`
- **Işıklandırma** `:` `Açık`
- **Kalabalık Yoğunluğu** `:` `Yüksek`
- **Eşli Takım Arkadaşı Etkileri** `:` `Açık`
- **Yüzey Altı Saçılımı** `:` `Yüksek`
- **Doku Filtreleme** `:` `1x`

---
### Kalite ve Performans Dengesi: Orta Özellikli Bilgisayarlar için
- **Görüntüleme Modu** `:` `Kendi Ekran Çözünürlüğünüz Tam Ekran`
- **FPS** `:` `60`
- **Dikey Senkronizasyon** `:` `Kapalı`
- **Modelleme Çözünürlüğü** `:` `0.8`
- **Gölge Kalitesi** `:` `Orta`
- **Görsel Efektler** `:` `Düşük`
- **Efekt Kalitesi** `:` `Orta`
- **Çevre Ayrıntısı** `:` `Düşük`
- **Anti-Aliasing** `:` `FSR2`
- **Hacimsel Işıklandırma** `:` `Açık`
- **Yansımalar** `:` `Açık`
- **Hareket Bulanıklığı** `:` `Orta`
- **Işıklandırma** `:` `Açık`
- **Kalabalık Yoğunluğu** `:` `Yüksek`
- **Eşli Takım Arkadaşı Etkileri** `:` `Açık`
- **Yüzey Altı Saçılımı** `:` `Kapalı`
- **Doku Filtreleme** `:` `1x`

---
### Kalite ve Performans Dengesi: Harici Ekran Kartı Olan Düşük Özellikli Bilgisayarlar için
- **Görüntüleme Modu** `:` `1280x720 Tam Ekran`
- **FPS** `:` `60`
- **Dikey Senkronizasyon** `:` `Kapalı`
- **Modelleme Çözünürlüğü** `:` `0.6`
- **Gölge Kalitesi** `:` `Düşük`
- **Görsel Efektler** `:` `En Düşük`
- **Efekt Kalitesi** `:` `Orta`
- **Çevre Ayrıntısı** `:` `En Düşük`
- **Anti-Aliasing** `:` `FSR2`
- **Hacimsel Işıklandırma** `:` `Kapalı`
- **Yansımalar** `:` `Kapalı`
- **Hareket Bulanıklığı** `:` `Düşük`
- **Işıklandırma** `:` `Açık`
- **Kalabalık Yoğunluğu** `:` `Düşük`
- **Eşli Takım Arkadaşı Etkileri** `:` `Açık`
- **Yüzey Altı Saçılımı** `:` `Kapalı`
- **Doku Filtreleme** `:` `1x`

---
### Kalite ve Performans Dengesi: Harici Ekran Kartı Olmayan Düşük Özellikli Bilgisayarlar için
- **Görüntüleme Modu** `:` `1280x720 Tam Ekran (60 FPS'e yaklaşmak için 960x540 Pencereli'ye düşürün)`
- **FPS** `:` `60 - 720p çözünürlük seçtiyseniz 30'a düşürün`
- **Dikey Senkronizasyon** `:` `Kapalı`
- **Modelleme Çözünürlüğü** `:` `0.6`
- **Gölge Kalitesi** `:` `En Düşük`
- **Görsel Efektler** `:` `En Düşük`
- **Efekt Kalitesi** `:` `Düşük`
- **Çevre Ayrıntısı** `:` `En Düşük`
- **Anti-Aliasing** `:` `FSR2`
- **Hacimsel Işıklandırma** `:` `Kapalı`
- **Yansımalar** `:` `Kapalı`
- **Hareket Bulanıklığı** `:` `Kapalı`
- **Işıklandırma** `:` `Açık`
- **Kalabalık Yoğunluğu** `:` `Düşük`
- **Eşli Takım Arkadaşı Etkileri** `:` `Kısmen Kapalı`
- **Yüzey Altı Saçılımı** `:` `Kapalı`
- **Doku Filtreleme** `:` `1x`

---
### En Yüksek Performans: Aşırı Eski Bilgisayarlar ve Düşük Grafiklerde Oynamayı Sevenler için
- **Görüntüleme Modu** `:` `1280x720 Tam Ekran (sisteminiz zorlanıyorsa 960x540 Pencereli'ye düşürün)`
- `Diğer tüm ayarları mümkün olan en düşük ayara çekin`
- Eğer düşük özellikli bir sisteme sahipseniz, en aşağıda bulunan `Uyumluluk Modu`na tıklayın ve **başka hiçbir şeyi değiştirmeyin**.
  - Bu seçenek **ekran kartı yükünün** bir kısmını **işlemciye devreder**. Bu seçenek Genshin Impact oynarken **ekran kartı darboğazı** sorunu yaşayan sistemler için **faydalıdır**. Ancak, **ekran kartı darboğazı sorunu** yaşamayan bir sisteme sahipseniz, modern iyileştirmelerden **yararlanamazsınız** ve bu **düşük performans**a sebep olur. O yüzden bu seçeneği gerçekten ihtiyacınız varsa kullanın.
## Diğer Oyun İçi Ayarlar
- `Ayarlar` **-** `Ses` **-** `Dinamik Aralık` **-** `Sınırlı`
- `Ayarlar` **-** `Diğer` **-** `Mini Harita Ayarları` **-** `Sabit`
## Aşırı Eski Bilgisayar Kullanıcıları için Tavsiyeler
- En iyi performansı alabilmek için, özellikle sisteminizde sadece **dahili bir ekran kartı** varsa, **CachyOS XFCE** kullanmalısınız ve **kompozitörü devre dışı** bırakmalısınız.
  - CachyOS içinden `SchedExt GUI Manager`ı çalıştırın ve `scx_lavd` yöntemini seçtikten sonra `Gaming` profilini seçin. **Değişiklikleri kaydetmeyi** unutmayın.
  - Son olarak, `CachyOS Hello` **-** `Uygulamalar/İyileştirmeler` **-** `Install VRAM Management`
# Kapanış
Bu rehber Genshin Impact kurulumu ve yapılandırması hakkındaydı. Umarım rehber faydalı olmuştur. Okuduğunuz için teşekkürler, iyi oyunlar!

