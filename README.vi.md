<h1 align="center">AI Watermark Remover</h1>

<p align="center"><b>Tô lên logo, chữ ký, dòng chữ chèn hay watermark trên ảnh và video - AI tự vẽ lấp lại cho tự nhiên, chạy ngay trên máy bạn, không cần mạng.</b></p>

<p align="center">
  <a href="README.md">English</a> ·
  <b>Tiếng Việt</b> ·
  <a href="README.bn.md">বাংলা</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <a href="README.pt_BR.md">Português (BR)</a> ·
  <a href="README.ru.md">Русский</a> ·
  <a href="README.tr.md">Türkçe</a> ·
  <a href="README.ur.md">اردو</a> ·
  <a href="README.zh_CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Tải bản Lite cho Windows" src="https://img.shields.io/badge/T%E1%BA%A3i%20v%E1%BB%81-Windows%20Lite-0078D6?style=for-the-badge&logo=windows&logoColor=white"></a>&nbsp;
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Tải bản Lite cho macOS (Apple Silicon)" src="https://img.shields.io/badge/T%E1%BA%A3i%20v%E1%BB%81-macOS%20Apple%20Silicon%20Lite-000000?style=for-the-badge&logo=apple&logoColor=white"></a>&nbsp;
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3"><img alt="Tải bản Pro cho Windows (Google Drive)" src="https://img.shields.io/badge/T%E1%BA%A3i%20v%E1%BB%81-Windows%20Pro-76B900?style=for-the-badge&logo=windows&logoColor=white"></a>
</p>

---

## Cài đặt

### Bước 1 - Chọn đúng bản cho máy của bạn

Có hai bản. **Lite** xoá watermark trên **ảnh**, chạy bằng CPU. **Pro** xử lý **ảnh và video**, cần máy Windows có card NVIDIA. Tiêu đề cửa sổ ghi **"Lite"** hoặc **"Pro"** để bạn biết mình đang dùng bản nào.

| Máy của bạn | Tải tệp | Google Drive | Ghi chú |
|---|---|---|---|
| 🪟 **Windows 10/11 (64-bit)** - Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`Windows_AI_Watermark_Remover_Lite_…zip`) | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Chỉ ảnh · không cần card đồ hoạ |
| 🍎 **Mac chip Apple (M1/M2/M3/M4)** - Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`MacOS_AI-Watermark-Remover-Lite-arm64_…dmg`) | [macOS](https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l) | Chỉ ảnh · không có bản cho Mac chip Intel |
| 🪟 **Windows 10/11 (64-bit) + GPU NVIDIA** - Pro | - | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Ảnh **và video** · bản Pro chỉ phát hành trên Google Drive |

> Bản Pro cần card **NVIDIA** có CUDA - không hỗ trợ GPU AMD/Intel. Không có card NVIDIA thì dùng bản Lite (chỉ ảnh).

**Yêu cầu hệ thống**

| | |
|---|---|
| **Lite (ảnh)** | Windows 10/11 64-bit hoặc macOS chip Apple · không cần GPU · RAM 4 GB trở lên |
| **Pro (ảnh + video)** | Chỉ Windows 10/11 64-bit · GPU NVIDIA có CUDA, VRAM tối thiểu 4 GB (khuyên 6-8 GB cho video HD / dài) · RAM 8 GB trở lên |
| **CPU** | 64-bit có hỗ trợ AVX2 |
| **Cần cài sẵn (Windows)** | Visual C++ Redistributable 2015-2022 x64; bản Pro cần thêm driver NVIDIA mới |

### Bước 2 - Cài đặt

<details open>
<summary><b>🪟 Trên Windows</b></summary>

1. **Lite:** tải tệp `.zip` ở Releases rồi **giải nén**. **Pro:** tải trong thư mục Google Drive.
2. Chạy file cài đặt vừa tải (hoặc, nếu là thư mục chạy sẵn, mở **`AI Watermark Remover Lite.exe`** / **`AI Watermark Remover Pro.exe`** trong đó).
3. Nếu hiện **"Windows protected your PC"** (SmartScreen): bấm **More info** → **Run anyway**. *(App chưa ký chứng chỉ trả phí nên bị cảnh báo - không phải virus.)*
4. Trình cài đặt hỏi quyền admin (cài vào Program Files) và có tuỳ chọn tạo lối tắt ngoài Desktop. Mở app từ **Start Menu** hoặc **Desktop**.

Lite và Pro là hai bản cài riêng - có thể để cả hai trên cùng một máy và gỡ từng bản độc lập.

</details>

<details open>
<summary><b>🍎 Trên macOS</b></summary>

1. Mở tệp **`.dmg`** vừa tải, **kéo AI Watermark Remover Lite vào thư mục Applications**.
2. Vào **Applications**, **chuột phải** (hoặc Control-click) **AI Watermark Remover Lite** → **Open** → bấm **Open** lần nữa trong hộp thoại. *(App chưa được Apple ký nên **lần đầu** phải mở theo cách này; các lần sau mở bình thường.)*
3. Nếu macOS báo app **"bị hỏng / không mở được"**, hoặc không có nút Open, mở **Terminal** và dán:
   ```bash
   xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"
   ```
   Rồi mở lại app.

