# ScriptEngine

Ứng dụng desktop quản lý profile trình duyệt cô lập, gán proxy riêng cho từng profile.  
Xây dựng với **Avalonia UI** + **.NET 10 AOT** — chạy native, không cần runtime.

[![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![NativeAOT](https://img.shields.io/badge/NativeAOT-ready-512BD4?logo=dotnet)](https://learn.microsoft.com/dotnet/core/deploying/native-aot/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Chức năng

- **Quản lý profile:** tạo, sửa, nhân bản, xoá profile trình duyệt — mỗi profile có `--user-data-dir` riêng, cô lập hoàn toàn
- **Trình duyệt:** tự động phát hiện Chrome, Chromium, Edge, Brave, Opera, Vivaldi
- **Proxy:** gán HTTP/HTTPS/SOCKS4/SOCKS5 cho từng profile, kiểm tra sống/độ trễ, import hàng loạt
- **Workflow Automation:** thiết kế workflow trực quan (29 node), chạy tự động trên nhiều profile với điều chỉnh cửa sổ lưới
- **Tìm kiếm & lọc real-time**
- **Tự động xoá/đổi tên thư mục profile**

## Platform

| Nền tảng | Định dạng |
|----------|-----------|
| Windows x64 | `.zip` |
| Linux x64 | `.tar.gz` |

Không cần .NET Runtime — đã biên dịch AOT hoàn toàn.

## Giấy phép

MIT
