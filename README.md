# AI Watermark Remover — User Guide

<p align="left">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover//releases/latest">
    <img src="https://img.shields.io/badge/Windows-%F0%9F%92%BB-0078D6?style=for-the-badge&logo=windows&logoColor=white">
  </a>
  <a href="https://github.com/duckmartians/AI-Watermark-Remover//releases/latest">
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

🌐 **English** · [Tiếng Việt](README.vi.md) · [বাংলা](README.bn.md) · [हिन्दी](README.hi.md) · [Português (BR)](README.pt_BR.md) · [Русский](README.ru.md) · [Türkçe](README.tr.md) · [اردو](README.ur.md) · [简体中文](README.zh_CN.md)

This app helps you **remove logos, watermarks, signatures and text overlays from images and videos**.
Just **paint over what you want gone** and the app fills it back in naturally. Everything runs
**on your own computer** — **no internet needed**, and your images/videos are **never uploaded anywhere**.

---
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/dbcb0fad-cc38-49d6-b9c6-acd1c0e16983" />
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/f07d1f33-e835-4c6c-b5b6-6b8db94b9cb9" />

## Install & Open

1. Run the installer (or unzip the folder if you received a compressed archive).
2. Open **AI Watermark Remover** (from the Desktop, the Start menu, or the `.exe` file).

> **Windows shows "Windows protected your PC"?**
> This is the default warning for apps without a paid signing certificate — **it is not a virus**.
> Click **More info → Run anyway** to open it.

The first launch may take a little longer; subsequent launches are faster.

**There are two editions:** the **Pro** edition (images + video) and the **Lite** edition (images only, lighter).
Check the window title to tell them apart: **"Pro"** = full edition, **"Lite"** = light edition (cannot open videos).

---

## System requirements

| | **Lite** (images) | **Pro** (images + video) |
|---|---|---|
| OS | Windows 10/11 64-bit (or macOS) | Windows 10/11 64-bit (or macOS) |
| CPU | 64-bit with **AVX2** | 64-bit with **AVX2** |
| GPU | **not required** — runs on CPU | **NVIDIA GPU with CUDA required** for video |
| VRAM | — | 4 GB min · **6–8 GB recommended** (HD / long clips) |
| RAM | 4 GB+ | 8 GB+ |
| Also install | **Visual C++ Redistributable 2015–2022 x64** | same + an up-to-date **NVIDIA driver** |

- **Pro video needs an NVIDIA graphics card with CUDA** — roughly **RTX 2060 (RTX 20-series / GTX 16-series, "Turing") or newer**. Without a supported NVIDIA GPU the video engine falls back to the CPU and becomes **extremely slow** (often impractical).
- **Image** removal works fine **on CPU** in **both** editions — no graphics card needed.
- AMD/Intel GPUs, or NVIDIA cards older than the 16/20-series, are **not accelerated** for video.
- No internet is required and nothing is uploaded — everything runs locally.

---

## How to use — 4 steps

### Step 1 — Open an image/video
- Click the **document** button to pick one or more files, or the **folder** button to open a whole folder.
- Or **drag and drop** images/videos straight into the window.
- With multiple files you get a thumbnail strip at the bottom; each item has an **×** to remove it from the list.

### Step 2 — Paint over what to remove
Pick a tool in the left column, then paint/outline over the watermark (the painted area shows as a **soft red**):

| Tool | Use it to |
|----|---|
| **Brush** | Paint over the watermark (hold the left mouse button and drag). Adjust brush size with the slider below. |
| **Box** | Drag a rectangle over the watermark for a quick cover. |
| **Eraser** | Wipe away extra painting. |
| **Text** | Type text to precisely cover a text-style watermark. This text is only a **marker** — it disappears after processing and is not baked into the image. |

Painted too much? Use **Undo / Redo / Clear all / Reset** in the left column.
Click the tool button again (or press **Esc**) to deselect it.

> **Tip:** cover the watermark fully and spill over a little — results look better than under-painting.

### Step 3 — Click Run
- **Run** — process the currently open image/video.
- **Run all** — batch-process every file **with the same frame size** in the list
  (enabled only when there are 2 or more files).

### Step 4 — Save
- Click **Save**. **Each time you save, the app asks you to choose a folder** for the output files.
- Want to keep the originals? Enable the **"Add _clean"** option — new files get a `_clean` suffix
  in their name (e.g. `photo.png` → `photo_clean.png`), so the original is not overwritten.

---

## Video processing (Pro edition)

- Videos are **not saved with the Save button**. Click **Run** (one video) or **Run all**
  (multiple videos); the app asks for a save folder when it starts.
- Video is processed frame by frame by AI on the **GPU**, so it is slower than images — just let it run.

### Speed ⇄ quality sliders

Under the **Brush size** slider (left column, **Pro** only) there are four sliders that let you trade
**speed for quality**. Hover any slider to see a tip. Your settings are remembered.

| Slider | What it controls | Faster | Sharper |
|---|---|---|---|
| **Resolution** | Processing resolution — the **biggest** speed lever. Lower = much faster, erased area a little soft. | ~**50** | **100** |
| **Motion** | How thoroughly motion between frames is analysed (quality barely changes). | **2–4** | 20 |
| **Frames** | How many nearby frames are handled together. | lower | higher |
| **Reference** | Spacing when picking reference frames. | **higher** | lower |

- **Want it fast?** Set **Resolution ≈ 50** and **Motion ≈ 4** (defaults already favour speed).
- **Erased area looks blurry?** Raise **Resolution** toward **100**.
- These only affect **video**; images are unaffected.

---

## Viewing & utilities

- **Mouse wheel**: zoom in / out · **Hold middle mouse and drag**: pan · **F** or **double-click**: fit to window.
- **House** icon: open the homepage. **Globe** icon: change language (9 languages supported, including Vietnamese).

## Keyboard shortcuts

| Action | Key |
|---|---|
| Undo / Redo | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Change brush size | `Ctrl` + mouse wheel |
| Fit to window | `F` or double-click |
| Deselect tool | `Esc` |
| Quick erase (while using Brush) | Hold **right mouse button** |

---

## Supported formats

- **Images:** JPG, PNG, WEBP, BMP, TIFF and other common image formats.
- **Video:** MP4, MOV, MKV, AVI, WEBM, WMV, FLV… (Pro edition).

## Troubleshooting

| Symptom | What to do |
|---|---|
| Windows warns on open | Click **More info → Run anyway** (the app is safe, it just isn't code-signed). |
| Can't open videos | You're on the **Lite** edition — images only. Use the **Pro** edition. |
| Faint marks remain after removal | Paint **more fully and slightly over the edges**, then Run again. |
| Video is very slow | Lower the **Resolution** slider (≈50) and **Motion** (≈4) — see *Speed ⇄ quality sliders*. A CUDA NVIDIA GPU (RTX 2060+) is strongly recommended — see *System requirements*. |

Enjoy!
