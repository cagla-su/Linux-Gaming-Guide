# İçindekiler
- [Başlamadan Önce](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flamadan-%C3%B6nce)
- [Başlangıç](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flang%C4%B1%C3%A7)
  - [Performans Arttırma Tavsiyeleri](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#performans-artt%C4%B1rma-tavsiyeleri)
    - [Başlatıcı Ayarları](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#ba%C5%9Flat%C4%B1c%C4%B1-ayarlar%C4%B1)
    - [Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#oyun-i%CC%87%C3%A7i-ayarlar)
    - [Diğer Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#di%C4%9Fer-oyun-i%CC%87%C3%A7i-ayarlar)
- [Kapanış](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/T%C3%BCrk%C3%A7e%20%C3%87eviri/Oyunlara%20%C3%96zel%20Rehberler/Genshin-Impact-tr.md#kapan%C4%B1%C5%9F)
# Başlamadan Önce
> [!NOTE]
> - Linux'ta <img width="16" height="25" alt="GI" src="https://github.com/user-attachments/assets/5b348860-e317-42c5-b684-275fa9187545" /> Genshin Impact oynamak için kullanacağımız yazılım <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f50ef5c1-e0e0-4ab8-9a38-b687b8f9c08c" /> [AAGL](https://github.com/an-anime-team/an-anime-game-launcher)'dir.
> - Hazırsanız, başlayalım!
# Başlangıç
- Öncelikle, **<img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/f50ef5c1-e0e0-4ab8-9a38-b687b8f9c08c" /> AAGL'i başlatın** ve yükleme adımlarını tamamlayın.
> [!NOTE]
> - `Çalıştır` tuşunu gördüğünüzde, **resmi olarak** <img width="16" height="25" alt="GI" src="https://github.com/user-attachments/assets/5b348860-e317-42c5-b684-275fa9187545" /> Genshin Impact **oynamak için hazırsınız** demektir.
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
  - Şimdi `Bileşenler`e gidin ve `Seçilmiş versiyon`un bir `Spritz-Wine-TKG` yapısı olduğundan emin olun. Eğer değilse, aynı sayfadan yükleyebilirsiniz.
  - Aşağı kaydırın ve `Gplasync`'e gidin.
    - **En son** sürümü yükleyin ve `DXVK sürümü`nüzü yüklediğiniz sürüm olarak değiştirin.
- `Bileşenler`den geriye gidin ve yukarıda bulunan `Geliştirmeler` kısmına gidin.
  - `Wine` bölümünün altından `Eşleme` değerini `Boş` olarak değiştirin ve `Ortam`a gidin.
  - `Ortam` bölümünde ayarlarınızın böyle göründüğünden emin olun:
<img width="581" height="547" alt="image" src="https://github.com/user-attachments/assets/f94d0e3f-7b2c-44cc-885b-16c13f3c695e" />

> [!NOTE]
> - Eğer <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland **kullanmıyorsanız** `env -u DISPLAY %command%` kısmını **dahil etmeyin**.
>   - Eğer <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> Wayland kullanıyorsanız ve <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/6f97a779-0aa8-4ce8-adb0-ed680534e9af" /> **Wayland'in pencere süslemesi sizi rahatsız ediyorsa**, geri dönüp `Wine` bölümünün altında bulunan `Köşesiz Pencere` seçeneğini etkinleştirin.

### Oyun İçi Ayarlar
- `Esc` **-** `Ayarlar` **-** `Grafikler`


- **En uygun görsel kalite için** - *Oyun oynama bilgisayarları ve güçlü sistemler için*
<img width="903" height="613" alt="image" src="https://github.com/user-attachments/assets/b153c20e-4eab-4f25-ba4c-ce89fe4a8a89" />
<img width="903" height="316" alt="image" src="https://github.com/user-attachments/assets/4ac238a9-dcc6-4133-81c4-292bf8bbbe2e" />


- **En iyi performans için** - *Zayıf bilgisayarlar ve en yüksek performans sevenler için*
<img width="903" height="616" alt="image" src="https://github.com/user-attachments/assets/4fcd73f3-6061-4f50-824c-3391dabea8f1" />
<img width="903" height="320" alt="image" src="https://github.com/user-attachments/assets/c152a7f5-5621-4020-8f30-c74b73402592" />


- **Görsel kalite ve performans dengesi için** - *Orta özellikli bilgisayarlar için*
<img width="903" height="615" alt="image" src="https://github.com/user-attachments/assets/72f7c7e8-4e29-4f4c-aa76-6ddc5a8fffa9" />
<img width="903" height="318" alt="image" src="https://github.com/user-attachments/assets/d2501720-41dd-43a5-a61f-d542fa18844e" />


- **Görsel kalite ve performans dengesi için V2** - *Harici ekran kartı olmayan biraz güçlü işlemciye sahip bilgisayarlar için. Örn. i5-8265U + Intel UHD 620*
<img width="903" height="609" alt="image" src="https://github.com/user-attachments/assets/00b836b0-6b0b-45a7-a1f6-8199ce1891fd" />
<img width="903" height="319" alt="image" src="https://github.com/user-attachments/assets/df0ab682-26ac-4ee9-a8b2-b65a62853945" />


### Diğer Oyun İçi Ayarlar
- `Ayarlar` **-** `Ses` **-** `Dinamik Aralık` **-** `Sınırlı`
- `Ayarlar` **-** `Diğer` **-** `Mini Harita Ayarları` **-** `Sabit`

# Kapanış
Bu rehber Genshin Impact kurulumu ve yapılandırması hakkındaydı. Umarım rehber faydalı olmuştur. Okuduğunuz için teşekkürler, iyi oyunlar! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />

