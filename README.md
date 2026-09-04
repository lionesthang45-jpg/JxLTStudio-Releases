# JxLTStudio

### Công cụ quản lý JX1 Offline trên Windows · Liones Thắng Studio

Quản lý Server Power bằng WSL2, cấu hình Server, vật phẩm, Kỳ Trân Các và các công cụ hỗ trợ trong một giao diện.

> **1.2.20 · Bản thử nghiệm công khai**
> Bản này đã qua kiểm thử khởi động/tắt WSL2 và bộ cài trên máy phát triển. Chưa hoàn thành thử game qua đêm hoặc xác minh trên mọi cấu hình Windows. Hãy sao lưu dữ liệu trước khi cập nhật.

## Tải JxLTStudio 1.2.20

| Bạn cần gì? | Link tải | Dung lượng |
|---|---|---|
| **Cài lần đầu** — có Tool và Runtime WSL2 | [**TẢI BỘ CÀI ĐẦY ĐỦ**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Setup-1.2.20.exe) | Khoảng 403 MB |
| **Đã cài Tool** — chỉ cập nhật ứng dụng | [**TẢI BẢN CẬP NHẬT**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Patch-1.2.20.exe) | Khoảng 34 MB |
| Xác minh file tải | [SHA256SUMS.txt](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/SHA256SUMS.txt) | File văn bản |

[Thông tin phiên bản](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.2.20) · [Hướng dẫn cài đặt](INSTALL.md) · [Liên hệ hỗ trợ](https://www.facebook.com/lionesthang45/)

**Chọn file .exe ở các link trên. Không tải “Source code (zip/tar.gz)” để cài Tool.**

## Yêu cầu trước khi cài

- Windows 10 x64 từ build 19041 hoặc Windows 11 x64, phần cứng hỗ trợ WSL2.
- Bật ảo hóa CPU trong BIOS/UEFI nếu Windows yêu cầu.
- .NET 8 Desktop Runtime x86, Microsoft WebView2 và WSL2. Máy chưa có thành phần cần thiết có thể cần Internet, quyền quản trị và khởi động lại.
- Tối thiểu 8 GB trống để nhập Runtime Linux lần đầu; dữ liệu Server và Client cần thêm dung lượng.
- Chuẩn bị riêng Client và gói Server được phép sử dụng. **Bộ cài không kèm Server jxser.tgz hoặc dữ liệu người chơi.**

## Điểm mới trong 1.2.20

- Sửa cách truyền lệnh Bash sang WSL để tránh lỗi không xác nhận được phiên chạy nền.
- Duy trì phiên WSL nền khi đóng Tool; chống tạo phiên trùng.
- Không tự khởi động lại sau khi người dùng tắt WSL2 an toàn.
- Bổ sung thông tin lỗi của phiên nền; phát hiện WSL dừng trong lúc chờ Web.
- Bộ cài cập nhật ứng dụng và giữ Runtime hiện có.

Đóng cửa sổ Tool **không đồng nghĩa tắt Server**. Khi kết thúc, dùng **Tắt WSL2 an toàn** để chờ lưu dữ liệu và dừng MySQL trước khi đóng WSL.

## Hỗ trợ

Liên hệ [Liones Thắng Studio trên Facebook](https://www.facebook.com/lionesthang45/) với phiên bản Tool, mô tả thao tác và ảnh lỗi.

Trong Tool, mở **Nhật ký hệ thống → Xuất log hỗ trợ**. Kiểm tra nội dung trước khi gửi riêng cho người hỗ trợ; không đăng công khai mật khẩu, token, database hoặc thông tin người chơi.

## Về kho này

Kho này chỉ phân phối bộ cài, bản cập nhật và tài liệu; không công khai mã nguồn riêng của JxLTStudio.

Phần khởi động VLTK Offline tích hợp trong Server Power được ghi nhận tác giả **V.D.K**. Các thành phần bên thứ ba giữ bản quyền và điều kiện sử dụng tương ứng.
