# My-CV — Portfolio cá nhân

> Trang web CV/portfolio tĩnh dành cho Frontend Developer, được xây dựng bằng HTML5 và CSS3.

## 1. Tên dự án

**My-CV — Portfolio Cá Nhân**

Trang web hiện được thiết kế theo ngôn ngữ tiếng Việt, có bố cục responsive và tối ưu cho điện thoại, máy tính bảng và máy tính để bàn.

## 2. Mô tả dự án

`My-CV` là trang portfolio cá nhân dùng để giới thiệu thông tin cá nhân, vai trò nghề nghiệp, kỹ năng, dự án tiêu biểu và phương thức liên hệ. Dự án là một trang web tĩnh, không yêu cầu cơ sở dữ liệu hay backend.

Mục tiêu:

- Trình bày hồ sơ Frontend Developer một cách chuyên nghiệp.
- Giới thiệu kỹ năng và dự án tiêu biểu.
- Cung cấp giao diện dễ đọc, dễ truy cập và thân thiện trên mọi thiết bị.
- Có mã nguồn đơn giản để tùy chỉnh và triển khai nhanh.

## 3. Chức năng chính

- Header, thương hiệu cá nhân và thanh điều hướng sticky.
- Phần giới thiệu Hero với tên, vai trò, mô tả và ảnh đại diện.
- Danh sách kỹ năng bằng các thẻ (chips).
- Danh sách dự án dạng card sử dụng CSS Grid.
- Phần liên hệ bằng Email, GitHub và LinkedIn.
- Menu điều hướng cuộn mượt đến từng section.
- Nút quay về đầu trang.
- Bố cục mobile-first, hỗ trợ Flexbox và CSS Grid.
- Tránh tràn ngang trên màn hình nhỏ.

## 4. Công nghệ sử dụng

| Thành phần | Công nghệ |
|---|---|
| Ngôn ngữ đánh dấu | HTML5 |
| Giao diện | CSS3 |
| Bố cục | Flexbox, CSS Grid |
| Responsive | CSS Media Queries, Mobile-first |
| Mã nguồn | Git và GitHub |
| Máy chủ tĩnh thử nghiệm | Python HTTP Server, Live Server hoặc Nginx |
| Chạy bằng container | Docker |

Dự án hiện không sử dụng framework JavaScript, package manager hay cơ sở dữ liệu.

## 5. Cấu trúc thư mục

```text
My-CV/
├── index.html
├── README.md
├── BAOCAO-A2.1.docx
└── assets/
    ├── css/
    │   └── styles.css
    └── img/
        └── avatar.jpg
```

## 6. Yêu cầu môi trường

### Chạy trực tiếp

- Trình duyệt hiện đại: Chrome, Edge, Firefox hoặc Safari.
- Không bắt buộc Node.js, cơ sở dữ liệu hoặc biến môi trường.

### Làm việc với mã nguồn

- Git 2.x trở lên.
- Visual Studio Code hoặc trình soạn thảo khác.
- Python 3.x nếu muốn dùng máy chủ HTTP cục bộ.

### Docker

- Windows/macOS: Docker Desktop.
- Linux: Docker Engine.

## 7. Cài đặt

### Windows

```powershell
# Kiểm tra Git
git --version

# Clone dự án
git clone https://github.com/daitv-dnu/My-CV.git
cd My-CV

# Mở trực tiếp bằng trình duyệt mặc định
Start-Process .\index.html
```

Nếu chưa có Git, chọn **Code > Download ZIP** trên GitHub, giải nén và mở thư mục.

### macOS

```bash
# Kiểm tra Git
git --version

# Clone dự án
git clone https://github.com/daitv-dnu/My-CV.git
cd My-CV

# Mở trang
open index.html
```

### Linux

```bash
# Kiểm tra Git
git --version

# Clone dự án
git clone https://github.com/daitv-dnu/My-CV.git
cd My-CV

# Mở trang trên desktop Linux
xdg-open index.html
```

## 8. Cấu hình

Nội dung trang nằm trong `index.html`, còn giao diện nằm trong `assets/css/styles.css`.

Các biến CSS chính được đặt trong phần `:root`:

```css
:root {
  --color-primary: #2563eb;
  --color-primary-dark: #1d4ed8;
  --color-accent: #7c3aed;
  --color-text: #1e293b;
  --color-text-soft: #64748b;
  --color-bg: #ffffff;
  --color-surface: #f8fafc;
  --container-max: 1200px;
}
```

Các tùy chỉnh thường dùng:

