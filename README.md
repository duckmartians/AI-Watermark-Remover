# AI Watermark Remover — Hướng dẫn sử dụng

Ứng dụng giúp bạn **xóa logo chìm, chữ ký, dòng chữ (watermark) trên ảnh và video**.
Bạn chỉ cần **tô lên chỗ muốn xóa**, ứng dụng sẽ tự vẽ lấp lại cho tự nhiên. Mọi thứ xử lý
ngay trên máy bạn — **không cần mạng**, ảnh/video **không bị gửi đi đâu**.

---

## Cài đặt & mở ứng dụng

1. Chạy file cài đặt (hoặc giải nén thư mục nếu được gửi dạng nén).
2. Mở **AI Watermark Remover** (từ màn hình Desktop, menu Start, hoặc file `.exe`).

> **Windows hiện cảnh báo "Windows protected your PC"?**
> Đây là cảnh báo mặc định cho ứng dụng chưa mua chứng chỉ, **không phải virus**.
> Bấm **More info → Run anyway** (Thêm thông tin → Vẫn chạy) là mở được.

Lần đầu mở có thể hơi lâu một chút, những lần sau sẽ nhanh hơn.

**Có hai bản:** bản **Đầy đủ** (ảnh + video) và bản **Nhẹ** (chỉ ảnh, chạy nhẹ hơn).
Nhìn tiêu đề cửa sổ: có chữ **"Lite"** nghĩa là bản Nhẹ (không mở được video).

---

## Cách dùng — 4 bước

### Bước 1 — Mở ảnh/video
- Bấm nút **hình tờ giấy** để chọn một hay nhiều tệp, hoặc nút **hình thư mục** để mở cả thư mục.
- Hoặc **kéo thả** ảnh/video thẳng vào cửa sổ.
- Mở nhiều tệp thì có dải ảnh nhỏ ở dưới; mỗi ảnh có dấu **×** để bỏ ra khỏi danh sách.

### Bước 2 — Tô lên chỗ cần xóa
Chọn công cụ ở cột bên trái, rồi tô/khoanh lên watermark (vùng tô hiện **màu đỏ mờ**):

| Công cụ | Dùng để |
|---|---|
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

## Xử lý video (bản Đầy đủ)

- Video **không lưu bằng nút Lưu**. Hãy bấm **Chạy** (một video) hoặc **Chạy tất cả**
  (nhiều video); ứng dụng sẽ hỏi thư mục lưu khi bắt đầu.
- Video xử lý bằng AI theo từng khung hình nên **chậm hơn ảnh khá nhiều** — cứ để yên cho nó chạy.

---

## Xem ảnh & tiện ích

- **Lăn chuột**: phóng to / thu nhỏ · **Giữ chuột giữa và kéo**: di chuyển ảnh · phím **F** hoặc **nháy đúp**: vừa khung.
- Biểu tượng **ngôi nhà**: mở trang chủ. Biểu tượng **quả địa cầu**: đổi ngôn ngữ (hỗ trợ 9 thứ tiếng, có Tiếng Việt).

## Phím tắt

| Thao tác | Phím |
|---|---|
| Hoàn tác / Làm lại | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Đổi cỡ cọ | `[` `]` hoặc `Ctrl` + lăn chuột |
| Vừa khung | `F` hoặc nháy đúp |
| Bỏ chọn công cụ | `Esc` |
| Tẩy nhanh (khi đang dùng Cọ) | Giữ **chuột phải** |

---

## Định dạng mở được

- **Ảnh:** JPG, PNG, WEBP, BMP, TIFF và các định dạng ảnh phổ biến khác.
- **Video:** MP4, MOV, MKV, AVI, WEBM, WMV, FLV… (bản Đầy đủ).

## Gặp trục trặc?

| Hiện tượng | Cách xử lý |
|---|---|
| Windows cảnh báo khi mở | Bấm **More info → Run anyway** (ứng dụng an toàn, chỉ chưa mua chứng chỉ). |
| Không mở được video | Bạn đang dùng bản **Nhẹ (Lite)** — chỉ hỗ trợ ảnh. Hãy dùng bản Đầy đủ. |
| Xóa xong vẫn còn vết mờ | Tô **kín và lố hơn** một chút rồi Chạy lại. |
| Video chạy rất lâu | Bình thường — video xử lý nặng, hãy chờ hoặc dùng máy có card đồ họa. |

Chúc bạn dùng vui vẻ!
