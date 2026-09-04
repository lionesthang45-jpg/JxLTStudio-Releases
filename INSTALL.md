# Hướng dẫn cài đặt và cập nhật

## Cài lần đầu

1. Tải **JxLTStudio-Setup-1.2.20.exe** từ [trang phát hành](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.2.20).
2. Chạy bộ cài. Nếu thiếu .NET hoặc WebView2, làm theo thông báo cài thành phần Microsoft.
3. Mở Tool → **Server Power**. Thông thường Tool tự nhận thư mục **ServerRuntime** cạnh ứng dụng.
4. Bấm **Khởi động WSL2**. Nếu cần bật thành phần Windows, hoàn tất cài đặt và khởi động lại máy khi được yêu cầu.
5. Đợi bảng điều khiển Web sẵn sàng. Gói Server .tgz và Client phải chuẩn bị riêng.
6. Khi tải gói Server lên Linux, kiểm tra thư mục đích. Chỉ chọn giải nén khi hiểu nội dung gói và đã dừng dịch vụ game; không ghi đè dữ liệu đang sử dụng.

## Cập nhật từ bản đã cài

1. Sao lưu dữ liệu quan trọng; nên kết thúc phiên game và **Tắt WSL2 an toàn**.
2. Đóng JxLTStudio.
3. Chạy **JxLTStudio-Patch-1.2.20.exe** và chọn đúng thư mục JxLTStudio hiện tại.
4. Mở Tool, kiểm tra phiên bản **1.2.20**, rồi khởi động WSL2.

Bản vá không chứa ServerRuntime và không yêu cầu nhập lại Server .tgz. Không xóa distro hoặc ổ WSL để cập nhật.

## Khi sử dụng hằng ngày

**Khởi động WSL2 → chờ Web → bật dịch vụ Server → chơi game → tắt WSL2 an toàn.**

- Đóng/mở lại Tool không tự tắt Server đang chạy.
- Web/MySQL có thể đang chạy trong khi Goddess, Bishop, S3Relay và GameServer vẫn tắt.
- Nếu tắt an toàn báo chưa dừng sạch dịch vụ, giữ WSL chạy và gửi log hỗ trợ; không tắt cưỡng chế để bỏ qua cảnh báo.

## Kiểm tra file tải

Mở PowerShell trong thư mục chứa file tải, chạy:

```powershell
Get-FileHash -Algorithm SHA256 .\JxLTStudio-Setup-1.2.20.exe
```

Đối chiếu với **SHA256SUMS.txt** cùng phiên bản. Với bản vá, thay bằng tên file Patch.
Mã khớp giúp xác minh file tải không bị thay đổi; không thay thế chữ ký số hoặc việc kiểm tra nguồn phát hành.

Nếu Windows hoặc phần mềm bảo mật cảnh báo, kiểm tra nguồn tải và liên hệ hỗ trợ. Không tắt phần mềm bảo mật để cài.

## Báo lỗi

Gửi phiên bản Tool, phiên bản Windows, thao tác trước khi lỗi và ảnh thông báo.
Dùng **Nhật ký hệ thống → Xuất log hỗ trợ** khi cần, kiểm tra và gửi riêng; không đưa dữ liệu nhạy cảm lên kho công khai.
