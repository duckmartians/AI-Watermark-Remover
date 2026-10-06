<h1 align="center">AI Watermark Remover</h1>

<p align="center"><b>Paint over a logo, signature, text overlay or watermark on an image or video — AI fills it back in naturally, right on your computer, no internet needed.</b></p>

<p align="center">
  <b>English</b> ·
  <a href="README.vi.md">Tiếng Việt</a> ·
  <a href="README.bn.md">বাংলা</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <a href="README.pt_BR.md">Português (BR)</a> ·
  <a href="README.ru.md">Русский</a> ·
  <a href="README.tr.md">Türkçe</a> ·
  <a href="README.ur.md">اردو</a> ·
  <a href="README.zh_CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Download Lite for Windows" src="https://img.shields.io/badge/Download-Windows%20Lite-0078D6?style=for-the-badge&logo=windows&logoColor=white"></a>&nbsp;
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Download Lite for macOS (Apple Silicon)" src="https://img.shields.io/badge/Download-macOS%20Apple%20Silicon%20Lite-000000?style=for-the-badge&logo=apple&logoColor=white"></a>&nbsp;
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3"><img alt="Download Pro for Windows (Google Drive)" src="https://img.shields.io/badge/Download-Windows%20Pro-76B900?style=for-the-badge&logo=windows&logoColor=white"></a>
</p>

---

## Install

### Step 1 — Pick the right edition for your machine

There are two editions. **Lite** removes watermarks from **images** and runs on the CPU. **Pro** handles **images and video** and needs a Windows PC with an NVIDIA card. The window title shows **"Lite"** or **"Pro"** so you always know which one you have.

| Your machine | Download | Google Drive | Notes |
|---|---|---|---|
| 🪟 **Windows 10/11 (64-bit)** — Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`Windows_AI_Watermark_Remover_Lite_…zip`) | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Images only · no graphics card needed |
| 🍎 **Mac with Apple chip (M1/M2/M3/M4)** — Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`MacOS_AI-Watermark-Remover-Lite-arm64_…dmg`) | [macOS](https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l) | Images only · there is no Intel Mac build |
| 🪟 **Windows 10/11 (64-bit) + NVIDIA GPU** — Pro | — | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Images **and video** · the Pro edition is published on Google Drive only |

> Pro needs an **NVIDIA** card with CUDA — AMD and Intel graphics are not supported. If you don't have one, use Lite (images only).

**System requirements**

| | |
|---|---|
| **Lite (images)** | Windows 10/11 64-bit or macOS on Apple Silicon · no GPU needed · 4 GB+ RAM |
| **Pro (images + video)** | Windows 10/11 64-bit only · NVIDIA GPU with CUDA, 4 GB VRAM minimum (6–8 GB recommended for HD / long clips) · 8 GB+ RAM |
| **CPU** | 64-bit with AVX2 support |
| **Prerequisites (Windows)** | Visual C++ Redistributable 2015–2022 x64; Pro also needs an up-to-date NVIDIA driver |

### Step 2 — Install

<details open>
<summary><b>🪟 On Windows</b></summary>

