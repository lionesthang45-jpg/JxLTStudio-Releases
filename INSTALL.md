# Hướng dẫn JxLTStudio 1.3.0

## 1. Cài Studio

[Tải bộ cài đầy đủ 1.3.0](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.3.0/JxLTStudio-Setup-1.3.0.exe). Chọn file .exe, không dùng Source code (zip/tar.gz).

Chạy bộ cài và chọn thư mục ở ổ bạn muốn. Nếu thiếu .NET 8 Desktop Runtime **x86** hoặc WebView2, làm theo thông báo thành phần Microsoft. Bộ cài chứa ServerRuntime gốc với web mới; không chứa Client hoặc GameServer.

## 2. Kiểm tra máy

Mở Studio → **JX Doctor → Kiểm tra máy của tôi**. Nếu máy chưa sẵn sàng, xem hướng dẫn và chọn **Cài Đặt Máy Ảo** khi phù hợp. Chỉ thực hiện sau khi đồng ý; có thể cần quyền quản trị, bật ảo hóa trong BIOS/UEFI hoặc reboot. Máy đã được xác minh thành công không phải kiểm tra lại chỉ vì hết thời gian.

## 3. Cài Client và GameServer

Mở **JX Setup**, chọn thư mục Client mới rồi bấm **Cài Client**. Gói được tải từ JxLTStudio, không cần tài khoản GitHub; chờ thanh tiến trình hoàn thành.

Ở **Cài GameServer**, Studio tự nhận ServerRuntime cạnh ứng dụng. Nếu cần chuẩn bị môi trường mới, đọc và xác nhận thông báo. Sau đó chọn cài GameServer. Không tự dùng/ghi đè Runtime khác; không đổi tên hoặc ghi đè Server cũ. Khi trùng tên jxser, Studio chọn tên chưa dùng như jxser1.

Sau khi hoàn tất, đường dẫn được đồng bộ sang Server & Client. **Xóa dữ liệu thừa sau khi cài đặt** dọn dữ liệu tải tạm được quản lý, không xóa phần đã cài. Server chưa tự start hoặc migrate SQL.

## 4. Sử dụng hằng ngày

Trở về **Easy Mode → Khởi Động GameServer**. WSL đang chạy thì mở trực tiếp web 127.0.0.1; chưa chạy thì bật WSL rồi mở web. Bật các dịch vụ Server trong web, sau đó chọn **Vào Game** (chọn Client nếu chưa có).

Kết thúc phiên game và dùng **Tắt GameServer** để dừng theo quy trình, rồi tắt riêng WSL đã chọn. Đóng cửa sổ Studio không đồng nghĩa tắt Server. Nếu dừng an toàn báo lỗi, giữ Runtime để kiểm tra và gửi log; không cưỡng chế bỏ qua.

## Cập nhật và lưu ý

Sao lưu, kết thúc phiên game an toàn và đóng Studio. Chạy bộ cài 1.3.0, chọn đúng thư mục Studio đang dùng. Chưa có Patch 1.3.0 riêng. Không xóa distro/ổ WSL để cập nhật.

Runtime đã import được giữ nguyên, không tự nâng cấp web hoặc thay rootfs. Runtime mới tạo từ bộ cài này có web mới. Chọn nơi cài Studio khác không tự di chuyển Runtime, Client hay dữ liệu Server cũ.

Rootfs có dữ liệu MySQL nền sẵn có, không phải chứng nhận database trắng. Chưa chứng nhận chạy nhiều GameServer đồng thời hoặc mọi cấu hình máy. Xem [ghi chú và giới hạn 1.3.0](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.3.0).

## Xác minh và hỗ trợ

Dùng PowerShell: Get-FileHash -Algorithm SHA256 .\JxLTStudio-Setup-1.3.0.exe

Đối chiếu [SHA256SUMS.txt](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.3.0/SHA256SUMS.txt). SHA-256 kiểm tra tính toàn vẹn, không thay thế đánh giá an toàn hoặc chữ ký số. Không vô hiệu hóa Defender để bỏ qua cảnh báo.

Gửi ảnh lỗi và phiên bản Windows/Studio tới [Fanpage](https://www.facebook.com/profile.php?id=61594062731594). Báo cáo Doctor hoặc Nhật ký hệ thống → Xuất log hỗ trợ nên được kiểm tra và gửi riêng, không công khai mật khẩu, token, database hoặc dữ liệu người chơi.

<details>
<summary>Hướng dẫn cũ 1.2.20 (lưu trữ)</summary>

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


</details>
