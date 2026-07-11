# AI Watermark Remover — 用户指南

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

🌐 [English](README.md) · [Tiếng Việt](README.vi.md) · [বাংলা](README.bn.md) · [हिन्दी](README.hi.md) · [Português (BR)](README.pt_BR.md) · [Русский](README.ru.md) · [Türkçe](README.tr.md) · [اردو](README.ur.md) · **简体中文**

这款应用可以帮你**从图片和视频中去除标志、水印、签名和文字叠加**。
只需**涂抹掉你想去除的部分**，应用就会自然地把它填补回来。所有处理都在
**你自己的电脑上**完成——**无需联网**，你的图片/视频**绝不会被上传到任何地方**。

---
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/dbcb0fad-cc38-49d6-b9c6-acd1c0e16983" />
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/f07d1f33-e835-4c6c-b5b6-6b8db94b9cb9" />

## 安装与打开

1. 运行安装程序（如果你收到的是压缩包，则先解压该文件夹）。
2. 打开 **AI Watermark Remover**（从桌面、开始菜单或 `.exe` 文件启动）。

> **Windows 弹出 "Windows protected your PC"（Windows 已保护你的电脑）？**
> 这是针对没有付费签名证书的应用的默认警告——**它不是病毒**。
> 点击 **More info → Run anyway**（更多信息 → 仍要运行）即可打开。

首次启动可能会稍慢一些；之后再打开会更快。

**共有两个版本：** **Pro** 版（图片 + 视频）和 **Lite** 版（仅图片，更轻量）。
查看窗口标题即可区分：**"Pro"** = 完整版，**"Lite"** = 轻量版（无法打开视频）。

---

## 使用方法 — 4 个步骤

### 第 1 步 — 打开图片/视频
- 点击**文档**按钮选择一个或多个文件，或点击**文件夹**按钮打开整个文件夹。
- 也可以直接把图片/视频**拖放**到窗口里。
- 打开多个文件时，底部会出现缩略图条；每一项上都有一个 **×**，可将其从列表中移除。

### 第 2 步 — 涂抹要去除的区域
在左侧栏中选择一个工具，然后在水印上涂抹/勾画（涂抹过的区域会显示为**淡红色**）：

| 工具 | 用途 |
|----|---|
| **画笔** | 涂抹水印（按住鼠标左键并拖动）。用下方的滑块调整画笔大小。 |
| **方框** | 在水印上拖出一个矩形，快速覆盖。 |
| **橡皮擦** | 擦掉多余的涂抹。 |
| **文字** | 输入文字以精确覆盖文字类水印。这段文字只是一个**标记**——处理后即会消失，不会被写入图片中。 |

涂多了？使用左侧栏中的**撤销 / 重做 / 全部清除 / 重置**。
再次点击工具按钮（或按 **Esc**）即可取消选中它。

> **提示：** 完整覆盖水印并稍微多涂一点——这样的效果比涂得不够更好。

### 第 3 步 — 点击运行
- **运行** — 处理当前打开的图片/视频。
- **全部运行** — 批量处理列表中所有**画面尺寸相同**的文件
  （仅当有 2 个或以上文件时可用）。

### 第 4 步 — 保存
- 点击**保存**。**每次保存时，应用都会让你为输出文件选择一个文件夹**。
- 想保留原文件？启用**"添加 _clean"**选项——新文件的名称会带上 `_clean` 后缀
  （例如 `photo.png` → `photo_clean.png`），这样原文件就不会被覆盖。

---

## 视频处理（Pro 版）

- 视频**不能用保存按钮保存**。点击**运行**（单个视频）或**全部运行**
  （多个视频）；应用会在开始时询问保存文件夹。
- 视频由 AI 逐帧处理，因此**比图片慢得多**——耐心等它跑完即可。

---

## 查看与实用功能

- **鼠标滚轮**：放大 / 缩小 · **按住鼠标中键并拖动**：平移 · **F** 键或**双击**：适应窗口。
- **房子**图标：打开主页。**地球**图标：切换语言（支持 9 种语言，包括越南语）。

## 键盘快捷键

| 操作 | 按键 |
|---|---|
| 撤销 / 重做 | `Ctrl+Z` / `Ctrl+Shift+Z` |
| 调整画笔大小 | `Ctrl` + 鼠标滚轮 |
| 适应窗口 | `F` 键或双击 |
| 取消选中工具 | `Esc` |
| 快速擦除（使用画笔时） | 按住**鼠标右键** |

---

## 支持的格式

- **图片：** JPG、PNG、WEBP、BMP、TIFF 以及其他常见图片格式。
- **视频：** MP4、MOV、MKV、AVI、WEBM、WMV、FLV……（Pro 版）。

## 疑难解答

| 问题 | 解决办法 |
|---|---|
| 打开时 Windows 报警 | 点击 **More info → Run anyway**（更多信息 → 仍要运行）（应用是安全的，只是没有做代码签名）。 |
| 无法打开视频 | 你用的是 **Lite** 版——仅支持图片。请改用 **Pro** 版。 |
| 去除后仍留有淡淡的痕迹 | 涂抹得**更完整一些，并稍微盖过边缘**，然后再次运行。 |
| 视频非常慢 | 属正常现象——视频处理很吃性能；请耐心等待，或使用带显卡的电脑。 |

祝使用愉快！
