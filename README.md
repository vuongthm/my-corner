# Góc nhỏ

Nguồn nội dung của Âm nhạc, Đọc sách, Hành trình, Bạn bè và Chuyện kể. Chỉ cần push repo `my-corner` để cập nhật các phần này.

```text
my-corner/
  module.json
  music/                  # tracks.json, covers/, lyrics/
  books/{vi,en,media}/
  films/{vi,en,media}/
  podcasts/{vi,en,media}/
  journey/
    module.json           # adapter journey, giữ ID và URL cũ
    page.md               # lock: false để mở trang hành trình
    vi/, en/, media/
  friends/
    friends.json
    media/                # avatar, đường dẫn trong JSON: media/ten-ban.webp
  stories/
    module.json           # adapter stories, giữ ID và khóa mật khẩu cũ
    media/                # ảnh dùng chung
    ten-truyen/{vi,en,media}/
```

Manifest gốc khai báo `collections: [journey, stories]` và `friends: friends/friends.json`. Website đọc từng bộ sưu tập bằng adapter riêng; bài truyện và mốc hành trình không bị trộn vào kệ sách. Các URL `/journey/`, `/stories/` và `/friends/` giữ nguyên.

- [Thêm bạn bè và avatar](friends/README.md).
- [Viết các mốc hành trình](journey/CONTRIBUTING.md).
- [Viết truyện và chương](stories/CONTRIBUTING.md).
- [Kệ sách, tiến độ và giấy ghi nhớ](books/README.md).
- [Nhạc và lời](CONTRIBUTING.md).

Trang Đọc sách chỉ hiển thị `books/`. Phim và podcast vẫn là nguồn nội dung được giữ riêng.

Nguồn gốc của chương truyện có khóa cũng nằm trong `my-corner`. Nếu muốn giữ bản gốc riêng tư, giữ repo `my-corner` private và cấp quyền đọc repo này cho secret `CONTENT_SOURCE_TOKEN` của website. Workflow không checkout `vuongthm/stories` hay dùng `STORIES_SOURCE_KEY` nữa; mật khẩu chương trong `CONTENT_PASSWORDS` giữ nguyên.
