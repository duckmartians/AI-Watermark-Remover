# AI Watermark Remover — Kullanıcı Kılavuzu

<p align="left">
  <a href="/releases/latest">
    <img src="https://img.shields.io/badge/Windows-%F0%9F%92%BB-0078D6?style=for-the-badge&logo=windows&logoColor=white">
  </a>
  <a href="/releases/latest">
    <img src="https://img.shields.io/badge/macOS-%F0%9F%8D%8E-000000?style=for-the-badge&logo=apple&logoColor=white">
  </a>
</p>
<p align="left">
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3">
    <img src="https://img.shields.io/badge/Windows-Drive%20backup-4285F4?style=flat-square&logo=googledrive&logoColor=white">
  </a>
  <a href="https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l">
    <img src="https://img.shields.io/badge/macOS-Drive%20backup-4285F4?style=flat-square&logo=googledrive&logoColor=white">
  </a>
</p>
<p align="left">
  <a href="https://duckmartians.info">
    <img src="https://img.shields.io/badge/Homepage-Visit-0A66C2?style=flat-square&logo=google-chrome&logoColor=white">
  </a>
  <a href="https://discord.gg/munMZEBMw5">
    <img src="https://img.shields.io/badge/dynamic/json?url=https://discord.com/api/guilds/1369302820037201981/widget.json&query=$.presence_count&label=Discord&color=5865F2&logo=discord&style=flat-square">
  </a>
</p>

🌐 [English](README.md) · [Tiếng Việt](README.vi.md) · [বাংলা](README.bn.md) · [हिन्दी](README.hi.md) · [Português (BR)](README.pt_BR.md) · [Русский](README.ru.md) · **Türkçe** · [اردو](README.ur.md) · [简体中文](README.zh_CN.md)

Bu uygulama, **logoları, filigranları, imzaları ve metin katmanlarını görüntülerden ve videolardan kaldırmanıza** yardımcı olur.
Sadece **kaldırmak istediğiniz alanın üzerini boyayın**, uygulama da o bölgeyi doğal bir şekilde geri doldursun. Her şey
**kendi bilgisayarınızda** çalışır — **internet gerekmez** ve görüntüleriniz/videolarınız **hiçbir yere yüklenmez**.

---
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/dbcb0fad-cc38-49d6-b9c6-acd1c0e16983" />
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/f07d1f33-e835-4c6c-b5b6-6b8db94b9cb9" />

## Kurulum ve Açma

1. Kurulum dosyasını çalıştırın (veya sıkıştırılmış bir arşiv aldıysanız klasörü açın).
2. **AI Watermark Remover** uygulamasını açın (Masaüstünden, Başlat menüsünden veya `.exe` dosyasından).

> **Windows "Windows protected your PC" (Windows bilgisayarınızı korudu) uyarısını mı gösteriyor?**
> Bu, ücretli bir imzalama sertifikası olmayan uygulamalar için gösterilen varsayılan uyarıdır — **bir virüs değildir**.
> Açmak için **More info → Run anyway** (Daha fazla bilgi → Yine de çalıştır) seçeneğine tıklayın.

İlk açılış biraz daha uzun sürebilir; sonraki açılışlar daha hızlıdır.

**İki sürüm vardır:** **Pro** sürümü (görüntüler + video) ve **Lite** sürümü (yalnızca görüntüler, daha hafif).
Aralarındaki farkı anlamak için pencere başlığına bakın: **"Pro"** = tam sürüm, **"Lite"** = hafif sürüm (video açamaz).

---

## Nasıl kullanılır — 4 adım

### Adım 1 — Bir görüntü/video açın
- Bir veya birden fazla dosya seçmek için **belge** düğmesine, ya da bütün bir klasörü açmak için **klasör** düğmesine tıklayın.
- Veya görüntüleri/videoları doğrudan pencerenin içine **sürükleyip bırakın**.
- Birden fazla dosyayla, alt kısımda bir küçük resim şeridi görürsünüz; her öğenin, listeden kaldırmak için bir **×** işareti vardır.

### Adım 2 — Kaldırılacak alanın üzerini boyayın
Sol sütundan bir araç seçin, ardından filigranın üzerini boyayın/çizin (boyanan alan **yumuşak kırmızı** renkte görünür):

