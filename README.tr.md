<h1 align="center">AI Watermark Remover</h1>

<p align="center"><b>Bir görsel veya videodaki logo, imza, üst yazı ya da filigranın üzerini boyayın — yapay zekâ alanı doğal şekilde doldurur, doğrudan bilgisayarınızda, internet gerekmeden.</b></p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.vi.md">Tiếng Việt</a> ·
  <a href="README.bn.md">বাংলা</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <a href="README.pt_BR.md">Português (BR)</a> ·
  <a href="README.ru.md">Русский</a> ·
  <b>Türkçe</b> ·
  <a href="README.ur.md">اردو</a> ·
  <a href="README.zh_CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Windows için Lite indir" src="https://img.shields.io/badge/%C4%B0ndir-Windows%20Lite-0078D6?style=for-the-badge&logo=windows&logoColor=white"></a>&nbsp;
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="macOS (Apple Silicon) için Lite indir" src="https://img.shields.io/badge/%C4%B0ndir-macOS%20Apple%20Silicon%20Lite-000000?style=for-the-badge&logo=apple&logoColor=white"></a>&nbsp;
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3"><img alt="Windows için Pro indir (Google Drive)" src="https://img.shields.io/badge/%C4%B0ndir-Windows%20Pro-76B900?style=for-the-badge&logo=windows&logoColor=white"></a>
</p>

---

## Kurulum

### Adım 1 — Makinenize uygun sürümü seçin

İki sürüm vardır. **Lite** **görsellerdeki** filigranları kaldırır ve CPU üzerinde çalışır. **Pro** **görsel ve videoları** işler; NVIDIA kartlı bir Windows bilgisayar gerektirir. Pencere başlığında **"Lite"** ya da **"Pro"** yazar, böylece hangisini kullandığınızı her zaman bilirsiniz.

| Makineniz | İndir | Google Drive | Not |
|---|---|---|---|
| 🪟 **Windows 10/11 (64-bit)** — Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`Windows_AI_Watermark_Remover_Lite_…zip`) | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Yalnızca görsel · ekran kartı gerekmez |
| 🍎 **Apple çipli Mac (M1/M2/M3/M4)** — Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`MacOS_AI-Watermark-Remover-Lite-arm64_…dmg`) | [macOS](https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l) | Yalnızca görsel · Intel Mac sürümü yok |
| 🪟 **Windows 10/11 (64-bit) + NVIDIA GPU** — Pro | — | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Görsel **ve video** · Pro sürümü yalnızca Google Drive'da yayınlanır |

> Pro, CUDA destekli bir **NVIDIA** kartı gerektirir — AMD ve Intel ekran kartları desteklenmez. Yoksa Lite'ı kullanın (yalnızca görsel).

**Sistem gereksinimleri**

| | |
|---|---|
| **Lite (görsel)** | Windows 10/11 64-bit veya Apple Silicon macOS · GPU gerekmez · 4 GB+ RAM |
| **Pro (görsel + video)** | Yalnızca Windows 10/11 64-bit · CUDA destekli NVIDIA GPU, en az 4 GB VRAM (HD / uzun klipler için 6–8 GB önerilir) · 8 GB+ RAM |
| **CPU** | AVX2 destekli 64-bit |
| **Ön koşullar (Windows)** | Visual C++ Redistributable 2015–2022 x64; Pro ayrıca güncel bir NVIDIA sürücüsü ister |

### Adım 2 — Kurun

<details open>
<summary><b>🪟 Windows'ta</b></summary>

