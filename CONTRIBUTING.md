# Đóng góp cho Góc nhỏ

## Đọc sách

Website hiện trưng bày sách trên kệ tương tác. Xem [books/README.md](books/README.md) cho các trường `readingProgress`, `keepsakes`, `cover` và nguồn giới thiệu. Tiến độ và ghi nhớ chỉ thêm khi có dữ liệu thực tế của tác giả.

Thêm Markdown theo nhóm/ngôn ngữ như `books/vi/new-book.md`, `films/vi/new-film.md` hoặc `podcasts/vi/new-episode.md`.

```yaml
id: my-corner-new-book
title: Tên tác phẩm
description: Giới thiệu ngắn.
category: books
creator: Tác giả
shelfStatus: planned
status: draft
```

`category` nhận `books`, `films`, `podcasts`; trang Đọc sách chỉ lấy `books`. Các nhóm còn lại vẫn có thể lưu nội dung riêng theo manifest. `shelfStatus` nhận `planned`, `current`, `finished`. Phần dưới frontmatter là cảm nhận/ghi chép; không tự khẳng định một tác phẩm là sở thích của tác giả khi chưa được xác nhận. Ảnh và link nguồn là tùy chọn.

## Nhạc và lời

Dữ liệu ở `music/tracks.json`. Giữ ID bài nhạc đang có; bài mới cần ID riêng, tiêu đề, nghệ sĩ, bìa, `mood` và một nguồn: `youtubeId` hoặc `src`. `mood` nhận một trong các giá trị: `focus` (tập trung), `quiet` (thư giãn), `love` (tình yêu), `sad` (tâm trạng), `nostalgia` (hoài niệm), `energy` (năng lượng), `personal` (nhạc từ thiết bị). Bộ lọc chỉ hiển thị các nhóm đang có bài hát. Đường dẫn bìa/audio/lời tính từ file JSON này. LRC đặt tên theo bài hát trong `music/lyrics/`:

```text
[ti:Tên bài hát]
[ar:Nghệ sĩ]
[offset:0]

[00:03.50]Dòng lời được cung cấp
```

Chỉ góp nội dung và tư liệu có quyền chia sẻ. Timestamp cần khớp đúng bản thu; không tự tạo mốc đều theo độ dài video. Bổ sung nguồn/giấy phép khi phù hợp.

## Gửi thay đổi

1. Tạo nhánh hoặc fork, sửa đúng nội dung và ngôn ngữ liên quan.
2. Giữ ID/slug cũ khi sửa bài; giữ chung ID hoặc `translationKey` giữa các bản dịch.
3. Kiểm tra cú pháp, code/ví dụ và nguồn tham khảo. Chỉ dùng media có quyền sử dụng.
4. Giữ bài mới ở trạng thái draft để review. Ghi rõ nội dung và cách kiểm tra trong PR.

Không đưa credential, nội dung cá nhân chưa được phép công khai, dependencies hoặc cache vào PR. Các thiết lập vận hành do maintainer quản lý; không cần yêu cầu khóa cá nhân để gửi đóng góp.

## Hành trình, bạn bè và truyện

Các phần này cùng nằm trong repo `my-corner`, ngang cấp với `music/` và `books/`. Xem `README.md` để biết cây thư mục. Avatar nằm trong `friends/media/`, ảnh hành trình trong `journey/media/`, ảnh truyện trong `stories/<ten-truyen>/media/` hoặc `stories/media/` cho ảnh dùng chung. Không đặt `.git` hay workflow thông báo riêng trong các thư mục con; workflow ở gốc `my-corner` thông báo cập nhật cho cả repo.

`journey/module.json` và `stories/module.json` giữ ID cũ để bảo toàn URL và khóa truyện `stories/<ten-truyen>/<chuong>`. Không sửa ID khi chỉ thay đổi vị trí lưu trữ. Mật khẩu vẫn nằm trong cấu hình riêng của website, không ghi mật khẩu vào repo này.
