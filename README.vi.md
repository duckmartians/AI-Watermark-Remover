# AI Watermark Remover — Hướng dẫn sử dụng

<p align="left">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest">
    <img src="https://img.shields.io/badge/Phiên%20bản%20Windows-%F0%9F%92%BB-0078D6?style=for-the-badge&logo=windows&logoColor=white">
  </a>
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest">
    <img src="https://img.shields.io/badge/Phiên%20bản%20macOS-%F0%9F%8D%8E-000000?style=for-the-badge&logo=apple&logoColor=white">
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

🌐 [English](README.md) · **Tiếng Việt** · [বাংলা](README.bn.md) · [हिन्दी](README.hi.md) · [Português (BR)](README.pt_BR.md) · [Русский](README.ru.md) · [Türkçe](README.tr.md) · [اردو](README.ur.md) · [简体中文](README.zh_CN.md)

Ứng dụng giúp bạn **xóa logo chìm, chữ ký, dòng chữ (watermark) trên ảnh và video**.
Bạn chỉ cần **tô lên chỗ muốn xóa**, ứng dụng sẽ tự vẽ lấp lại cho tự nhiên. Mọi thứ xử lý
ngay trên máy bạn — **không cần mạng**, ảnh/video **không bị gửi đi đâu**.

---
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/dbcb0fad-cc38-49d6-b9c6-acd1c0e16983" />
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/f07d1f33-e835-4c6c-b5b6-6b8db94b9cb9" />

## Cài đặt & mở ứng dụng

1. Chạy file cài đặt (hoặc giải nén thư mục nếu được gửi dạng nén).
2. Mở **AI Watermark Remover** (từ màn hình Desktop, menu Start, hoặc file `.exe`).

> **Windows hiện cảnh báo "Windows protected your PC"?**
> Đây là cảnh báo mặc định cho ứng dụng chưa mua chứng chỉ, **không phải virus**.
> Bấm **More info → Run anyway** (Thêm thông tin → Vẫn chạy) là mở được.

Lần đầu mở có thể hơi lâu một chút, những lần sau sẽ nhanh hơn.

**Có hai bản:** bản **Pro** (ảnh + video) và bản **Lite** (chỉ ảnh, chạy nhẹ hơn).
Nhìn tiêu đề cửa sổ để biết bản nào: chữ **"Pro"** = bản đầy đủ, chữ **"Lite"** = bản nhẹ (không mở được video).

---

## Cấu hình yêu cầu

| | **Lite** (ảnh) | **Pro** (ảnh + video) |
|---|---|---|
| Nền tảng | **Windows 10/11** 64-bit **và macOS** | **chỉ Windows 10/11 64-bit** — *không có macOS* |
| CPU | 64-bit, có **AVX2** | 64-bit, có **AVX2** |
| GPU | **không cần** — chạy bằng CPU | **bắt buộc GPU NVIDIA có CUDA** |
| VRAM | — | tối thiểu 4 GB · **khuyến nghị 6–8 GB** (video HD / dài) |
| RAM | 4 GB trở lên | 8 GB trở lên |
| Cài thêm (Windows) | **Visual C++ Redistributable 2015–2022 x64** | như trên + **driver NVIDIA** mới |

- Bản **Pro** xử lý video bằng **nhân CUDA của NVIDIA**, nên **chỉ chạy trên Windows và bắt buộc có card đồ họa NVIDIA** — cỡ **RTX 2060 (dòng RTX 20 / GTX 16, kiến trúc "Turing") trở lên**.
- **macOS không có CUDA** → trên máy Mac hãy dùng bản **Lite** (xử lý ảnh). GPU AMD/Intel cũng **không chạy được** engine video của bản Pro.
- **Xóa ẢNH** (cả hai bản) chạy tốt **bằng CPU**, không cần card đồ họa.
- Không cần mạng, không gửi dữ liệu đi đâu — mọi thứ chạy tại máy.

---

## Cách dùng — 4 bước

### Bước 1 — Mở ảnh/video
- Bấm nút **hình tờ giấy** để chọn một hay nhiều tệp, hoặc nút **hình thư mục** để mở cả thư mục.
- Hoặc **kéo thả** ảnh/video thẳng vào cửa sổ.
- Mở nhiều tệp thì có dải ảnh nhỏ ở dưới; mỗi ảnh có dấu **×** để bỏ ra khỏi danh sách.

### Bước 2 — Tô lên chỗ cần xóa
Chọn công cụ ở cột bên trái, rồi tô/khoanh lên watermark (vùng tô hiện **màu đỏ mờ**):

| Công cụ | Dùng để |
|----|---|
| **Cọ** | Tô lên watermark (giữ chuột trái và kéo). Cỡ cọ chỉnh bằng thanh trượt bên dưới. |
| **Khung** | Kéo một khung chữ nhật phủ lên watermark cho nhanh. |
| **Tẩy** | Xóa bớt chỗ tô thừa. |
| **Văn bản** | Gõ chữ để che watermark dạng chữ cho chính xác. Chữ này chỉ để **đánh dấu**, xóa xong sẽ biến mất chứ không dính vào ảnh. |

