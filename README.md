# Portfolio Lê Ngọc Khánh

Website portfolio cá nhân tĩnh được xây dựng bằng HTML, CSS và JavaScript thuần cho môn Nhập môn Công nghệ số và Ứng dụng AI.

## Cách mở website

Mở trực tiếp file `index.html` bằng trình duyệt. Website không cần chạy server và không yêu cầu framework.

## Cách thay ảnh cá nhân

Thay file ảnh tại:

```text
assets/images/avatar-khanh.jpg
```

Giữ nguyên tên file `avatar-khanh.jpg` để website tự nhận ảnh mới.

## Cách thêm hoặc thay ảnh nền hero

Đặt ảnh nền đầu trang tại:

```text
assets/images/hero-bg.png
```

Hero đang dùng file này làm ảnh nền, kết hợp overlay tối để chữ dễ đọc. Nếu muốn thay ảnh, chỉ cần thay file `hero-bg.png` và giữ nguyên tên file.

## Cách thay PDF minh chứng

Thay các file PDF trong thư mục:

```text
assets/docs/
```

Giữ nguyên tên file:

```text
bai1.pdf
bai2.pdf
bai3.pdf
bai4.pdf
bai5.pdf
bai6.pdf
```

Mỗi PDF được nhúng trực tiếp trong phần bài học tương ứng ở website.

## Cách chỉnh sửa nội dung cá nhân

Mở file `index.html` và tìm các section theo `id`:

```text
#about       Giới thiệu bản thân
#skills      Năng lực
#projects    Dự án học tập
#summary     Tổng kết và tự đánh giá
#lien-he     Gửi lời nhắn
```

Chỉnh sửa văn bản trực tiếp trong các section tương ứng.

## Form liên hệ

Form trong section `#lien-he` hiện là form tĩnh. Khi người dùng bấm `Gửi lời nhắn`, JavaScript sẽ chặn reload trang, hiển thị thông báo cảm ơn và xóa nội dung form.

Form chưa kết nối backend, chưa gửi email thật và chưa lưu dữ liệu lên server.

## Cách đổi tone màu

Mở file `style.css` và chỉnh các biến trong phần `:root`:

```css
--bg-main: #020617;
--bg-soft: #0f172a;
--accent-blue: #38bdf8;
--accent-cyan: #22d3ee;
--accent-indigo: #818cf8;
--accent-emerald: #34d399;
--text-main: #f8fafc;
--text-muted: #94a3b8;
```

## Cách deploy website

### GitHub Pages

1. Tạo repository trên GitHub.
2. Đẩy toàn bộ thư mục project lên repository.
3. Vào `Settings` -> `Pages`.
4. Chọn branch chứa code, thường là `main`.
5. Chọn thư mục gốc `/root`, sau đó lưu lại.

### Netlify

1. Đăng nhập Netlify.
2. Chọn `Add new site` -> `Deploy manually`.
3. Kéo thả toàn bộ thư mục project lên Netlify.
4. Netlify sẽ tạo link public cho website.

## Cấu trúc thư mục

```text
portfolio-khanh/
├── index.html
├── style.css
├── script.js
├── README.md
└── assets/
    ├── images/
    │   ├── avatar-khanh.jpg
    │   └── hero-bg.png
    └── docs/
        ├── bai1.pdf
        ├── bai2.pdf
        ├── bai3.pdf
        ├── bai4.pdf
        ├── bai5.pdf
        └── bai6.pdf
```

## Lưu ý

Nếu trình duyệt không hiển thị PDF trực tiếp, người xem có thể dùng nút `Xem file PDF` hoặc `Tải xuống` trong từng bài học.
