🚀 Nền Tảng Quản Lý Công Việc Cá Nhân / Nhóm
📌 Giới thiệu

Nền tảng Quản lý Công việc Cá nhân/Nhóm là hệ thống backend được xây dựng nhằm hỗ trợ người dùng quản lý công việc hiệu quả, theo dõi tiến độ và cộng tác nhóm.

Dự án được phát triển bằng:

☕ Java

🌱 Spring Boot

🛢 SQL (MySQL)

🔐 Spring Security + JWT

🐳 Docker

💻 IntelliJ IDEA Community Edition


🧱 Kiến trúc hệ thống

Hệ thống được xây dựng theo mô hình:

Controller → Service → Repository → Database


👤 Chức năng chính
🔐 Quản lý người dùng

Đăng ký tài khoản

Đăng nhập (JWT Authentication)

Mã hóa mật khẩu (BCrypt)

Phân quyền (USER / ADMIN)

📋 Quản lý công việc cá nhân

Tạo công việc

Cập nhật công việc

Xoá công việc

Đánh dấu hoàn thành

Lọc theo:

Trạng thái (TODO / IN_PROGRESS / DONE)

Độ ưu tiên (LOW / MEDIUM / HIGH)

Deadline

👥 Quản lý nhóm

Tạo nhóm

Thêm thành viên

Phân công công việc

Theo dõi tiến độ nhóm

Thống kê % hoàn thành

🐳 Chạy bằng Docker
Build image
docker build -t task-manager .

Run container
docker run -p 8080:8080 task-manager

🔐 API Authentication

Sau khi đăng nhập thành công, hệ thống sẽ trả về JWT Token.

Sử dụng token trong header:

Authorization: Bearer <your_token>

📈 Hướng phát triển tương lai

Comment trong task

Subtask

File attachment

Notification

WebSocket realtime

Swagger API Documentation

Unit Test (JUnit + Mockito)

CI/CD Pipeline

Công nghệ: Java, Spring Boot, Docker, SQL
