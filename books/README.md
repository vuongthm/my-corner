# Kệ sách

Ba mục hiện có: `the-little-prince`, `ngay-xua-co-mot-chuyen-tinh`, `toi-thay-hoa-vang-tren-co-xanh`.

Mỗi cuốn có bản `vi` và `en`, dùng chung `id`, `order`, `cover`, `source`. Nội dung giới thiệu đối chiếu với trang chính thức của tác phẩm hoặc Nhà xuất bản Trẻ. Bìa SVG là thiết kế trình bày riêng của website, không đại diện cho một ấn bản cụ thể.

## Tiến độ và giấy ghi nhớ

Thêm `readingProgress` (phần trăm từ 0 đến 100) khi có tiến độ đọc thực tế. Thêm `keepsakes` là danh sách ghi chú ngắn trong từng bản ngôn ngữ. Hai trường đều tùy chọn; giao diện chỉ hiển thị khi có dữ liệu. Những cuốn hiện có không gán sẵn lịch sử đọc hay trích dẫn cá nhân.

```json
{
  "readingProgress": 38,
  "keepsakes": ["Một điều bạn muốn giữ lại sau khi đọc."]
}
```

Trang đọc sách được mở công khai qua `site/shelf.md` của website. Sách riêng vẫn có thể dùng `lock: true` và mật khẩu theo hướng dẫn `CONTENT.md`.