1. **Lite:** download the `.zip` from Releases and **extract it**. **Pro:** download it from the Google Drive folder.
2. Run the installer you got (or, if it is a ready-to-run folder, open **`AI Watermark Remover Lite.exe`** / **`AI Watermark Remover Pro.exe`** inside it).
3. If **"Windows protected your PC"** (SmartScreen) appears: click **More info** → **Run anyway**. *(The app isn't signed with a paid certificate, so it's flagged — it isn't a virus.)*
4. The installer asks for admin rights (it installs into Program Files) and can add a Desktop shortcut. Launch the app from the **Start Menu** or the **Desktop**.

Lite and Pro are separate installs — you can keep both on the same PC and uninstall each one on its own.

</details>

<details open>
<summary><b>🍎 On macOS</b></summary>

1. Open the downloaded **`.dmg`**, then **drag AI Watermark Remover Lite into the Applications folder**.
2. Go to **Applications**, **right-click** (or Control-click) **AI Watermark Remover Lite** → **Open** → click **Open** again in the dialog. *(The app isn't signed by Apple, so you must open it this way the **first time**; afterwards it opens normally.)*
3. If macOS says the app is **"damaged / can't be opened"**, or there's no Open button, open **Terminal** and paste:
   ```bash
   xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"
   ```
   Then open the app again.

</details>

The first launch may take a little longer; later launches are faster.

### Step 3 — Free, no account

Both editions are **free** — no account, no license key, no file limits. The AI models ship inside the app, so it downloads nothing while it runs and **never uploads your images or videos** anywhere; everything works offline.

---

## First run

1. **Open a file.** Click the **📄** button to pick one or more files, the **📁** button to open a whole folder, or **drag and drop** files into the window. If the files have different aspect ratios, the app asks which ratio to load (or all of them).
2. **Paint over the watermark.** Pick **Brush**, **Box** or **Text** in the Tools column; the painted area shows in **soft red**. Cover it fully and spill over the edges a little — that looks better than under-painting.
3. **Click Run.** The result replaces the painted area. With several files open, **Run all** applies the same painted area to every file of the same size.
4. **Click Save** and choose an output folder (the app asks every time). Turn on **Add _clean** first if you want to keep the originals.

---

## Features

- **Paint, box or type** — paint freely with the Brush, drag a Box for a quick cover, wipe extra paint with the Eraser, or type text over a text-style watermark to cover it precisely. The text is only a marker — it disappears after processing and is never baked into the image.
- **Fix your selection** — Undo / Redo, Clear the whole painted area, or Reset to restore the original.
- **Batch processing** — **Run all** applies the current painted area to every open file with the same aspect ratio; files with a different ratio are skipped and counted when it finishes.
- **Video watermark removal (Pro)** — AI processes the video frame by frame, works only on the area around the watermark, puts the result back into the original frame and keeps the original audio. A built-in player lets you scrub through the clip with 100 / 75 / 50 / 25% preview quality.
- **Save without overwriting** — Save one file and jump to the next, or **Save all** processed files into one folder; **Add _clean** gives new files a suffix (`photo.png` → `photo_clean.png`).
- **Offline and private** — everything runs on your computer; nothing is uploaded.
- **9 interface languages** — English, Tiếng Việt, বাংলা, हिन्दी, Português (BR), Русский, Türkçe, اردو, 简体中文 — switch with the globe icon.

---

## Tools & controls

### 📂 Open

**📄** opens one or more files, **📁** opens a whole folder, or drag files straight into the window. With several files a thumbnail strip appears at the bottom — click a thumbnail to switch, or its **×** to remove it from the list. Lite only accepts images; video files are filtered out.

### 🖌 Tools

| Tool | Use it to |
|---|---|
| **Brush** | Paint over the watermark (hold the left mouse button and drag). Set the size with the slider, `Ctrl` + mouse wheel, or `[` / `]`. Hold the **right mouse button** to erase while painting. |
| **Box** | Drag a rectangle over the watermark for a quick cover. |
| **Erase** | Wipe away extra paint. |
| **Text** | Type text over a text watermark to cover it precisely (images only). `Delete` removes the selected text. |

Click the tool button again, or press **Esc**, to deselect it. **Undo / Redo / Clear / Reset** sit in the same column.

### ▶ Run

**Run** processes the file you're looking at; **Run all** (shown when 2+ files are open) processes every file with the same aspect ratio. While a job runs the buttons turn into **Stop** / **Stop all**. Results stay in the app until you save them.

### 🎬 Video (Pro)

Open a video, pause on any frame and paint over the watermark with the Brush or Box (painting pauses playback). Use the play button and seek bar to check the clip, and the quality menu (100 / 75 / 50 / 25%) to keep the preview light. Video is processed frame by frame, so it's **much slower than images** — just let it run. When it's done, save it with **Save** or **Save all** like an image; the output is an `.mp4`.

### 💾 Save

**Save** writes the current result and moves to the next file; **Save all** writes every processed file into one folder. The app asks for the output folder each time. Tick **Add _clean** to append `_clean` to file names instead of reusing the original name.

### 🔍 View

Mouse wheel to zoom, hold the middle button and drag to pan, **F** or double-click to fit the window. The **house** icon opens the homepage; the **globe** icon changes the language.

### ⌨️ Keyboard shortcuts

| Action | Key |
|---|---|
| Undo / Redo | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Brush size | `Ctrl` + mouse wheel, or `[` / `]` |
| Fit to window | `F`, `0` or double-click |
| Deselect tool | `Esc` |
| Quick erase (while using Brush) | Hold the **right mouse button** |
| Pan | Hold the **middle mouse button** and drag |

### 🗂 Supported formats

- **Images:** PNG, JPG/JPEG, WEBP, BMP, TIFF, PPM/PGM/PBM/PNM.
- **Video (Pro):** MP4, M4V, MOV, WEBM, MKV, AVI, FLV, WMV, MPG/MPEG, TS/M2TS/MTS, 3GP, OGV. Output is saved as `.mp4`.

---

## Where your data lives

| What | Windows | macOS |
|---|---|---|
| Output images / videos | The folder you pick when saving | The folder you pick when saving |
| Settings (language, Add _clean) | Registry: `HKEY_CURRENT_USER\Software\Duckmartians\AI Watermark Remover` | `~/Library/Preferences/com.duckmartians.AI Watermark Remover.plist` |
| Unsaved results (temporary) | `%TEMP%\AIWatermarkRemover_work` | `AIWatermarkRemover_work` in the system temp folder |
| Crash log | `%APPDATA%\AI Watermark Remover\crash.log` | `~/AI Watermark Remover/crash.log` |

The temporary folder is cleared every time the app starts — **save your results before closing the app**.

---

## Troubleshooting

**Windows blocks it at "Windows protected your PC"** — click **More info → Run anyway**. The app isn't signed with a paid certificate, so it's flagged — it isn't a virus.

**macOS says the app is damaged / can't be opened** — it isn't signed by Apple. Right-click → **Open** the first time, or run `xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"`.

**Can't open videos** — you're on the **Lite** edition, which handles images only. Install **Pro** (Windows + NVIDIA card) to remove watermarks from video.

**Save says videos are exported with Run** — that video hasn't been processed yet. Click **Run** (or **Run all**) first, then **Save**.

**Run all skipped some files** — Run all only processes files with the same aspect ratio as the one you painted on. Open the others separately, or pick their ratio when opening.

**Faint marks remain after removal** — paint more fully and slightly past the edges of the watermark, then Run again. Large areas over busy backgrounds can still leave traces.

**Video is very slow** — normal: AI processes every frame, so video takes much longer than images. Just let it run; shorter clips and a card with more VRAM finish faster.

**The app closes on its own** — send the `crash.log` file (see the table above) when you report the problem.

---

Only remove watermarks and logos from images and videos you own or have the right to edit.
