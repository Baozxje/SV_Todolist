# 🚀 NỀN TẢNG QUẢN LÝ CÔNG VIỆC CÁ NHÂN / NHÓM

## 📌 Giới thiệu

Hệ thống backend hỗ trợ quản lý công việc cá nhân và nhóm, giúp theo dõi tiến độ, phân công nhiệm vụ và cộng tác hiệu quả.

---

## 🛠 Công nghệ sử dụng

- Java
- Spring Boot
- Spring Security + JWT
- Spring Data JPA
- MySQL
- Docker
- Maven

---

## 🧱 Kiến trúc hệ thống

```
Controller → Service → Repository → Database
```

Cấu trúc thư mục:

```
com.taskmanager
 ├── config
 ├── controller
 ├── service
 ├── repository
 ├── entity
 ├── dto
 ├── security
 ├── exception
```

---

## 👤 Chức năng chính

### 🔐 Quản lý người dùng
- Đăng ký
- Đăng nhập (JWT)
- Phân quyền (USER / ADMIN)

### 📋 Quản lý công việc cá nhân
- Tạo task
- Cập nhật task
- Xoá task
- Đánh dấu hoàn thành
- Lọc theo trạng thái, deadline, độ ưu tiên

### 👥 Quản lý nhóm
- Tạo nhóm
- Thêm thành viên
- Phân công công việc
- Theo dõi tiến độ nhóm

---


### Clone project

```
git clone https://github.com/Baozxje/SV_Todolist.git
```


### Chạy project

```
mvn spring-boot:run
```


---

## 👨‍💻 Tác giả

Lam Gia Bao  
Backend Developer – Java & Spring Boot
