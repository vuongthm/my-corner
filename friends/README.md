# Bạn bè và avatar

Sửa `friends.json`, đặt ảnh trong `media/` rồi push repo **my-corner**. Không sửa dữ liệu sinh tự động trong website.

Một bản ghi gồm `id` duy nhất, `name`, `alias`, `initials`, `website` (HTTP/HTTPS), `topics`, `description` (vi/en/ja/zh), và `avatar` nếu có. Ví dụ đường dẫn ảnh: `"avatar": "media/ten-ban.webp"`. `avatarSource` là đường dẫn nguồn ảnh để ghi nhận xuất xứ; trình duyệt dùng bản local trong `media/`.

Các lĩnh vực trùng nhau tạo ra đường kết nối. Chọn một người để đưa vào trung tâm và xem các kết nối chung; chọn lại người ở giữa để trở về toàn cảnh. Có thể kéo các nút, chúng sẽ tránh nhau và ổn định trở lại sau khi thả.

Không có avatar thì dùng chữ viết tắt. `websitePlaceholder: true` giữ bản ghi trong nguồn và chưa đưa ra danh bạ công khai; đặt thành `false` hoặc bỏ thuộc tính khi đã có website thật. `status: draft` hoặc `visibility: private` loại bản ghi khỏi dữ liệu xuất bản.
