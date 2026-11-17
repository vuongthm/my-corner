# Đóng góp cho module hành trình

Mỗi dấu mốc nằm ở `vi/<milestone-id>.md`; bản dịch ở thư mục ngôn ngữ tương ứng. Sửa nội dung theo thông tin do tác giả cung cấp, không tự gán thành tích hoặc sự kiện chưa được xác nhận.

```yaml
id: journey-new-step
title: Tên dấu mốc
label: Nhãn ngắn
description: Giới thiệu ngắn.
status: draft
order: 100
```

Sau frontmatter là nội dung Markdown. `order` sắp thứ tự; khi xuất bản, trạng thái hiển thị được chọn từ `current`, `completed`, `planned`. Ảnh dùng đường dẫn tương đối và thông tin chú thích đúng nguồn.

Trang Hành trình hiện mở công khai và hiển thị các mốc dọc một đường SVG. `period` là nhãn thời gian; `year` có thể bổ sung khi biết năm chính xác. Để thêm ảnh, khai báo `photos` gồm `src`, `title`, `place`, hoặc dùng `photoSources` tham chiếu ảnh đã đăng ký trong hồ sơ website. Các trường `storySlug`, `entrySlugs`, `page` nối đến nội dung liên quan. Giữ ID mốc ổn định vì mỗi mốc có URL riêng.

## Gửi thay đổi

1. Tạo nhánh hoặc fork, sửa đúng nội dung và ngôn ngữ liên quan.
2. Giữ ID/slug cũ khi sửa bài; giữ chung ID hoặc `translationKey` giữa các bản dịch.
3. Kiểm tra cú pháp, code/ví dụ và nguồn tham khảo. Chỉ dùng media có quyền sử dụng.
4. Giữ bài mới ở trạng thái draft để review. Ghi rõ nội dung và cách kiểm tra trong PR.

Không đưa credential, nội dung cá nhân chưa được phép công khai, dependencies hoặc cache vào PR. Các thiết lập vận hành do maintainer quản lý; không cần yêu cầu khóa cá nhân để gửi đóng góp.

Trong workspace website, chạy `pnpm content:new milestone <id>` để tạo mốc trong `content/my-corner/journey/vi/`. Ảnh riêng đặt ở `media/` và dùng đường dẫn `../media/anh.webp` từ bài. Cấu hình khóa trang chung ở `page.md`. Push repo **my-corner**, không cần repo journey riêng.