</details>

Lần mở đầu có thể hơi lâu, các lần sau sẽ nhanh hơn.

### Bước 3 - Miễn phí, không cần tài khoản

Cả hai bản đều **miễn phí** - không tài khoản, không key bản quyền, không giới hạn số tệp. Mô hình AI đóng gói sẵn trong app nên khi chạy app không tải gì về và **không gửi ảnh/video của bạn** đi đâu; mọi thứ chạy offline.

---

## Lần chạy đầu tiên

1. **Mở tệp.** Bấm nút **📄** để chọn một hay nhiều tệp, nút **📁** để mở cả thư mục, hoặc **kéo thả** tệp vào cửa sổ. Nếu các tệp khác tỉ lệ khung hình, app hỏi bạn muốn nạp tỉ lệ nào (hoặc tất cả).
2. **Tô lên watermark.** Chọn **Cọ**, **Khung** hoặc **Văn bản** ở cột Công cụ; vùng tô hiện **màu đỏ mờ**. Tô kín và lố ra ngoài mép một chút sẽ đẹp hơn tô thiếu.
3. **Bấm Chạy.** Kết quả thay vào vùng đã tô. Khi mở nhiều tệp, **Chạy tất cả** áp cùng vùng tô cho mọi tệp cùng kích thước.
4. **Bấm Lưu** và chọn thư mục lưu (mỗi lần lưu app đều hỏi). Muốn giữ tệp gốc thì bật **Thêm _clean** trước.

---

## Tính năng

- **Tô, khoanh khung hoặc gõ chữ** - tô tự do bằng Cọ, kéo Khung để che nhanh, xoá chỗ tô thừa bằng Tẩy, hoặc gõ chữ đè lên watermark dạng chữ để che cho chính xác. Chữ này chỉ để đánh dấu - xử lý xong sẽ biến mất, không dính vào ảnh.
- **Sửa vùng chọn** - Hoàn tác / Làm lại, Xóa toàn bộ vùng tô, hoặc Về gốc để lấy lại ảnh ban đầu.
- **Xử lý hàng loạt** - **Chạy tất cả** áp vùng tô hiện tại cho mọi tệp đang mở cùng tỉ lệ khung hình; tệp khác tỉ lệ được bỏ qua và báo số lượng khi xong.
- **Xoá watermark video (Pro)** - AI xử lý video từng khung hình, chỉ làm ở vùng quanh watermark, ghép kết quả về khung gốc và giữ nguyên tiếng gốc. Trình phát có sẵn cho tua xem với chất lượng xem trước 100 / 75 / 50 / 25%.
- **Lưu không đè tệp gốc** - Lưu một tệp rồi sang tệp kế, hoặc **Lưu tất cả** tệp đã xử lý vào một thư mục; **Thêm _clean** thêm hậu tố vào tên tệp mới (`anh.png` → `anh_clean.png`).
- **Offline và riêng tư** - mọi thứ chạy trên máy bạn, không tải lên đâu.
- **9 ngôn ngữ giao diện** - English, Tiếng Việt, বাংলা, हिन्दी, Português (BR), Русский, Türkçe, اردو, 简体中文 - đổi bằng biểu tượng quả địa cầu.

---

## Công cụ & điều khiển

### 📂 Mở

**📄** mở một hay nhiều tệp, **📁** mở cả thư mục, hoặc kéo tệp thẳng vào cửa sổ. Mở nhiều tệp thì có dải ảnh nhỏ ở dưới - bấm ảnh nhỏ để chuyển, hoặc dấu **×** để bỏ khỏi danh sách. Bản Lite chỉ nhận ảnh; tệp video bị lọc ra.

### 🖌 Công cụ

| Công cụ | Dùng để |
|---|---|
| **Cọ** | Tô lên watermark (giữ chuột trái và kéo). Chỉnh cỡ bằng thanh trượt, `Ctrl` + lăn chuột, hoặc `[` / `]`. Giữ **chuột phải** để tẩy ngay khi đang tô. |
| **Khung** | Kéo một khung chữ nhật phủ lên watermark cho nhanh. |
| **Tẩy** | Xoá bớt chỗ tô thừa. |
| **Văn bản** | Gõ chữ đè lên watermark dạng chữ để che chính xác (chỉ với ảnh). `Delete` xoá chữ đang chọn. |

Bấm lại nút công cụ, hoặc phím **Esc**, để bỏ chọn. **Hoàn tác / Làm lại / Xóa / Về gốc** nằm cùng cột.

### ▶ Chạy

