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

---
- **En uygun görsel kalite için** - *Oyun oynama bilgisayarları ve güçlü sistemler için*
<img width="897" height="615" alt="image" src="https://github.com/user-attachments/assets/29b57225-0baa-48b6-b77f-2c9c0db16a14" />
<img width="897" height="316" alt="image" src="https://github.com/user-attachments/assets/f6a08a72-31c2-46b4-a783-e637c446be41" />

---
- **En iyi performans için** - *Zayıf bilgisayarlar ve en yüksek performans sevenler için*
<img width="903" height="616" alt="image" src="https://github.com/user-attachments/assets/4fcd73f3-6061-4f50-824c-3391dabea8f1" />
<img width="903" height="320" alt="image" src="https://github.com/user-attachments/assets/c152a7f5-5621-4020-8f30-c74b73402592" />

---
- **Görsel kalite ve performans dengesi için** - *Orta özellikli bilgisayarlar için*
<img width="897" height="611" alt="image" src="https://github.com/user-attachments/assets/5f8c0f59-8164-4af1-afab-1e05c5fea398" />
<img width="897" height="316" alt="image" src="https://github.com/user-attachments/assets/64504d76-9292-42e0-995d-2f77e57178c6" />


---
- **Görsel kalite ve performans dengesi için V2** - *Harici ekran kartı olmayan biraz güçlü işlemciye sahip bilgisayarlar için. Örn. i5-8265U + Intel UHD 620*
<img width="897" height="615" alt="image" src="https://github.com/user-attachments/assets/386ab2ec-f1dc-4a63-8885-6d72e585c00f" />
<img width="896" height="316" alt="image" src="https://github.com/user-attachments/assets/5de943e5-5959-4ce7-bba5-e15906156374" />


### Diğer Oyun İçi Ayarlar
- `Ayarlar` **-** `Ses` **-** `Dinamik Aralık` **-** `Sınırlı`
- `Ayarlar` **-** `Diğer` **-** `Mini Harita Ayarları` **-** `Sabit`

# Kapanış
Bu rehber Genshin Impact kurulumu ve yapılandırması hakkındaydı. Umarım rehber faydalı olmuştur. Okuduğunuz için teşekkürler, iyi oyunlar! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />

