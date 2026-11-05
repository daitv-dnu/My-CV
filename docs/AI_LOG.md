# Nhật ký thay đổi AI

## 2026-11-05 15:51

- **Tác nhân:** GitHub Copilot
- **Nhiệm vụ:** Viết tài liệu release note cho phiên bản v1.0.0.
- **Thay đổi lớn:**
  - Tạo [RELEASENOTE.md](RELEASENOTE.md) với phiên bản, ngày phát hành, chức năng mới, lỗi đã sửa và hạn chế còn tồn tại.
- **Kết quả kiểm tra:** Đã xem lại nội dung file; workspace không có bộ kiểm thử tự động nên không chạy test.
- **Trạng thái:** Hoàn thành

## 2026-11-05 15:57

- **Tác nhân:** GitHub Copilot
- **Nhiệm vụ:** Soạn báo cáo kiểm thử sản phẩm theo đúng 6 nhóm tiêu chí.
- **Thay đổi lớn:**
  - Tạo [test_report.md](test_report.md) với thông tin chung, bảng tổng quan, checklist chi tiết từng tiêu chí, đánh giá bàn giao, đề xuất khắc phục và bảng ký duyệt.
  - Phân biệt các trạng thái Đạt, Chưa đạt và Cần cải thiện dựa trên bằng chứng có thể xác minh trong repository.
- **Kết quả kiểm tra:** Đã kiểm tra cấu trúc nội dung và xác nhận workspace không có bộ kiểm thử tự động; chưa thực hiện kiểm thử trên trình duyệt.
- **Trạng thái:** Hoàn thành

## 2026-11-05 16:02

- **Tác nhân:** GitHub Copilot
- **Nhiệm vụ:** Tạo minh chứng kiểm thử giao diện responsive.
- **Thay đổi lớn:**
  - Chụp trang `index.html` ở kích thước mobile 390 x 844, tablet 768 x 1024 và desktop 1440 x 900.
  - Lưu các ảnh minh chứng vào `docs/screenshots/mobile.png`, `docs/screenshots/tablet.png` và `docs/screenshots/desktop.png`.
  - Cập nhật phần tiêu chí responsive trong [test_report.md](test_report.md) và nhúng ba ảnh minh chứng vào báo cáo.
- **Kết quả kiểm tra:** Ba ảnh đã tồn tại trong thư mục minh chứng; đánh giá responsive được cập nhật dựa trên quan sát trực tiếp giao diện.
- **Trạng thái:** Hoàn thành

## Mẫu ghi nhật ký cho thay đổi lớn tiếp theo

```text
## YYYY-MM-DD HH:mm

- **Tác nhân:** <Tên công cụ hoặc tác nhân AI>
- **Nhiệm vụ:** <Mô tả ngắn mục tiêu thực hiện>
- **Thay đổi lớn:**
  - <Danh sách thay đổi quan trọng>
- **Kết quả kiểm tra:** <Kiểm tra đã thực hiện hoặc lý do không thể kiểm tra>
- **Trạng thái:** Hoàn thành | Bị chặn
```