**Chạy** xử lý tệp đang xem; **Chạy tất cả** (hiện khi mở từ 2 tệp) xử lý mọi tệp cùng tỉ lệ khung hình. Khi đang chạy, nút đổi thành **Dừng** / **Dừng tất cả**. Kết quả được giữ trong app cho tới khi bạn lưu.

### 🎬 Video (Pro)

Mở video, dừng ở khung bất kỳ và tô lên watermark bằng Cọ hoặc Khung (bắt đầu tô là video tự dừng phát). Dùng nút phát và thanh tua để xem lại, chọn chất lượng xem trước (100 / 75 / 50 / 25%) cho nhẹ máy. Video xử lý từng khung hình nên **chậm hơn ảnh khá nhiều** - cứ để nó chạy. Xong thì lưu bằng **Lưu** hoặc **Lưu tất cả** như ảnh; tệp xuất ra là `.mp4`.

### 💾 Lưu

**Lưu** ghi kết quả hiện tại rồi chuyển sang tệp kế; **Lưu tất cả** ghi mọi tệp đã xử lý vào một thư mục. Mỗi lần lưu app đều hỏi thư mục. Bật **Thêm _clean** để thêm `_clean` vào tên tệp thay vì dùng lại tên gốc.

### 🔍 Xem

Lăn chuột để phóng to/thu nhỏ, giữ chuột giữa và kéo để di chuyển, phím **F** hoặc nháy đúp để vừa khung. Biểu tượng **ngôi nhà** mở trang chủ; **quả địa cầu** đổi ngôn ngữ.

### ⌨️ Phím tắt

| Thao tác | Phím |
|---|---|
| Hoàn tác / Làm lại | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Cỡ cọ | `Ctrl` + lăn chuột, hoặc `[` / `]` |
| Vừa khung | `F`, `0` hoặc nháy đúp |
| Bỏ chọn công cụ | `Esc` |
| Tẩy nhanh (khi đang dùng Cọ) | Giữ **chuột phải** |
| Di chuyển ảnh | Giữ **chuột giữa** và kéo |

### 🗂 Định dạng hỗ trợ

- **Ảnh:** PNG, JPG/JPEG, WEBP, BMP, TIFF, PPM/PGM/PBM/PNM.
- **Video (Pro):** MP4, M4V, MOV, WEBM, MKV, AVI, FLV, WMV, MPG/MPEG, TS/M2TS/MTS, 3GP, OGV. Tệp xuất ra là `.mp4`.

---

## Nơi lưu dữ liệu

| Cái gì | Windows | macOS |
|---|---|---|
| Ảnh / video đã xuất | Thư mục bạn chọn khi lưu | Thư mục bạn chọn khi lưu |
| Cài đặt (ngôn ngữ, Thêm _clean) | Registry: `HKEY_CURRENT_USER\Software\Duckmartians\AI Watermark Remover` | `~/Library/Preferences/com.duckmartians.AI Watermark Remover.plist` |
| Kết quả chưa lưu (tạm) | `%TEMP%\AIWatermarkRemover_work` | `AIWatermarkRemover_work` trong thư mục tạm của hệ thống |
| Nhật ký lỗi | `%APPDATA%\AI Watermark Remover\crash.log` | `~/AI Watermark Remover/crash.log` |

Thư mục tạm được dọn mỗi lần mở app - **hãy lưu kết quả trước khi đóng app**.

---

## Khắc phục sự cố

**Windows chặn với "Windows protected your PC"** - bấm **More info → Run anyway**. App chưa ký chứng chỉ trả phí nên bị cảnh báo - không phải virus.

**macOS báo app bị hỏng / không mở được** - app chưa được Apple ký. Lần đầu chuột phải → **Open**, hoặc chạy `xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"`.

**Không mở được video** - bạn đang dùng bản **Lite**, chỉ xử lý ảnh. Cài bản **Pro** (Windows + card NVIDIA) để xoá watermark video.

**Bấm Lưu thì báo video xuất bằng "Chạy"** - video đó chưa được xử lý. Bấm **Chạy** (hoặc **Chạy tất cả**) trước, rồi mới **Lưu**.

**Chạy tất cả bỏ qua một số tệp** - Chạy tất cả chỉ xử lý tệp cùng tỉ lệ khung hình với tệp bạn đã tô. Mở các tệp kia riêng, hoặc chọn tỉ lệ của chúng khi mở.

**Xoá xong vẫn còn vết mờ** - tô kín hơn và lố ra ngoài mép watermark một chút rồi Chạy lại. Vùng lớn trên nền nhiều chi tiết vẫn có thể còn dấu vết.

**Video chạy rất lâu** - bình thường: AI xử lý từng khung hình nên video lâu hơn ảnh nhiều. Cứ để nó chạy; clip ngắn hơn và card nhiều VRAM hơn sẽ xong nhanh hơn.

**App tự tắt** - khi báo lỗi, gửi kèm tệp `crash.log` (xem bảng ở trên).

---

Chỉ xoá watermark và logo trên ảnh, video bạn sở hữu hoặc có quyền chỉnh sửa.
