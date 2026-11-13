# AI Animation Studio

Website tĩnh tiếng Việt để lập storyboard video hoạt hình 3D CGI **không thoại**, 30 hoặc 60 giây, mỗi cảnh 10 giây.

## Chạy thử
Mở `index.html` trên trình duyệt. Để chạy qua local server: `python -m http.server 8000`, sau đó mở `http://localhost:8000`.

## Tính năng
- Tạo prompt theo nhịp hook → phát triển → twist, có thể chỉnh sửa từng cảnh.
- Tối đa 3 nhân vật từ thư viện, ảnh tham chiếu JPG/PNG/WebP tối đa 1 MB.
- Mẫu prompt, quản lý dự án/trạng thái, sao chép prompt, xuất TXT, sao lưu JSON.
- Khung hình 9:16, 1080×1920, 30 FPS; không thoại, không âm thanh meme.
- Responsive; không cần API key, framework hay máy chủ.

## Giới hạn
Đây là **bản MVP**: trình tạo prompt theo mẫu, **không gọi AI** và **không render video**. Ảnh tham chiếu được lưu cục bộ để người dùng quản lý, không được đính kèm tự động vào công cụ video bên ngoài. Dữ liệu lưu bằng `localStorage` trên thiết bị/trình duyệt hiện tại; xóa dữ liệu trình duyệt sẽ mất dự án. Nên sao lưu JSON định kỳ. Bản này chưa hỗ trợ nhập lại JSON.

## Đưa lên GitHub
1. Tạo repository mới (ví dụ `ai-animation-studio`) trên GitHub.
2. Tải 4 tệp `index.html`, `style.css`, `app.js`, `README.md` vào thư mục gốc của repository (Add file → Upload files → Commit changes).
3. Trong Settings → Pages, chọn **Deploy from a branch**, branch `main`, folder `/ (root)` và Save.
4. Chờ GitHub Pages xuất bản. URL thường có dạng `https://USERNAME.github.io/ai-animation-studio/`.

## Quyền riêng tư
Không tải ảnh nhạy cảm lên repository công khai. Dữ liệu dự án được lưu trên trình duyệt, không tự động gửi lên GitHub.