Tô lố thì dùng **Hoàn tác / Làm lại / Xóa hết / Về gốc** ở cột trái để sửa.
Bấm lại vào nút công cụ (hoặc phím **Esc**) để bỏ chọn.

> **Mẹo:** tô trùm kín watermark, hơi lố ra ngoài một chút, kết quả sẽ đẹp hơn là tô thiếu.

### Bước 3 — Bấm Chạy
- **Chạy** — xử lý ảnh/video đang mở.
- **Chạy tất cả** — làm hàng loạt cho mọi tệp **cùng khung hình** trong danh sách
  (chỉ bật khi có từ 2 tệp trở lên).

### Bước 4 — Lưu
- Bấm **Lưu**. **Mỗi lần lưu, ứng dụng sẽ hỏi bạn chọn thư mục** để cất tệp kết quả.
- Muốn giữ lại ảnh gốc? Bật ô **"Thêm _clean"** — tệp mới sẽ có thêm chữ `_clean`
  trong tên (ví dụ `anh.png` → `anh_clean.png`), không đè lên ảnh gốc.

---

## Xử lý video (bản Pro)

- Video **không lưu bằng nút Lưu**. Hãy bấm **Chạy** (một video) hoặc **Chạy tất cả**
  (nhiều video); ứng dụng sẽ hỏi thư mục lưu khi bắt đầu.
- Video xử lý bằng AI theo từng khung hình trên **GPU** nên chậm hơn ảnh — cứ để yên cho nó chạy.

### Thanh trượt Tốc độ ⇄ Chất lượng

Ngay dưới thanh **Cỡ cọ** (cột trái, **chỉ bản Pro**) có 4 thanh trượt để bạn cân **tốc độ và chất lượng**.
Rê chuột vào từng thanh sẽ hiện giải thích. Ứng dụng tự nhớ vị trí bạn chỉnh.

| Thanh trượt | Điều khiển gì | Nhanh hơn | Nét hơn |
|---|---|---|---|
| **Độ phân giải** | Độ phân giải khi xử lý — **đòn bẩy tốc độ mạnh nhất**. Thấp = nhanh hơn nhiều, vùng xóa hơi mờ. | ~**50** | **100** |
| **Chuyển động** | Độ kỹ khi phân tích chuyển động giữa các khung (chất lượng gần như không đổi). | **2–4** | 20 |
| **Số khung xét** | Số khung gần nhau xử lý cùng lúc. | thấp | cao |
| **Khung tham chiếu** | Khoảng cách khi lấy khung tham chiếu. | **cao** | thấp |

- **Muốn nhanh?** Đặt **Độ phân giải ≈ 50** và **Chuyển động ≈ 4** (mặc định đã ưu tiên tốc độ).
- **Vùng xóa bị mờ?** Kéo **Độ phân giải** lên gần **100**.
- Các thông số này chỉ ảnh hưởng **video**; xử lý ảnh không bị ảnh hưởng.

---

## Xem ảnh & tiện ích

- **Lăn chuột**: phóng to / thu nhỏ · **Giữ chuột giữa và kéo**: di chuyển ảnh · phím **F** hoặc **nháy đúp**: vừa khung.
- Biểu tượng **ngôi nhà**: mở trang chủ. Biểu tượng **quả địa cầu**: đổi ngôn ngữ (hỗ trợ 9 thứ tiếng, có Tiếng Việt).

## Phím tắt

| Thao tác | Phím |
|---|---|
| Hoàn tác / Làm lại | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Đổi cỡ cọ | `Ctrl` + lăn chuột |
| Vừa khung | `F` hoặc nháy đúp |
| Bỏ chọn công cụ | `Esc` |
| Tẩy nhanh (khi đang dùng Cọ) | Giữ **chuột phải** |

---

## Định dạng mở được

- **Ảnh:** JPG, PNG, WEBP, BMP, TIFF và các định dạng ảnh phổ biến khác.
- **Video:** MP4, MOV, MKV, AVI, WEBM, WMV, FLV… (bản Pro).

## Gặp trục trặc?

| Hiện tượng | Cách xử lý |
|---|---|
| Windows cảnh báo khi mở | Bấm **More info → Run anyway** (ứng dụng an toàn, chỉ chưa mua chứng chỉ). |
| Không mở được video | Bạn đang dùng bản **Lite** (nhẹ) — chỉ hỗ trợ ảnh. Hãy dùng bản **Pro**. |
| Xóa xong vẫn còn vết mờ | Tô **kín và lố hơn** một chút rồi Chạy lại. |
| Video chạy rất lâu | Kéo thanh **Độ phân giải** xuống (~50) và **Chuyển động** (~4) — xem *Thanh trượt Tốc độ ⇄ Chất lượng*. Nên dùng GPU NVIDIA có CUDA (RTX 2060 trở lên) — xem *Cấu hình yêu cầu*. |

Chúc bạn dùng vui vẻ!