- Thay nội dung trong `index.html`.
- Thay màu, phông chữ và khoảng cách trong `assets/css/styles.css`.
- Thay ảnh đại diện tại `assets/img/avatar.jpg`.
- Thay email bằng cách cập nhật giá trị `mailto:` trong phần Liên hệ.
- Thay GitHub và LinkedIn bằng URL thật trong phần Liên hệ.
- Kiểm tra tên, vai trò và mô tả ở phần Hero trong `index.html`.

## 9. Chạy thử

### Cách 1: Mở trực tiếp

Mở `index.html` bằng trình duyệt. Đây là cách đơn giản nhất để xem trang.

### Cách 2: Chạy bằng Python trên Windows

```powershell
cd D:\duong-dan\My-CV
py -m http.server 8080
```

### Cách 2: Chạy bằng Python trên macOS

```bash
cd /duong-dan/My-CV
python3 -m http.server 8080
```

### Cách 2: Chạy bằng Python trên Linux

```bash
cd /duong-dan/My-CV
python3 -m http.server 8080
```

Sau đó truy cập:

```text
http://localhost:8080
```

Nhấn `Ctrl+C` để dừng máy chủ.

### Cách 3: Chạy bằng VS Code Live Server

1. Mở thư mục dự án bằng VS Code.
2. Cài extension **Live Server**.
3. Nhấp chuột phải vào `index.html`.
4. Chọn **Open with Live Server**.
5. Truy cập địa chỉ do extension cung cấp, thường là `http://127.0.0.1:5500`.

## 10. Chạy bằng Docker

### Dùng Docker/Nginx trực tiếp trên macOS hoặc Linux

```bash
cd /duong-dan/My-CV
docker run --rm -d \
  --name my-cv \
  -p 8080:80 \
  -v "$(pwd):/usr/share/nginx/html:ro" \
  nginx:alpine
```

### Dùng Docker/Nginx trên Windows PowerShell

```powershell
cd D:\duong-dan\My-CV
docker run --rm -d --name my-cv -p 8080:80 `
  -v "${PWD}:/usr/share/nginx/html:ro" `
  nginx:alpine
```

### Dùng Docker/Nginx trên Windows Command Prompt

```bat
cd /d D:\duong-dan\My-CV
docker run --rm -d --name my-cv -p 8080:80 -v "%cd%:/usr/share/nginx/html:ro" nginx:alpine
```

Sau đó truy cập `http://localhost:8080`.

Kiểm tra và dừng container:

```bash
docker ps
docker logs my-cv
docker stop my-cv
```

### Tạo Dockerfile tùy chọn

Tạo tệp `Dockerfile` tại thư mục gốc:

```dockerfile
FROM nginx:alpine
COPY index.html /usr/share/nginx/html/index.html
COPY assets /usr/share/nginx/html/assets
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Build và chạy:

```bash
docker build -t my-cv:latest .
docker run --rm -d --name my-cv -p 8080:80 my-cv:latest
```

## 11. Kiểm tra trước khi hoàn tất

- Trang tải không có lỗi tài nguyên trong tab Network.
- Header, Hero, kỹ năng, dự án và liên hệ hiển thị đầy đủ.
- Thanh điều hướng cuộn đúng đến từng section.
- Ảnh đại diện hiển thị đúng.
- Bố cục không bị tràn ngang trên mobile.
- Email, GitHub và LinkedIn đã thay bằng thông tin thật.

## 12. Triển khai tĩnh

Vì đây là trang web tĩnh, có thể triển khai bằng GitHub Pages, Cloudflare Pages, Netlify hoặc một hosting HTTP tĩnh:

- Build command: không cần.
- Publish/output directory: thư mục gốc hoặc `.`, tùy nhà cung cấp.
- Entry file: `index.html`.

## 13. Thông tin liên hệ

Các thông tin hiện trong trang là dữ liệu mẫu và cần được thay trước khi công khai:

- Email: `an.nguyen@example.com`
- GitHub: `github.com/nguyenvanan`
- LinkedIn: `linkedin.com/in/nguyenvanan`

Repository:

- GitHub Repository: https://github.com/daitv-dnu/My-CV
- GitHub cá nhân: https://github.com/daitv-dnu

## 14. Đóng góp

1. Fork repository.
2. Tạo nhánh mới:

   ```bash
   git checkout -b feature/ten-tinh-nang
   ```

3. Commit thay đổi:

   ```bash
   git commit -m "Cập nhật portfolio cá nhân"
   ```

4. Push nhánh và tạo Pull Request:

   ```bash
   git push origin feature/ten-tinh-nang
   ```

## 15. Giấy phép

Chưa cấu hình tệp giấy phép cụ thể cho dự án. Dự án được sử dụng cho mục đích học tập và cá nhân; cần xin phép chủ dự án trước khi sử dụng lại hoặc phân phối ngoài mục đích cá nhân/học tập.
