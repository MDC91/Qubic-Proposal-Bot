<div align="center">

# 🤖 Bot Đề Xuất Qubic

### **Tóm Tắt Đề Xuất Tự Động Cho Cộng Đồng Qubic Bằng 13 Ngôn Ngữ**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
</div>

## 📖 Mục Lục

- [🚀 Về Dự Án](#-về-dự-án)
- [🏗️ Kiến Trúc & Công Nghệ](#️-kiến-trúc--công-nghệ)
- [📋 Ngôn Ngữ Được Hỗ Trợ](#-ngôn-ngữ-được-hỗ-trợ)
- [🎯 Tính Năng Chi Tiết](#-tính-năng-chi-tiết)
- [💬 Sử Dụng Discord](#-sử-dụng-discord)
  - [Thêm Bot Vào Máy Chủ Của Bạn](#thêm-bot-vào-máy-chủ-của-bạn)
  - [Lệnh Discord](#lệnh-discord)
- [📱 Sử Dụng Telegram](#-sử-dụng-telegram)
  - [Thêm Bot Vào Nhóm Của Bạn](#thêm-bot-vào-nhóm-của-bạn)
  - [Lệnh Telegram](#lệnh-telegram)
- [⚙️ Quản Lý Trạng Thái](#️-quản-lý-trạng-thái)
- [❓ Câu Hỏi Thường Gặp](#-câu-hỏi-thường-gặp)
- [🛠️ Hỗ Trợ](#️-hỗ-trợ)

## 🚀 Về Dự Án

**Bot Đề Xuất Qubic** là một bot được phát triển đặc biệt cho cộng đồng Qubic, tự động phát hiện các đề xuất quản trị mới, tóm tắt chúng bằng AI bằng 13 ngôn ngữ khác nhau và xuất bản chúng trong các máy chủ Discord và nhóm Telegram.

### 🌟 Lợi Ích Chính

- **🔍 Phát Hiện Tự Động** - Giám sát liên tục các đề xuất Qubic mới
- **🌍 Khả Năng Truy Cập Đa Ngôn Ngữ** - Giúp đề xuất có sẵn cho các thành viên cộng đồng không nói tiếng Anh
- **🤖 Tóm Tắt Bằng AI** - Sử dụng DeepSeek AI để tạo tóm tắt chính xác, dễ hiểu
- **⏰ Thông Báo Kịp Thời** - Đăng đề xuất mới trong vòng 15 phút sau khi xuất bản
- **📊 Kết Quả Bỏ Phiếu** - Tự động xuất bản kết quả vào cuối mỗi kỷ nguyên

## 🏗️ Kiến Trúc & Công Nghệ

Bot dựa trên kiến trúc đa nền tảng mạnh mẽ:

### Thành Phần Cốt Lõi

- **Tích Hợp Qubic API** - Truy xuất các đề xuất đang hoạt động và đã hoàn thành
- **DeepSeek AI** - Tạo tóm tắt đa ngôn ngữ
- **Cầu Nối Discord & Telegram** - Phân phối đa nền tảng
- **Lưu Trữ Dựa Trên GitHub** - Quản lý trạng thái liên tục và lưu trữ đệm
- **Lưu Trữ Đệm Thông Minh** - Tránh các cuộc gọi API trùng lặp

## 📋 Ngôn Ngữ Được Hỗ Trợ

Bot hiện hỗ trợ **13 ngôn ngữ**:

| Ngôn Ngữ | Mã |
|----------|------|
| Tiếng Đức | `de` |
| Tiếng Anh | `en` |
| Tiếng Pháp | `fr` |
| Tiếng Tây Ban Nha | `es` |
| Tiếng Ý | `it` |
| Tiếng Bồ Đào Nha | `pt` |
| Tiếng Nga | `ru` |
| Tiếng Nhật | `ja` |
| Tiếng Trung | `zh` |
| Tiếng Hàn | `ko` |
| Tiếng Ả Rập | `ar` |
| Tiếng Thổ Nhĩ Kỳ | `tr` |
| Tiếng Việt | `vi` |

## 🎯 Tính Năng Chi Tiết

### 🤖 Phát Hiện Đề Xuất Tự Động
- **Khoảng Thời Gian 15 Phút** - Kiểm tra đề xuất mới thường xuyên
- **Xử Lý Theo Kỷ Nguyên** - Quản lý trạng thái riêng biệt cho mỗi kỷ nguyên
- **Phát Hiện Trùng Lặp** - Ngăn chặn thông báo nhiều lần

### 🧠 Tóm Tắt AI Thông Minh
- **Tóm Tắt Nhận Thức Ngữ Cảnh** - Trích xuất các điểm chính từ mỗi đề xuất
- **Định Dạng Theo Ngôn Ngữ Cụ Thể** - Điều chỉnh theo sắc thái văn hóa
- **Cơ Chế Lưu Trữ Đệm** - Tránh các cuộc gọi AI trùng lặp cho cùng một đề xuất

### 🔄 Quản Lý Trạng Thái Mạnh Mẽ
- **Trạng Thái Theo Máy Chủ/Cuộc Trò Chuyện** - Mỗi cộng đồng quản lý trạng thái riêng
- **Duy Trì GitHub** - Trạng thái tồn tại sau khi khởi động lại
- **Dọn Dẹp Tự Động** - Loại bỏ dữ liệu kỷ nguyên lỗi thời

### 🌐 Hỗ Trợ Đa Nền Tảng
- **Tích Hợp Discord Liền Mạch** - Lệnh gạch chéo và tin nhắn nhúng
- **Tối Ưu Hóa Telegram** - Bàn phím nội tuyến và hỗ trợ Markdown
- **Trải Nghiệm Nhất Quán** - Cùng tính năng trên cả hai nền tảng

## 💬 Sử Dụng Discord

### Thêm Bot Vào Máy Chủ Của Bạn
1. Sử dụng [**liên kết mời**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot)
2. Cấp **quyền quản trị viên** và thêm bot vào kênh mong muốn
3. Thực hiện **thiết lập** với `/setup`

### Lệnh Discord

| **Lệnh** | **Mô Tả** | **Tham Số** |
|-------------|-----------------|----------------|
| ❔ `/help` | Hiển thị trợ giúp | Trợ giúp và hướng dẫn chi tiết |
| ⚙️ `/setup` | Thiết lập bot cho máy chủ của bạn | • `channel`: Kênh cho tóm tắt đề xuất<br>• `language`: Ngôn ngữ cho các bản tóm tắt |
| ℹ️ `/info` | Hiển thị thông tin chi tiết về trạng thái bot | • Kênh và ngôn ngữ được cấu hình<br>• Kỷ nguyên hiện tại<br>• Số lượng đề xuất đang hoạt động<br>• Trạng thái DeepSeek API<br>• Thời gian hoạt động của bot<br>• Khoảng thời gian kiểm tra |

## 📱 Sử Dụng Telegram

### Thêm Bot Vào Nhóm Của Bạn
1. **Quản lý nhóm**
2. **Thêm thành viên**
3. **Tìm kiếm bot:** `@QubicTranslationBot`
4. **Thêm vào nhóm** với tư cách quản trị viên
5. **Thực hiện thiết lập** trong cuộc trò chuyện mong muốn với `/setup`

> [!IMPORTANT]
> Lệnh `/setup` <ins>**phải**</ins> được sử dụng trong cuộc trò chuyện nơi cần đăng tóm tắt.

### Lệnh Telegram

| **Lệnh** | **Mô Tả** | **Tham Số** |
|-------------|-----------------|----------------|
| ❔ `/start` hoặc `/help` | Hiển thị trợ giúp | Trợ giúp và hướng dẫn chi tiết |
| ⚙️ `/setup` | Mở bàn phím nội tuyến để chọn ngôn ngữ | • Bàn phím nội tuyến với các tùy chọn ngôn ngữ<br>• Chọn ngôn ngữ mong muốn |
| ℹ️ `/info` | Hiển thị thông tin chi tiết về trạng thái bot | • Cuộc trò chuyện và ngôn ngữ được cấu hình<br>• Kỷ nguyên hiện tại<br>• Số lượng đề xuất đang hoạt động<br>• Trạng thái DeepSeek API<br>• Thời gian hoạt động của bot<br>• Khoảng thời gian kiểm tra |

## ⚙️ Quản Lý Trạng Thái

Bot quản lý cho mỗi kỷ nguyên:

- **Đề Xuất Đã Xử Lý** - Tránh trùng lặp
- **Bộ Đếm Đề Xuất** - Đánh số liên tục cho mỗi kỷ nguyên
- **Trạng Thái Theo Ngôn Ngữ Cụ Thể** - Cho phép chuyển đổi ngôn ngữ mà không mất dữ liệu

## ❓ Câu Hỏi Thường Gặp

### 🤔 Câu Hỏi Chung

**H: Những ngôn ngữ nào được hỗ trợ?**  
Đ: Hiện tại 13 ngôn ngữ: Tiếng Đức, Tiếng Anh, Tiếng Pháp, Tiếng Tây Ban Nha, Tiếng Ý, Tiếng Bồ Đào Nha, Tiếng Nga, Tiếng Nhật, Tiếng Trung, Tiếng Hàn, Tiếng Ả Rập, Tiếng Thổ Nhĩ Kỳ, Tiếng Việt.

**H: Bản tóm tắt đề xuất có tính cập nhật như thế nào?**  
Đ: Các đề xuất mới được phát hiện và tóm tắt trong vòng 15 phút sau khi xuất bản.

**H: Tôi có thể thay đổi ngôn ngữ sau này không?**  
Đ: Có, chỉ cần sử dụng `/setup` lại. Các đề xuất đã xử lý sẽ được cung cấp bằng ngôn ngữ mới.

### 🔧 Câu Hỏi Kỹ Thuật

**H: Bot không phản hồi với lệnh - phải làm gì?**  
Đ: Đảm bảo bot có các quyền cần thiết và thử lại lệnh.

**H: Kết quả bỏ phiếu được thông báo như thế nào?**  
Đ: Mỗi thứ Tư lúc 12:15 UTC, kết quả của kỷ nguyên trước sẽ được tự động đăng.

### 🌐 Câu Hỏi Theo Nền Tảng Cụ Thể

**H: Tất cả lệnh có hoạt động trên cả hai nền tảng không?**  
Đ: Có, chức năng cốt lõi giống nhau trên Discord và Telegram.

**H: Tôi có thể sử dụng bot trên cả Discord và Telegram không?**  
Đ: Có, bạn có thể sử dụng bot trên cả hai nền tảng song song.

**H: Bot cần những quyền gì trên Discord?**  
Đ: Bot cần quyền gửi tin nhắn, nhúng liên kết và sử dụng lệnh gạch chéo.

## 🛠️ Hỗ Trợ

Đối với câu hỏi hoặc vấn đề với bot, vui lòng liên hệ:

**📞 Liên Hệ Discord/Telegram:** MDC

**⚠️ Quan Trọng:**  
Vui lòng đảm bảo bạn có sẵn thông tin sau:
- ID máy chủ/cuộc trò chuyện nơi xảy ra sự cố
- Lệnh chính xác không hoạt động
- Thời gian xảy ra sự cố
- Thông báo lỗi (nếu có)

---

<div align="center">

**🌍 Một Dự Án Cho Cộng Đồng Qubic**  
*Giúp mọi người có thể tiếp cận đề xuất bằng mọi ngôn ngữ*

</div>
