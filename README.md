# 💚 Sổ Thu Chi

Ứng dụng quản lý tài chính cá nhân — **không quảng cáo, không thu thập dữ liệu, hoàn toàn miễn phí**. Toàn bộ dữ liệu thu chi được lưu ngay trên thiết bị của bạn, không gửi đi bất cứ đâu.

Ứng dụng chạy dưới dạng PWA (Progressive Web App): cài được ra màn hình chính như app thật và **hoạt động cả khi không có mạng**.

## ✨ Tính năng

- **Sổ giao dịch** — ghi các khoản thu, chi theo danh mục (ăn uống, nhà ở, y tế, công việc, BHXH, đầu tư...), kèm ghi chú và ngày. Chạm vào giao dịch để sửa hoặc xóa. Xem theo từng tháng.
- **Ngân sách 50/30/20** — chia thu nhập thành 3 nhóm: Thiết yếu, Cá nhân, Tiết kiệm & đầu tư. Tỷ lệ phần trăm và thu nhập dự kiến chỉnh được tùy ý. Thanh đo chuyển màu đỏ khi chi vượt hạn mức.
- **Biểu đồ** — chi tiêu trong tháng theo từng danh mục, và tổng kết thu – chi – còn lại của toàn bộ thời gian sử dụng.
- **Sao lưu & khôi phục** — xuất file sao lưu `.json`, khôi phục khi đổi máy, xuất bảng tính `.csv` mở được bằng Excel.

## 📲 Cách cài lên điện thoại

1. Mở địa chỉ app bằng trình duyệt Chrome (địa chỉ dạng `https://<tên-người-dùng>.github.io/sothuchi/`)
2. Bấm menu **⋮** → chọn **"Thêm vào Màn hình chính"** (hoặc "Cài đặt ứng dụng")
3. Mở app từ icon ngoài màn hình chính. Sau lần mở đầu tiên, app dùng được cả khi không có mạng.

## 🔄 Cách cập nhật app

1. Vào kho GitHub → **Add file → Upload files** → tải file mới lên đè file cũ → **Commit changes**
2. Chờ 1–2 phút, sau đó **đóng hẳn app và mở lại 2 lần** để bản mới được nạp (lần mở đầu app âm thầm tải bản mới, lần mở sau bản mới hiện ra)

Việc cập nhật **không ảnh hưởng** đến dữ liệu giao dịch đã nhập.

## 💾 Dữ liệu & quyền riêng tư

- Dữ liệu lưu trong bộ nhớ trình duyệt (localStorage) **trên thiết bị của bạn** — kho GitHub này chỉ chứa "vỏ" ứng dụng, không chứa bất kỳ giao dịch nào.
- Nếu xóa dữ liệu trình duyệt hoặc gỡ app, dữ liệu sẽ mất. Vì vậy hãy vào tab **Dữ liệu → Tải file sao lưu (.json)** định kỳ (ví dụ cuối mỗi tháng) và cất file ở nơi an toàn.
- Khi đổi điện thoại: cài app trên máy mới → tab Dữ liệu → **Khôi phục từ file sao lưu**.

## 🛠 Kỹ thuật

| Thành phần | Mô tả |
|---|---|
| `index.html` | Toàn bộ ứng dụng (HTML + CSS + JavaScript thuần, không dùng thư viện ngoài) |
| `sw.js` | Service worker — lưu đệm app để chạy offline |
| `manifest.webmanifest` | Khai báo PWA để cài ra màn hình chính |
| `icon-192.png`, `icon-512.png` | Biểu tượng ứng dụng |

Không máy chủ, không cơ sở dữ liệu, không theo dõi người dùng, không phụ thuộc dịch vụ bên thứ ba nào ngoài GitHub Pages để phát hành.

## 📄 Giấy phép

Dự án cá nhân, tự do sử dụng và chỉnh sửa cho nhu cầu của bạn.

---

*Ứng dụng được xây dựng với sự hỗ trợ của Claude (Anthropic).*