1. **Lite:** Releases'tan `.zip` dosyasını indirip **çıkarın**. **Pro:** Google Drive klasöründen indirin.
2. İndirdiğiniz kurulum dosyasını çalıştırın (ya da hazır çalışan bir klasörse içindeki **`AI Watermark Remover Lite.exe`** / **`AI Watermark Remover Pro.exe`** dosyasını açın).
3. **"Windows protected your PC"** (SmartScreen) çıkarsa: **More info** → **Run anyway**'e tıklayın. *(Uygulama ücretli bir sertifikayla imzalanmadığı için işaretlenir — virüs değildir.)*
4. Kurulum yönetici izni ister (Program Files'a kurar) ve masaüstü kısayolu ekleyebilir. Uygulamayı **Başlat Menüsü**'nden veya **Masaüstü**'nden açın.

Lite ve Pro ayrı kurulumlardır — ikisini aynı bilgisayarda tutabilir, her birini ayrı ayrı kaldırabilirsiniz.

</details>

<details open>
<summary><b>🍎 macOS'ta</b></summary>

1. İndirilen **`.dmg`** dosyasını açın ve **AI Watermark Remover Lite'ı Uygulamalar klasörüne sürükleyin**.
2. **Uygulamalar**'a gidin, **AI Watermark Remover Lite**'a **sağ tıklayın** (veya Control-tık) → **Aç** → iletişim kutusunda yeniden **Aç**'a tıklayın. *(Uygulama Apple tarafından imzalanmadığı için **ilk seferde** bu şekilde açılmalıdır; sonrasında normal açılır.)*
3. macOS uygulamanın **"hasarlı / açılamıyor"** olduğunu söylerse veya Aç düğmesi yoksa **Terminal**'i açıp yapıştırın:
   ```bash
   xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"
   ```
   Sonra uygulamayı yeniden açın.

</details>

İlk açılış biraz daha uzun sürebilir; sonrakiler daha hızlıdır.

### Adım 3 — Ücretsiz, hesap gerekmez

İki sürüm de **ücretsizdir** — hesap yok, lisans anahtarı yok, dosya sınırı yok. Yapay zekâ modelleri uygulamanın içinde gelir; çalışırken hiçbir şey indirmez ve **görsellerinizi ya da videolarınızı hiçbir yere göndermez**; her şey çevrimdışı çalışır.

---

## İlk çalıştırma

1. **Bir dosya açın.** Bir veya daha fazla dosya seçmek için **📄**, bütün bir klasörü açmak için **📁** düğmesine tıklayın ya da dosyaları pencereye **sürükleyip bırakın**. Dosyaların en-boy oranları farklıysa uygulama hangi oranı (veya hepsini) yükleyeceğinizi sorar.
2. **Filigranın üzerini boyayın.** Araçlar sütunundan **Fırça**, **Kutu** veya **Metin** seçin; boyanan alan **soluk kırmızı** görünür. Tamamen kaplayın ve kenarlardan biraz taşırın — eksik boyamaktan daha iyi sonuç verir.
3. **Çalıştır'a tıklayın.** Sonuç boyanan alanın yerine geçer. Birden fazla dosya açıkken **Tümünü çalıştır**, aynı boyuttaki tüm dosyalara aynı boyalı alanı uygular.
4. **Kaydet'e tıklayın** ve bir çıktı klasörü seçin (uygulama her seferinde sorar). Orijinalleri korumak istiyorsanız önce **_clean ekle**'yi açın.

---

## Özellikler

- **Boyayın, kutu çizin veya yazın** — Fırça ile serbestçe boyayın, hızlı kaplama için Kutu sürükleyin, fazlasını Sil ile temizleyin ya da metin tipi bir filigranı tam kaplamak için üzerine metin yazın. Metin yalnızca bir işarettir — işlemden sonra kaybolur, görsele asla işlenmez.
- **Seçimi düzeltin** — Geri al / Yinele, tüm boyalı alanı Temizle veya görseli geri getirmek için Orijinal.
- **Toplu işleme** — **Tümünü çalıştır**, mevcut boyalı alanı aynı en-boy oranındaki tüm açık dosyalara uygular; farklı orandaki dosyalar atlanır ve sonunda sayılır.
- **Videodan filigran kaldırma (Pro)** — yapay zekâ videoyu kare kare işler, yalnızca filigranın çevresinde çalışır, sonucu orijinal kareye geri koyar ve orijinal sesi korur. Yerleşik oynatıcıyla klibi 100 / 75 / 50 / 25% önizleme kalitesinde gezebilirsiniz.
- **Üzerine yazmadan kaydetme** — Bir dosyayı kaydedip sonrakine geçin veya işlenmiş tüm dosyaları **Tümünü kaydet** ile tek klasöre yazın; **_clean ekle** yeni dosyalara son ek ekler (`foto.png` → `foto_clean.png`).
- **Çevrimdışı ve gizli** — her şey bilgisayarınızda çalışır; hiçbir şey yüklenmez.
- **9 arayüz dili** — English, Tiếng Việt, বাংলা, हिन्दी, Português (BR), Русский, Türkçe, اردو, 简体中文 — dünya simgesiyle değiştirin.

---

## Araçlar ve kontroller

### 📂 Aç

**📄** bir veya daha fazla dosya açar, **📁** bütün bir klasörü açar; dosyaları doğrudan pencereye de sürükleyebilirsiniz. Birden fazla dosyada altta bir küçük resim şeridi çıkar — geçiş için küçük resme, listeden çıkarmak için **×**'e tıklayın. Lite yalnızca görsel kabul eder; video dosyaları elenir.

### 🖌 Araçlar

| Araç | Ne için |
|---|---|
| **Fırça** | Filigranın üzerini boyamak (sol tuşu basılı tutup sürükleyin). Boyutu kaydırıcıyla, `Ctrl` + fare tekerleğiyle veya `[` / `]` ile ayarlayın. Boyarken silmek için **sağ tuşu** basılı tutun. |
| **Kutu** | Hızlı kaplama için filigranın üzerine dikdörtgen sürüklemek. |
| **Sil** | Fazla boyayı temizlemek. |
| **Metin** | Metin tipi filigranı tam kaplamak için üzerine yazı yazmak (yalnızca görsel). `Delete` seçili metni siler. |

Aracı bırakmak için düğmesine yeniden tıklayın veya **Esc**'ye basın. **Geri al / Yinele / Temizle / Orijinal** aynı sütundadır.

### ▶ Çalıştır

**Çalıştır** baktığınız dosyayı işler; **Tümünü çalıştır** (2+ dosya açıkken görünür) aynı en-boy oranındaki tüm dosyaları işler. İş sürerken düğmeler **Durdur** / **Tümünü durdur** olur. Sonuçlar siz kaydedene kadar uygulamada kalır.

### 🎬 Video (Pro)

Bir video açın, herhangi bir karede durdurun ve filigranın üzerini Fırça veya Kutu ile boyayın (boyamaya başlamak oynatmayı duraklatır). Klibi kontrol etmek için oynat düğmesini ve arama çubuğunu, önizlemeyi hafif tutmak için kalite menüsünü (100 / 75 / 50 / 25%) kullanın. Video kare kare işlendiği için **görsellerden çok daha yavaştır** — bırakın çalışsın. Bitince görsel gibi **Kaydet** veya **Tümünü kaydet** ile kaydedin; çıktı `.mp4` olur.

### 💾 Kaydet

**Kaydet** mevcut sonucu yazar ve sonraki dosyaya geçer; **Tümünü kaydet** işlenmiş tüm dosyaları tek klasöre yazar. Uygulama çıktı klasörünü her seferinde sorar. Orijinal adı kullanmak yerine `_clean` eklemek için **_clean ekle**'yi işaretleyin.

### 🔍 Görünüm

Yakınlaştırmak için fare tekerleği, kaydırmak için orta tuşu basılı tutup sürükleyin, pencereye sığdırmak için **F** veya çift tık. **Ev** simgesi ana sayfayı açar; **dünya** simgesi dili değiştirir.

### ⌨️ Klavye kısayolları

| İşlem | Tuş |
|---|---|
| Geri al / Yinele | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Fırça boyutu | `Ctrl` + fare tekerleği veya `[` / `]` |
| Pencereye sığdır | `F`, `0` veya çift tık |
| Aracı bırak | `Esc` |
| Hızlı silme (Fırça kullanırken) | **Sağ fare tuşunu** basılı tutun |
| Kaydırma | **Orta fare tuşunu** basılı tutup sürükleyin |

### 🗂 Desteklenen biçimler

- **Görseller:** PNG, JPG/JPEG, WEBP, BMP, TIFF, PPM/PGM/PBM/PNM.
- **Video (Pro):** MP4, M4V, MOV, WEBM, MKV, AVI, FLV, WMV, MPG/MPEG, TS/M2TS/MTS, 3GP, OGV. Çıktı `.mp4` olarak kaydedilir.

---

## Verileriniz nerede

| Ne | Windows | macOS |
|---|---|---|
| Çıktı görselleri / videoları | Kaydederken seçtiğiniz klasör | Kaydederken seçtiğiniz klasör |
| Ayarlar (dil, _clean ekle) | Kayıt Defteri: `HKEY_CURRENT_USER\Software\Duckmartians\AI Watermark Remover` | `~/Library/Preferences/com.duckmartians.AI Watermark Remover.plist` |
| Kaydedilmemiş sonuçlar (geçici) | `%TEMP%\AIWatermarkRemover_work` | Sistem geçici klasöründe `AIWatermarkRemover_work` |
| Çökme günlüğü | `%APPDATA%\AI Watermark Remover\crash.log` | `~/AI Watermark Remover/crash.log` |

Geçici klasör uygulama her açıldığında temizlenir — **uygulamayı kapatmadan önce sonuçlarınızı kaydedin**.

---

## Sorun giderme

**Windows "Windows protected your PC" ile engelliyor** — **More info → Run anyway**'e tıklayın. Uygulama ücretli bir sertifikayla imzalanmadığı için işaretlenir — virüs değildir.

**macOS uygulamanın hasarlı / açılamadığını söylüyor** — Apple tarafından imzalanmamıştır. İlk seferde sağ tık → **Aç**, ya da `xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"` komutunu çalıştırın.

**Videolar açılmıyor** — yalnızca görselleri işleyen **Lite** sürümündesiniz. Videodan filigran kaldırmak için **Pro**'yu kurun (Windows + NVIDIA kart).

**Kaydederken videoların "Çalıştır" ile dışa aktarıldığı söyleniyor** — o video henüz işlenmedi. Önce **Çalıştır** (veya **Tümünü çalıştır**), sonra **Kaydet**'e tıklayın.

**Tümünü çalıştır bazı dosyaları atladı** — yalnızca boyadığınız dosyayla aynı en-boy oranındaki dosyalar işlenir. Diğerlerini ayrıca açın veya açarken onların oranını seçin.

**Kaldırmadan sonra soluk izler kalıyor** — daha eksiksiz ve filigranın kenarlarından biraz taşarak boyayın, sonra yeniden Çalıştır'a basın. Karmaşık arka planlardaki büyük alanlarda yine iz kalabilir.

**Video çok yavaş** — normaldir: yapay zekâ her kareyi işler, bu yüzden video görsellerden çok daha uzun sürer. Bırakın çalışsın; kısa klipler ve daha fazla VRAM'li kart daha hızlı biter.

**Uygulama kendi kendine kapanıyor** — sorunu bildirirken `crash.log` dosyasını (yukarıdaki tabloya bakın) gönderin.

---

Filigran ve logoları yalnızca size ait olan veya düzenleme hakkına sahip olduğunuz görsel ve videolardan kaldırın.
