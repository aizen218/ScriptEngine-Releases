# ScriptEngine

**ScriptEngine** là ứng dụng desktop hiện đại giúp quản lý các hồ sơ (profile) trình duyệt cô lập, mỗi profile có thể gán một proxy riêng.  
Xây dựng với **Avalonia UI** và **.NET 10** — chạy gốc (native AOT), không cần cài đặt runtime.

---

## Tính năng chính

### Quản lý Profile
- Tạo, sửa, nhân bản và xoá profile trình duyệt
- Mỗi profile chạy trong thư mục `--user-data-dir` riêng biệt, dữ liệu hoàn toàn cô lập
- Theo dõi trạng thái real-time: sẵn sàng, đang chạy, đang dừng
- Thư mục profile tự động tạo khi chạy lần đầu, tự động đổi tên khi rename, tự động xoá khi xoá profile

### Hỗ trợ trình duyệt
- Tự động phát hiện trình duyệt đã cài đặt (Chrome, Chromium, Edge, Brave, Opera, Vivaldi)
- Mỗi profile có thể chọn trình duyệt riêng
- Khởi động với cờ `--no-first-run` và `--no-default-browser-check`

### Proxy Routing
- Gán proxy (HTTP, HTTPS, SOCKS4, SOCKS5) cho từng profile
- Kiểm tra sức khoẻ proxy tích hợp: đo độ trễ, ghi log kiểm tra
- Import hàng loạt proxy từ danh sách
- Xem proxy nào đang được profile nào sử dụng

### Tìm kiếm & Lọc
- Tìm kiếm real-time theo tên profile, trình duyệt, proxy, loại proxy
- Lọc danh sách proxy theo trạng thái

### Thư mục Profiles
- Cấu hình thư mục lưu profile tuỳ ý
- Toàn bộ profile được tổ chức gọn gàng dưới một thư mục gốc

---

## Tải về

| Nền tảng  | Kiến trúc | Định dạng   |
|-----------|-----------|-------------|
| Windows   | x64       | `.zip`      |
| Linux     | x64       | `.tar.gz`   |

> Hỗ trợ macOS (ARM64 & Intel) sẽ có trong bản cập nhật sau.

---

## Yêu cầu hệ thống

- **Windows 10** 1809+ / Windows 11
- **Linux**: Ubuntu 22.04+, Fedora 38+, hoặc bất kỳ distro nào tương thích
- **macOS**: *Sắp ra mắt*

Không cần cài đặt .NET Runtime — ứng dụng đã được biên dịch **AOT** hoàn toàn.

---

## Hướng dẫn nhanh

1. Tải file cho nền tảng của bạn từ trang [Releases](https://github.com/aizen218/ScriptEngine-Releases/releases)
2. Giải nén vào thư mục bất kỳ
3. Chạy `ScriptEngine`

Lần đầu khởi động, ứng dụng sẽ tự động quét trình duyệt đã cài đặt và tạo cơ sở dữ liệu SQLite cục bộ.

---

## Tính năng sắp tới

- **Hỗ trợ macOS** – Bản dựng gốc cho Apple Silicon (ARM64) và Intel
- **Tự động hoá workflow** – Ghi và phát lại các thao tác trình duyệt (click, điền form, điều hướng)
- **Import/Export profile** – Chia sẻ profile giữa các máy
- **Nhóm profile** – Gom profile vào nhóm để thao tác hàng loạt
- **Chuyển đổi giao diện Sáng/Tối**
- **Giao diện dòng lệnh (CLI)** – Khởi động profile từ terminal

---

## Công nghệ sử dụng

- **Avalonia UI** – Framework desktop đa nền tảng
- **.NET 10** – Native AOT publishing, hiệu năng cao
- **CommunityToolkit.Mvvm** – Source generators cho mô hình MVVM
- **Material.Icons** – Bộ icon hiện đại
- **SQLite** – Lưu trữ dữ liệu cục bộ

---

## Giấy phép

MIT
