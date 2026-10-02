<div align="center">

<img src="jxltstudio-wordmark-v1.png" alt="JxLTStudio — LT Studio" width="560">

# JxLTStudio 1.3.0

**JX1 Offline made easier**

Easy Mode · JX Doctor · JX Setup · JX Advanced

[**TẢI BỘ CÀI 1.3.0 — khoảng 410 MB**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.3.0/JxLTStudio-Setup-1.3.0.exe)

[Ghi chú đầy đủ](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.3.0) · [Hướng dẫn cài đặt](INSTALL.md) · [Liên hệ Fanpage](https://www.facebook.com/profile.php?id=61594062731594)

</div>

## Bắt đầu với 1.3.0

1. Chạy bộ cài và **chọn thư mục cài JxLTStudio**. Không bắt buộc cài vào ổ C:.
2. Mở **JX Doctor** để kiểm tra máy; chuẩn bị thành phần WSL2 khi được yêu cầu và hoàn tất reboot nếu cần.
3. Vào **JX Setup** để cài Client và GameServer từ nguồn tải JxLTStudio. Runtime đi kèm được tự nhận theo nơi bạn cài Studio.
4. Trở về Easy Mode, chọn **Khởi Động GameServer** để bật WSL/mở web 127.0.0.1; bật Server trong web rồi chọn **Vào Game**. Khi kết thúc dùng **Tắt GameServer**.

**Bộ cài kèm ServerRuntime gốc với giao diện web mới, không kèm Client/GameServer.** Hai gói game được tải trong Setup, không cần đăng nhập GitHub. Đây là bộ cài đầy đủ; chưa có Patch 1.3.0 riêng. Sao lưu và đóng Studio trước khi cập nhật.

## Điểm mới của 1.3.0

- **Easy Mode**: màn hình chào, ba lựa chọn chính, các nút mở web/vào game/tắt an toàn, Facebook và QR ủng hộ; bố cục cửa sổ nhỏ và fullscreen được điều chỉnh.
- **JX Doctor**: kết quả dễ hiểu bằng tiếng Việt, xuất báo cáo, chuẩn bị thành phần WSL2 sau xác nhận; ghi nhớ máy đã sẵn sàng không hết hạn theo thời gian.
- **JX Setup**: tải tự động, thanh tiến trình %, tránh trùng tên GameServer, bảo vệ Server cũ, dọn dữ liệu tải tạm và đồng bộ đường dẫn Server & Client sau khi cài thành công.
- **Lua Studio**: mở file Lua bên ngoài Server và tạo file mới, giữ gợi ý mã, trợ giúp JX1, snippets, chẩn đoán, diff và bảo vệ khi lưu.
- **Web 127.0.0.1**: hình nền, logo và giao diện mới đồng bộ với JxLTStudio. Lịch Sự Kiện tạm ẩn để hoàn thiện sau.
- **JX Advanced** giữ đầy đủ công cụ cũ: cấu hình, vật phẩm, kỹ năng, rơi đồ, Kỳ Trân Các, tài khoản/nhân vật, SimAI/hành trang, Lua, logs và backup.

## Yêu cầu và giới hạn

Windows 10 x64 build 19041+ hoặc Windows 11; hỗ trợ ảo hóa/WSL2; .NET 8 Desktop Runtime **x86** và WebView2. Cần internet để tải gói/thành phần thiếu; một số bước Windows cần quyền quản trị và reboot.

Runtime đã import trước đây **không bị tự sửa/thay thế** khi cập nhật Studio. Rootfs đi kèm có dữ liệu MySQL nền, không cam kết cơ sở dữ liệu trắng. Server mới cài chưa tự kích hoạt; chưa chứng nhận chạy nhiều Server đồng thời. Doctor kiểm tra Windows, không chứng nhận mọi lỗi game.

Regression **59/59 PASS** cùng kiểm thử offline UI/web và bộ cài; chưa chứng nhận mọi cấu hình máy hoặc chạy game dài hạn. Bộ cài chưa ký Authenticode. Không tự tắt Defender; SHA-256 chỉ kiểm tra tính toàn vẹn, không chứng nhận an toàn của tệp khi antivirus cảnh báo.

[SHA256SUMS.txt](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.3.0/SHA256SUMS.txt) · [Tất cả phiên bản](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases)

<details>
<summary>Giới thiệu và hướng dẫn phiên bản cũ 1.2.20 (lưu trữ)</summary>

> **Máy chưa có hoặc đang lỗi WSL2?** Dùng [**JxLTSetup 1.0.0**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/jxltsetup-v1.0.0) để kiểm tra Windows và cài/sửa chữa WSL2 trước. Công cụ độc lập, không chứa JxLTStudio và không chạm dữ liệu ServerRuntime.

<div align="center">

<img src="jxltstudio-wordmark-v1.png" alt="JxLTStudio — LT Studio" width="560">

### Một ứng dụng quản lý dành cho JX1 Offline phát triển bởi LT

Server Power · Cấu hình · Vật phẩm · Kỳ Trân Các

**WINDOWS 10 / 11** &nbsp; / &nbsp; **WSL2** &nbsp; / &nbsp; **GIAO DIỆN TIẾNG VIỆT**

[<img src="download-full.svg" alt="Tải bộ cài đầy đủ 1.2.20" width="250">](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Setup-1.2.20.exe)
[<img src="download-patch.svg" alt="Tải bản cập nhật 1.2.20" width="250">](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Patch-1.2.20.exe)

[Hướng dẫn cài đặt](INSTALL.md) &nbsp; · &nbsp; [Ghi chú phiên bản](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.2.20) &nbsp; · &nbsp; [Liên hệ hỗ trợ](https://www.facebook.com/lionesthang45/)

<img src="dashboard-hero-lt-v2.png" alt="Không gian sơn thủy xanh đậm và vàng đồng trong bộ nhận diện JxLTStudio" width="100%">

**LIONES THẮNG STUDIO**

*Từ khởi động máy chủ đến quản lý dữ liệu game — tập trung trong một giao diện.*

</div>

---

## Tổng Quan

JxLTStudio tập hợp các công cụ quản lý JX1 Offline trên Windows. Giao diện tiếng Việt với tông xanh đậm và vàng đồng giúp bạn làm việc với Server, cấu hình và dữ liệu game trong cùng một ứng dụng.

| Server & vận hành | Dữ liệu & nội dung game |
|---|---|
| **Server Power** — khởi động WSL2, bảng điều khiển Web và tắt an toàn. | **Cấu hình** — form trực quan, Event theo tháng, xem diff và backup trước khi upload. |
| **Server & Client** — tập trung thiết lập kết nối và đường dẫn làm việc. | **Vật phẩm & Kỳ Trân Các** — các công cụ hỗ trợ quản lý mặt hàng và dữ liệu vật phẩm. |
| **Nhật ký hệ thống** — xuất log hỗ trợ để kiểm tra khi có sự cố. | **Lua Studio & công cụ dữ liệu** — hỗ trợ quy trình chỉnh sửa nội dung game. |

## Nhìn gần hơn vào giao diện

<img src="event-configuration.png" alt="Giao diện cấu hình Event theo tháng: công tắc kích hoạt, chọn tháng, bật từng Event và xem diff trước khi upload" width="100%">

**Cấu hình Event theo tháng** · Bố cục chia nhóm, trạng thái dễ đọc và các bước xem diff / backup trước khi ghi dữ liệu.

<sub>Ảnh chụp giao diện từ quá trình phát triển; một số chi tiết có thể khác bản đang cài. Ảnh dùng để minh họa bố cục, không phải thiết lập bắt buộc cho Server của bạn.</sub>

---

## Chọn bản tải phù hợp

> **1.2.20 · Bản thử nghiệm công khai**
> Bản này đã qua kiểm thử khởi động/tắt WSL2 và bộ cài trên máy phát triển. Chưa hoàn thành thử game qua đêm hoặc xác minh trên mọi cấu hình Windows. Hãy sao lưu dữ liệu trước khi cập nhật.

### JxLTStudio 1.2.20

| Bạn cần gì? | Link tải | Dung lượng |
|---|---|---|
| **Cài lần đầu** — có Tool và Runtime WSL2 | [**TẢI BỘ CÀI ĐẦY ĐỦ**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Setup-1.2.20.exe) | Khoảng 403 MB |
| **Đã cài Tool** — chỉ cập nhật ứng dụng | [**TẢI BẢN CẬP NHẬT**](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/JxLTStudio-Patch-1.2.20.exe) | Khoảng 34 MB |
| Xác minh file tải | [SHA256SUMS.txt](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/download/v1.2.20/SHA256SUMS.txt) | File văn bản |

[Thông tin phiên bản](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.2.20) · [Hướng dẫn cài đặt](INSTALL.md) · [Liên hệ hỗ trợ](https://www.facebook.com/lionesthang45/)

**Chọn file .exe ở các link trên. Không tải “Source code (zip/tar.gz)” để cài Tool.**

## Bắt đầu trong 3 bước

| 01 · Cài đặt | 02 · Thiết lập | 03 · Vận hành |
|---|---|---|
| Chọn **Setup** nếu cài lần đầu; chọn **Patch** nếu đã có Tool. | Mở **Server Power**, kiểm tra ServerRuntime và khởi động WSL2. Chuẩn bị riêng Server và Client. | Theo dõi trong bảng Web. Khi kết thúc, chọn **Tắt WSL2 an toàn**. |

Đọc [hướng dẫn đầy đủ](INSTALL.md) trước khi nhập dữ liệu Server hoặc nâng cấp. Nếu Windows yêu cầu cài thành phần bổ sung hay khởi động lại, hãy hoàn tất bước đó trước khi tiếp tục.

<details>
<summary><strong>Yêu cầu hệ thống và các thành phần cần thiết</strong></summary>

- Windows 10 x64 từ build 19041 hoặc Windows 11 x64, phần cứng hỗ trợ WSL2.
- Bật ảo hóa CPU trong BIOS/UEFI nếu Windows yêu cầu.
- .NET 8 Desktop Runtime x86, Microsoft WebView2 và WSL2. Máy chưa có thành phần cần thiết có thể cần Internet, quyền quản trị và khởi động lại.
- Tối thiểu 8 GB trống để nhập Runtime Linux lần đầu; dữ liệu Server và Client cần thêm dung lượng.
- Chuẩn bị riêng Client và gói Server được phép sử dụng. **Bộ cài không kèm Server jxser.tgz hoặc dữ liệu người chơi.**

</details>

## Điểm mới trong 1.2.20

- Sửa cách truyền lệnh Bash sang WSL để tránh lỗi không xác nhận được phiên chạy nền.
- Duy trì phiên WSL nền khi đóng Tool; chống tạo phiên trùng.
- Không tự khởi động lại sau khi người dùng tắt WSL2 an toàn.
- Bổ sung thông tin lỗi của phiên nền; phát hiện WSL dừng trong lúc chờ Web.
- Bộ cài cập nhật ứng dụng và giữ Runtime hiện có.

Đóng cửa sổ Tool **không đồng nghĩa tắt Server**. Khi kết thúc, dùng **Tắt WSL2 an toàn** để chờ lưu dữ liệu và dừng MySQL trước khi đóng WSL.

## Cùng phát triển JxLTStudio

**JxLTAuto đang phát triển**, chưa phải chức năng Auto hoàn chỉnh. Những bạn thường xuyên treo game và muốn tham gia thử nghiệm có thể liên hệ Liones Thắng Studio để trao đổi.

### Cần hỗ trợ?

Liên hệ [Liones Thắng Studio trên Facebook](https://www.facebook.com/lionesthang45/) với phiên bản Tool, mô tả thao tác và ảnh lỗi.

Trong Tool, mở **Nhật ký hệ thống → Xuất log hỗ trợ**. Kiểm tra nội dung trước khi gửi riêng cho người hỗ trợ; File này không đăng công khai mật khẩu, token, database hoặc thông tin người chơi.

Lưu ý hiện tại vì số lượng người cần hỗ trợ khá nhiều và thời gian của mình có hạn vì mình còn phát triển thêm tính năng JxLTStudio & JxLTAuto, mình đã làm hướng dẫn rất chi tiết tại Github về cách cài đặt, nếu anh em nào muốn mình trực tiếp hỗ trợ cài đặt mình sẽ lấy chi phí là 50k - 100k - 200k hoặc nhiều hơn tùy tâm anh em và số tiền này mình sẽ gom lại và chuyển cho Mặt Trận Tổ Quốc vào cuối tháng, xin cảm ơn anh em.

## Về kho này

Kho này chỉ phân phối bộ cài, bản cập nhật và tài liệu; không công khai mã nguồn riêng của JxLTStudio.

Phần khởi động VLTK Offline tích hợp trong Server Power được lấy cảm hứng từ tác giả **V.D.K**. Các thành phần bên thứ ba giữ bản quyền và điều kiện sử dụng tương ứng.

---

<div align="center">

**JxLTStudio · Liones Thắng Studio**

[Tải phiên bản 1.2.20](https://github.com/lionesthang45-jpg/JxLTStudio-Releases/releases/tag/v1.2.20) &nbsp; · &nbsp; [Hướng dẫn](INSTALL.md) &nbsp; · &nbsp; [Facebook](https://www.facebook.com/lionesthang45/)

</div>


</details>
