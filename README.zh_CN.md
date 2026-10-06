<h1 align="center">AI Watermark Remover</h1>

<p align="center"><b>在图片或视频上涂抹 Logo、签名、叠加文字或水印 —— AI 会自然地填补该区域，直接在你的电脑上运行，无需联网。</b></p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.vi.md">Tiếng Việt</a> ·
  <a href="README.bn.md">বাংলা</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <a href="README.pt_BR.md">Português (BR)</a> ·
  <a href="README.ru.md">Русский</a> ·
  <a href="README.tr.md">Türkçe</a> ·
  <a href="README.ur.md">اردو</a> ·
  <b>简体中文</b>
</p>

<p align="center">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="下载 Windows Lite 版" src="https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD-Windows%20Lite-0078D6?style=for-the-badge&logo=windows&logoColor=white"></a>&nbsp;
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="下载 macOS（Apple 芯片）Lite 版" src="https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD-macOS%20Apple%20Silicon%20Lite-000000?style=for-the-badge&logo=apple&logoColor=white"></a>&nbsp;
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3"><img alt="下载 Windows Pro 版（Google Drive）" src="https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD-Windows%20Pro-76B900?style=for-the-badge&logo=windows&logoColor=white"></a>
</p>

---

## 安装

### 第 1 步 —— 选择适合你电脑的版本

共有两个版本。**Lite** 去除**图片**水印，使用 CPU 运行。**Pro** 可处理**图片和视频**，需要配备 NVIDIA 显卡的 Windows 电脑。窗口标题会显示 **"Lite"** 或 **"Pro"**，让你随时知道在用哪个版本。

| 你的电脑 | 下载 | Google Drive | 说明 |
|---|---|---|---|
| 🪟 **Windows 10/11（64 位）** —— Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest)（`Windows_AI_Watermark_Remover_Lite_…zip`） | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | 仅图片 · 无需显卡 |
| 🍎 **Apple 芯片 Mac（M1/M2/M3/M4）** —— Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest)（`MacOS_AI-Watermark-Remover-Lite-arm64_…dmg`） | [macOS](https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l) | 仅图片 · 没有 Intel Mac 版本 |
| 🪟 **Windows 10/11（64 位）+ NVIDIA 显卡** —— Pro | — | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | 图片**和视频** · Pro 版仅在 Google Drive 发布 |

> Pro 版需要支持 CUDA 的 **NVIDIA** 显卡 —— 不支持 AMD 和 Intel 显卡。没有的话请使用 Lite 版（仅图片）。

**系统要求**

| | |
|---|---|
| **Lite（图片）** | Windows 10/11 64 位或 Apple 芯片的 macOS · 无需 GPU · 4 GB 以上内存 |
| **Pro（图片 + 视频）** | 仅 Windows 10/11 64 位 · 支持 CUDA 的 NVIDIA GPU，显存至少 4 GB（高清 / 长视频建议 6–8 GB）· 8 GB 以上内存 |
| **CPU** | 支持 AVX2 的 64 位处理器 |
| **前置组件（Windows）** | Visual C++ Redistributable 2015–2022 x64；Pro 版还需要较新的 NVIDIA 驱动 |

### 第 2 步 —— 安装

<details open>
<summary><b>🪟 Windows</b></summary>

1. **Lite：** 从 Releases 下载 `.zip` 并**解压**。**Pro：** 从 Google Drive 文件夹下载。
2. 运行下载到的安装程序（如果是可直接运行的文件夹，则打开其中的 **`AI Watermark Remover Lite.exe`** / **`AI Watermark Remover Pro.exe`**）。
3. 如果出现 **"Windows protected your PC"**（SmartScreen）：点击 **More info** → **Run anyway**。*（应用没有付费证书签名，所以会被标记 —— 这不是病毒。）*
4. 安装程序会请求管理员权限（安装到 Program Files），并可创建桌面快捷方式。从**开始菜单**或**桌面**启动应用。

Lite 和 Pro 是两个独立安装 —— 可以同时装在一台电脑上，并分别卸载。