| Araç | Ne için kullanılır |
|----|---|
| **Fırça** | Filigranın üzerini boyayın (sol fare düğmesini basılı tutup sürükleyin). Fırça boyutunu aşağıdaki kaydırıcıyla ayarlayın. |
| **Kutu** | Hızlı bir kapatma için filigranın üzerine bir dikdörtgen sürükleyin. |
| **Silgi** | Fazla boyamayı temizleyin. |
| **Metin** | Metin biçimindeki bir filigranı tam olarak kapatmak için metin yazın. Bu metin yalnızca bir **işaretleyicidir** — işlemden sonra kaybolur ve görüntüye kalıcı olarak eklenmez. |

Çok mu boyadınız? Sol sütundaki **Geri al / Yinele / Tümünü temizle / Sıfırla** seçeneklerini kullanın.
Aracı bırakmak için araç düğmesine tekrar tıklayın (ya da **Esc** tuşuna basın).

> **İpucu:** filigranı tamamen kapatın ve kenarlardan biraz taşırın — sonuçlar, eksik boyamaya göre daha iyi görünür.

### Adım 3 — Çalıştır'a tıklayın
- **Çalıştır** — o anda açık olan görüntüyü/videoyu işleyin.
- **Tümünü çalıştır** — listedeki **aynı kare boyutuna sahip** her dosyayı toplu olarak işleyin
  (yalnızca 2 veya daha fazla dosya olduğunda etkinleşir).

### Adım 4 — Kaydet
- **Kaydet**'e tıklayın. **Her kaydettiğinizde, uygulama çıktı dosyaları için bir klasör seçmenizi ister.**
- Orijinalleri korumak mı istiyorsunuz? **"_clean ekle"** seçeneğini etkinleştirin — yeni dosyaların adına bir `_clean` eki
  eklenir (örneğin `photo.png` → `photo_clean.png`), böylece orijinalin üzerine yazılmaz.

---

## Video işleme (Pro sürümü)

- Videolar **Kaydet düğmesiyle kaydedilmez**. **Çalıştır** (tek video) veya **Tümünü çalıştır**
  (birden fazla video) düğmesine tıklayın; uygulama başladığında bir kayıt klasörü ister.
- Video, yapay zeka ile kare kare işlenir, bu yüzden **görüntülerden çok daha yavaştır** — bırakın çalışsın.

---

## Görüntüleme ve yardımcı araçlar

- **Fare tekerleği**: yakınlaştır / uzaklaştır · **Orta fare düğmesini basılı tutup sürükleyin**: kaydır · **F** veya **çift tıklama**: pencereye sığdır.
- **Ev** simgesi: ana sayfayı açar. **Küre** simgesi: dili değiştirir (Vietnamca dahil 9 dil desteklenir).

## Klavye kısayolları

| İşlem | Tuş |
|---|---|
| Geri al / Yinele | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Fırça boyutunu değiştir | `Ctrl` + fare tekerleği |
| Pencereye sığdır | `F` veya çift tıklama |
| Aracı bırak | `Esc` |
| Hızlı silme (Fırça kullanırken) | **Sağ fare düğmesini** basılı tutun |

---

## Desteklenen biçimler

- **Görüntüler:** JPG, PNG, WEBP, BMP, TIFF ve diğer yaygın görüntü biçimleri.
- **Video:** MP4, MOV, MKV, AVI, WEBM, WMV, FLV… (Pro sürümü).

## Sorun giderme

| Belirti | Ne yapmalı |
|---|---|
| Windows açılışta uyarı veriyor | **More info → Run anyway** (Daha fazla bilgi → Yine de çalıştır) seçeneğine tıklayın (uygulama güvenlidir, yalnızca kod imzalı değildir). |
| Videolar açılamıyor | **Lite** sürümünü kullanıyorsunuz — yalnızca görüntüler. **Pro** sürümünü kullanın. |
| Kaldırmadan sonra soluk izler kalıyor | Alanı **daha tam olarak ve kenarlardan biraz taşacak şekilde** boyayın, ardından tekrar Çalıştır'a tıklayın. |
| Video çok yavaş | Normaldir — video ağır bir işlemdir; lütfen bekleyin veya ekran kartı olan bir makine kullanın. |

Keyfini çıkarın!
