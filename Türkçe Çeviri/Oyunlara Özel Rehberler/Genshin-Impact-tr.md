# İçindekiler
- [Başlamadan Önce](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#before-starting)
- [Başlangıç](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#get-started)
  - [Performans Arttırma Tavsiyeleri](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#optimization-tips)
    - [Başlatıcı Ayarları](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#launcher-settings)
    - [Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#in-game-settings)
    - [Diğer Oyun İçi Ayarlar](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#other-in-game-settings)
- [Kapanış](https://github.com/cagla-su/Linux-Gaming-Guide/blob/main/Game%20Specific%20Guides/Genshin-Impact-Installation-And-Optimization-Guide.md#conclusion)
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
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/2dea7cf5-a2a4-493a-a45f-9a3e517d6f08" />
<img width="894" height="319" alt="image" src="https://github.com/user-attachments/assets/e915c866-72bd-4064-b8b6-f2ea54ecfd9e" />


- **En iyi performans için** - *Zayıf bilgisayarlar ve en yüksek performans sevenler için*
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/8686b8fc-0e88-41c6-9b96-00500f352eb6" />
<img width="894" height="319" alt="image" src="https://github.com/user-attachments/assets/485e9dd3-1192-4bd5-ba58-2a2604c19f7e" />


- **Görsel kalite ve performans dengesi için** - *Orta özellikli bilgisayarlar için*
<img width="894" height="610" alt="image" src="https://github.com/user-attachments/assets/57e32bf1-8296-4bc4-b602-c596692fa488" />
<img width="894" height="322" alt="image" src="https://github.com/user-attachments/assets/851bba7e-10f2-4796-8d23-e39677ec63a1" />


- **Görsel kalite ve performans dengesi için V2** - *Harici ekran kartı olmayan biraz güçlü işlemciye sahip bilgisayarlar için. Örn. i5-8265U + Intel UHD 620*
<img width="894" height="609" alt="image" src="https://github.com/user-attachments/assets/90fdaa7e-7ff1-4db2-b1ac-f24cad059efa" />
<img width="894" height="318" alt="image" src="https://github.com/user-attachments/assets/51b84c24-c719-411a-9e0d-1cc8eeedd674" />
<img width="894" height="318" alt="image" src="https://github.com/user-attachments/assets/857dd3e4-54a1-4123-9f9e-0b05962dd76e" />

### Diğer Oyun İçi Ayarlar
- `Ayarlar` **-** `Ses` **-** `Dinamik Aralık` **-** `Sınırlı`
- `Ayarlar` **-** `Diğer` **-** `Mini Harita Ayarları` **-** `Sabit`

# Kapanış
Bu rehber Genshin Impact kurulumu ve yapılandırması hakkındaydı. Umarım rehber faydalı olmuştur. Okuduğunuz için teşekkürler, iyi oyunlar! <img width="16" height="25" alt="image" src="https://github.com/user-attachments/assets/60e83c84-d8f8-4035-8052-08aabe1d83a1" />

