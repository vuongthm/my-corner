# Đóng góp truyện và bản dịch

Mỗi truyện có thư mục riêng, ví dụ `new-story/vi/series.md`, các chương `chapter-1.md`, `chapter-2.md` và thư mục `new-story/media/`. Bản dịch giữ cấu trúc tương ứng trong `en/` hoặc ngôn ngữ được hỗ trợ.

`series.md` chứa frontmatter tiêu đề, mô tả, ngày và ảnh bìa. Chương có frontmatter riêng:

```yaml
title: Tên chương
date: 2026-01-01
part: 1
status: draft
```

Sau frontmatter là nội dung Markdown. Gallery công khai của truyện có thể khai báo bằng `gallery` với `src`, `title`, `place`; đường dẫn ảnh tính từ file Markdown. Chỉ bổ sung câu chuyện, ảnh và chi tiết cá nhân đã được tác giả đồng ý. Không sửa cài đặt truy cập của nội dung riêng trong một PR biên tập.

## Gửi thay đổi

1. Tạo nhánh hoặc fork, sửa đúng nội dung và ngôn ngữ liên quan.
2. Giữ ID/slug cũ khi sửa bài; giữ chung ID hoặc `translationKey` giữa các bản dịch.
3. Kiểm tra cú pháp, code/ví dụ và nguồn tham khảo. Chỉ dùng media có quyền sử dụng.
4. Giữ bài mới ở trạng thái draft để review. Ghi rõ nội dung và cách kiểm tra trong PR.

Không đưa credential, nội dung cá nhân chưa được phép công khai, dependencies hoặc cache vào PR. Các thiết lập vận hành do maintainer quản lý; không cần yêu cầu khóa cá nhân để gửi đóng góp.

Phần này nằm trong `my-corner/stories/`. Push repo **my-corner** để cập nhật; không cần repo stories riêng. Khóa mật khẩu chương tiếp tục dùng `stories/<ten-truyen>/<ten-file>`.
