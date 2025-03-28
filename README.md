# Hệ Thống Quản Lý Sự Kiện HUTECH

Một hệ thống quản lý sự kiện toàn diện cho Trường Đại học HUTECH giúp quản lý sự kiện, tham gia của sinh viên, tạo chứng nhận và báo cáo điểm danh.

## 📋 Tính Năng

- **Quản Lý Sự Kiện**: Tạo, cập nhật và xóa sự kiện
- **Quản Lý Sinh Viên**: Theo dõi thông tin và sự tham gia của sinh viên
- **Quản Lý Ban Cán Sự**: Quản lý ban cán sự lớp
- **Tạo Chứng Nhận**: Tạo và tùy chỉnh chứng nhận cho người tham gia
- **Báo Cáo**: Tạo báo cáo về sự tham gia của sinh viên, hoạt động của ban cán sự và điểm danh lớp học
- **Xác Thực Người Dùng**: Kiểm soát truy cập dựa trên vai trò

## 🔧 Công Nghệ

### Backend
- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT Authentication
- Bcrypt
- Nodemailer
- Node-schedule

### Frontend
- React (v18.3.1)
- Vite
- React Router DOM (v7.0.2)
- TailwindCSS
- Axios
- Day.js
- HTML-to-Image
- React Export Table to Excel

## 🚀 Cài Đặt

### Yêu Cầu Hệ Thống
- Node.js (v16 trở lên)
- MongoDB

### Cài Đặt Backend
1. Sao chép kho lưu trữ
   ```bash
   git clone https://github.com/yourusername/hutech-event-backend.git
   cd hutech-event-backend
   ```

2. Cài đặt các gói phụ thuộc
   ```bash
   npm install
   ```

3. Tạo file `.env` trong thư mục gốc với các biến sau:
   ```
   PORT=3000
   MONGODB_URI=mongodb://localhost:27017/hutech-event
   JWT_SECRET=your_jwt_secret
   ```

4. Khởi động máy chủ backend
   ```bash
   npm run dev
   ```

### Cài Đặt Frontend
1. Di chuyển đến thư mục frontend
   ```bash
   cd hutech-event-frontend
   ```

2. Cài đặt các gói phụ thuộc
   ```bash
   npm install
   ```

3. Khởi động máy chủ phát triển frontend
   ```bash
   npm run dev
   ```

## 📱 Sử Dụng

### Truy Cập Ứng Dụng
- API Backend: http://localhost:3000
- Frontend: http://localhost:5173

### Vai Trò Người Dùng
1. **Admin**: Quyền truy cập đầy đủ vào tất cả tính năng
2. **Cộng Tác Viên**: Quản lý sự kiện, chứng nhận và báo cáo

### Tính Năng Chính
- **Sự Kiện**: Tạo và quản lý sự kiện với chi tiết như tên, ngày, địa điểm, v.v.
- **Sinh Viên**: Theo dõi sự tham gia của sinh viên và tạo chứng nhận
- **Báo Cáo**: Xem và xuất báo cáo về điểm danh và sự tham gia của sinh viên
- **Chứng Nhận**: Tạo chứng nhận tùy chỉnh cho người tham gia sự kiện

## 🗂️ Cấu Trúc Dự Án

### Backend
```markdown
hutech-event-backend/
├── index.js         # Điểm khởi đầu
├── models/          # Các mô hình MongoDB
├── controllers/     # Xử lý yêu cầu
├── routes/          # Các route API
├── middlewares/     # Middleware Express
└── services/        # Logic nghiệp vụ
```

### Frontend
```markdown
hutech-event-frontend/
├── src/
│   ├── assets/      # Tài nguyên tĩnh
│   ├── components/  # Các component tái sử dụng
│   ├── pages/       # Các component trang
│   ├── services/    # Các cuộc gọi dịch vụ API
│   ├── App.jsx      # Component ứng dụng chính
│   └── main.jsx     # Điểm khởi đầu
└── index.html       # Template HTML
```

## 🔑 Các Endpoint API

### Xác Thực
- `POST /api/auth/login` - Đăng nhập người dùng
- `POST /api/auth/register` - Đăng ký người dùng (Chỉ Admin)

### Sự Kiện
- `GET /api/events` - Lấy tất cả sự kiện
- `GET /api/events/:id` - Lấy sự kiện theo ID
- `POST /api/events` - Tạo sự kiện mới
- `PUT /api/events/:id` - Cập nhật sự kiện
- `DELETE /api/events/:id` - Xóa sự kiện

### Sinh Viên
- `GET /api/students` - Lấy tất cả sinh viên
- `POST /api/students` - Tạo sinh viên mới
- `PUT /api/students/:id` - Cập nhật sinh viên
- `DELETE /api/students/:id` - Xóa sinh viên

### Chứng Nhận
- `GET /api/certificates` - Lấy tất cả chứng nhận
- `POST /api/certificates` - Tạo chứng nhận
- `GET /api/cef-templates` - Lấy mẫu chứng nhận

## 🤝 Đóng Góp

1. Fork repository
2. Tạo nhánh tính năng (`git checkout -b feature/amazing-feature`)
3. Commit thay đổi của bạn (`git commit -m 'Add some amazing feature'`)
4. Push đến nhánh (`git push origin feature/amazing-feature`)
5. Mở một Pull Request

## 📜 Giấy Phép

Dự án này được cấp phép theo Giấy phép MIT - xem file LICENSE để biết chi tiết.

## 👥 Thành Viên

Phạm Trung Nam

Nguyễn Trung Kiên