</details>

<details open>
<summary><b>🍎 macOS</b></summary>

1. 打开下载的 **`.dmg`**，然后**把 AI Watermark Remover Lite 拖到"应用程序"文件夹**。
2. 进入**应用程序**，**右键**（或按住 Control 点击）**AI Watermark Remover Lite** → **打开** → 在对话框中再次点击**打开**。*（应用没有经过 Apple 签名，所以**第一次**必须这样打开；之后可正常打开。）*
3. 如果 macOS 提示应用**"已损坏 / 无法打开"**，或没有"打开"按钮，请打开**终端**并粘贴：
   ```bash
   xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"
   ```
   然后重新打开应用。

</details>

第一次启动可能稍慢，之后会更快。

### 第 3 步 —— 免费，无需账号

两个版本都**免费** —— 无需账号、无需许可证密钥、不限文件数量。AI 模型已内置在应用中，运行时不会下载任何内容，也**绝不会上传你的图片或视频**；一切离线运行。

---

## 首次运行

1. **打开文件。** 点击 **📄** 选择一个或多个文件，点击 **📁** 打开整个文件夹，或把文件**拖放**到窗口中。如果文件的宽高比不同，应用会询问要载入哪种比例（或全部）。
2. **涂抹水印。** 在工具栏选择**画笔**、**框选**或**文字**；涂抹区域显示为**淡红色**。完全覆盖并稍微超出边缘 —— 效果比涂得不够好。
3. **点击运行。** 结果会替换涂抹区域。打开多个文件时，**全部运行**会把同一涂抹区域应用到所有相同尺寸的文件。
4. **点击保存**并选择输出文件夹（每次都会询问）。想保留原文件，请先勾选**添加 _clean**。

---

## 功能

- **涂抹、框选或输入文字** —— 用画笔自由涂抹，拖出框选快速覆盖，用擦除去掉多余部分，或在文字水印上输入文字以精确覆盖。文字只是标记 —— 处理后会消失，不会写入图片。
- **修正选区** —— 撤销 / 重做，清除全部涂抹区域，或还原到原图。
- **批量处理** —— **全部运行**把当前涂抹区域应用到所有相同宽高比的已打开文件；比例不同的文件会被跳过，并在结束时统计。
- **视频去水印（Pro）** —— AI 逐帧处理视频，只处理水印周围的区域，把结果放回原始画面，并保留原始音频。内置播放器可拖动预览，预览质量可选 100 / 75 / 50 / 25%。
- **保存不覆盖原文件** —— 保存一个文件并跳到下一个，或用**全部保存**把已处理的文件存到一个文件夹；**添加 _clean** 会给新文件加后缀（`photo.png` → `photo_clean.png`）。
- **离线且私密** —— 一切都在你的电脑上运行，不上传任何内容。
- **9 种界面语言** —— English、Tiếng Việt、বাংলা、हिन्दी、Português (BR)、Русский、Türkçe、اردو、简体中文 —— 点击地球图标切换。

---

## 工具与操作

### 📂 打开

**📄** 打开一个或多个文件，**📁** 打开整个文件夹，也可以直接把文件拖进窗口。打开多个文件时底部会出现缩略图条 —— 点击缩略图切换，点击 **×** 将其移出列表。Lite 版只接受图片，视频文件会被过滤。

### 🖌 工具

| 工具 | 用途 |
|---|---|
| **画笔** | 涂抹水印（按住左键拖动）。用滑块、`Ctrl` + 鼠标滚轮或 `[` / `]` 调整大小。涂抹时按住**右键**可直接擦除。 |
| **框选** | 在水印上拖出矩形，快速覆盖。 |
| **擦除** | 擦掉多余的涂抹。 |
| **文字** | 在文字水印上输入文字以精确覆盖（仅图片）。`Delete` 删除选中的文字。 |

再次点击工具按钮或按 **Esc** 取消选择。**撤销 / 重做 / 清除 / 还原**在同一栏。

### ▶ 运行

