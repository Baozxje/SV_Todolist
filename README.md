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

🎯 Mục tiêu dự án

Xây dựng hệ thống backend theo kiến trúc chuẩn RESTful API

Áp dụng Spring Security và JWT để xác thực người dùng

Thiết kế cơ sở dữ liệu chuẩn hóa

Docker hóa hệ thống để dễ triển khai

Rèn luyện kỹ năng phát triển backend thực tế

🧱 Kiến trúc hệ thống

Hệ thống được xây dựng theo mô hình:

Controller → Service → Repository → Database


Cấu trúc thư mục:

com.taskmanager
 ├── config
 ├── controller
 ├── service
 ├── repository
 ├── entity
 ├── dto
 ├── security
 ├── exception
 └── TaskManagerApplication.java

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

🛢 Thiết kế cơ sở dữ liệu
Bảng users
Field	Type	Description
id	Long	Primary Key
username	String	Tên người dùng
email	String	Email
password	String	Mật khẩu đã mã hóa
role	String	USER / ADMIN
created_at	DateTime	Ngày tạo
Bảng tasks
Field	Type	Description
id	Long	Primary Key
title	String	Tiêu đề
description	String	Mô tả
status	Enum	TODO / IN_PROGRESS / DONE
priority	Enum	LOW / MEDIUM / HIGH
deadline	DateTime	Hạn hoàn thành
user_id	Long	Người tạo
group_id	Long	(Nullable)
Bảng groups
Field	Type
id	Long
name	String
created_by	Long
created_at	DateTime
Bảng group_members
Field	Type
id	Long
group_id	Long
user_id	Long
⚙️ Công nghệ sử dụng
Công nghệ	Vai trò
Spring Boot	Framework backend
Spring Data JPA	ORM
Spring Security	Xác thực & phân quyền
JWT	Token-based authentication
MySQL	Database
Docker	Containerization
Maven	Quản lý dependency
🚀 Hướng dẫn chạy dự án
1️⃣ Clone project
git clone https://github.com/Baozxje/SV_Todolist.git
cd SV_Todolist

2️⃣ Cấu hình database

Tạo database MySQL:

CREATE DATABASE task_manager_db;


Cập nhật application.yml:

spring:
  datasource:
    url: jdbc:mysql://localhost:3306/task_manager_db
    username: root
    password: 123456

3️⃣ Chạy project
mvn spring-boot:run


Hoặc chạy trực tiếp trong IntelliJ.

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

📜 License

Dự án phục vụ mục đích học tập và nghiên cứu.
