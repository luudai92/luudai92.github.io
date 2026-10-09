# luudai92.github.io

Trang cá nhân của **Lưu Văn Đại**, AI-Augmented Software Engineer.

🌐 **Live:** https://luudai92.github.io

## Giới thiệu

Website portfolio một trang (single page), giới thiệu năng lực xây dựng hệ thống dữ liệu, Data Warehouse, ERP và giải pháp ứng dụng AI với C#, ASP.NET Core, SQL Server.

## Tính năng

- Một trang tĩnh, tải nhanh, không cần bước build.
- Hiệu ứng nền 3D bằng [three.js](https://threejs.org/) r128 (nạp từ cdnjs).
- Song ngữ Việt / Anh, tự chọn theo ngôn ngữ trình duyệt và ghi nhớ lựa chọn bằng `localStorage`.
- Giao diện tối, responsive, hỗ trợ safe-area trên thiết bị di động.
- SEO: meta description, Open Graph (`assets/og.jpg`), JSON-LD `Person`.

## Các mục trên trang

| Mục | Anchor |
| --- | --- |
| Hero | `#top` |
| Giới thiệu | `#about` |
| Năng lực | `#capabilities` |
| Quy trình làm việc có AI | `#workflow` |
| Công nghệ | `#stack` |
| Nguyên tắc | `#principles` |
| Liên hệ | `#contact` |

## Cấu trúc thư mục

```
.
├── index.html        # Toàn bộ HTML, CSS, JS của trang
├── assets/
│   ├── avatar.jpg    # Ảnh chân dung (720x900)
│   ├── avatar-sm.jpg # Ảnh đại diện nhỏ cho thanh điều hướng (160x160)
│   └── og.jpg        # Ảnh xem trước khi chia sẻ link (1200x928)
├── .nojekyll         # Tắt Jekyll, GitHub Pages phục vụ file nguyên trạng
└── README.md
```

> Các ảnh trong `assets/` phải được commit cùng `index.html`, nếu thiếu thì ảnh trên site sẽ báo 404.

## Chạy cục bộ

Không cần cài đặt gì. Mở trực tiếp `index.html` bằng trình duyệt, hoặc chạy một server tĩnh:

```bash
python -m http.server 8000
# truy cập http://localhost:8000
```

Cần có kết nối Internet để nạp font (Google Fonts) và three.js (cdnjs).

## Triển khai

Site được phục vụ bằng GitHub Pages từ nhánh `main`, thư mục gốc (`/`).

```bash
git add -A
git commit -m "Update site"
git push origin main
```

Sau khi push, GitHub Pages thường cập nhật trong vòng 1 đến 2 phút.

## Công nghệ

HTML5, CSS3, JavaScript thuần, three.js r128, Google Fonts (Be Vietnam Pro, JetBrains Mono).

## Liên hệ

GitHub: [@luudai92](https://github.com/luudai92)