**运行**处理当前查看的文件；**全部运行**（打开 2 个以上文件时显示）处理所有相同宽高比的文件。运行中按钮会变为**停止** / **全部停止**。结果会保留在应用中，直到你保存。

### 🎬 视频（Pro）

打开视频，暂停在任意一帧，用画笔或框选涂抹水印（开始涂抹会自动暂停播放）。用播放按钮和进度条检查视频，用质量菜单（100 / 75 / 50 / 25%）让预览更流畅。视频逐帧处理，所以**比图片慢得多** —— 耐心等待即可。完成后像图片一样用**保存**或**全部保存**导出；输出为 `.mp4`。

### 💾 保存

**保存**写出当前结果并跳到下一个文件；**全部保存**把所有已处理的文件写入一个文件夹。每次都会询问输出文件夹。勾选**添加 _clean** 会在文件名后加 `_clean`，而不是沿用原文件名。

### 🔍 查看

鼠标滚轮缩放，按住中键拖动平移，按 **F** 或双击适应窗口。**房子**图标打开主页；**地球**图标切换语言。

### ⌨️ 快捷键

| 操作 | 按键 |
|---|---|
| 撤销 / 重做 | `Ctrl+Z` / `Ctrl+Shift+Z` |
| 画笔大小 | `Ctrl` + 鼠标滚轮，或 `[` / `]` |
| 适应窗口 | `F`、`0` 或双击 |
| 取消选择工具 | `Esc` |
| 快速擦除（使用画笔时） | 按住**鼠标右键** |
| 平移 | 按住**鼠标中键**拖动 |

### 🗂 支持的格式

- **图片：** PNG、JPG/JPEG、WEBP、BMP、TIFF、PPM/PGM/PBM/PNM。
- **视频（Pro）：** MP4、M4V、MOV、WEBM、MKV、AVI、FLV、WMV、MPG/MPEG、TS/M2TS/MTS、3GP、OGV。输出保存为 `.mp4`。

---

## 数据存放位置

| 内容 | Windows | macOS |
|---|---|---|
| 输出的图片 / 视频 | 保存时选择的文件夹 | 保存时选择的文件夹 |
| 设置（语言、添加 _clean） | 注册表：`HKEY_CURRENT_USER\Software\Duckmartians\AI Watermark Remover` | `~/Library/Preferences/com.duckmartians.AI Watermark Remover.plist` |
| 未保存的结果（临时） | `%TEMP%\AIWatermarkRemover_work` | 系统临时文件夹中的 `AIWatermarkRemover_work` |
| 崩溃日志 | `%APPDATA%\AI Watermark Remover\crash.log` | `~/AI Watermark Remover/crash.log` |

每次启动应用都会清空临时文件夹 —— **关闭应用前请先保存结果**。

---

## 故障排除

**Windows 提示 "Windows protected your PC" 并阻止运行** —— 点击 **More info → Run anyway**。应用没有付费证书签名，所以会被标记 —— 这不是病毒。

**macOS 提示应用已损坏 / 无法打开** —— 应用未经 Apple 签名。第一次请右键 → **打开**，或运行 `xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"`。

**无法打开视频** —— 你使用的是只处理图片的 **Lite** 版。要去除视频水印，请安装 **Pro** 版（Windows + NVIDIA 显卡）。

**保存时提示视频需通过"运行"导出** —— 该视频还没有处理。请先点击**运行**（或**全部运行**），再点击**保存**。

**全部运行跳过了一些文件** —— 只会处理与你涂抹的文件宽高比相同的文件。请单独打开其他文件，或在打开时选择它们的比例。

**去除后仍有淡淡痕迹** —— 涂得更完整，并稍微超出水印边缘，然后再次运行。复杂背景上的大面积区域仍可能留下痕迹。

**视频处理很慢** —— 这是正常的：AI 会处理每一帧，所以视频比图片慢得多。耐心等待；较短的视频和显存更大的显卡会更快完成。

**应用自行关闭** —— 反馈问题时请附上 `crash.log` 文件（见上表）。

---

请只对你拥有或有权编辑的图片和视频去除水印和 Logo。
