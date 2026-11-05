# Đóng góp cho Góc nhỏ

## Sách, phim và podcast

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

`category` nhận `books`, `films`, `podcasts`; `shelfStatus` nhận `planned`, `current`, `finished`. Phần dưới frontmatter là cảm nhận/ghi chép; không tự khẳng định một tác phẩm là sở thích của tác giả khi chưa được xác nhận. Ảnh và link nguồn là tùy chọn.

## Nhạc và lời

Dữ liệu ở `music/tracks.json`. Giữ ID bài nhạc đang có; bài mới cần ID riêng, tiêu đề, nghệ sĩ, bìa, `mood` (`focus`, `quiet`, `personal`) và một nguồn: `youtubeId` hoặc `src`. Đường dẫn bìa/audio/lời tính từ file JSON này. LRC đặt tên theo bài hát trong `music/lyrics/`:

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
