# Lab 1 - MongoDB CRUD Operation

# 1. Mục tiêu bài thực hành
Làm quen với hệ quản trị cơ sở dữ liệu **MongoDB** và các thao tác cơ bản trong MongoDB như:
* Tạo database trên MongoDB Atlas
* Kết nối MongoDB Atlas với MongoDB Compass
* Thực hiện các thao tác CRUD:
  * Create (thêm document)
  * Read (truy vấn dữ liệu)
  * Update (cập nhật dữ liệu)
  * Delete (xóa field dữ liệu)
* Sử dụng **aggregation** để tính toán dữ liệu.

---

# 2. Công cụ / môi trường sử dụng
Các công cụ được sử dụng trong lab:
* **MongoDB Atlas** – tạo cluster database trên cloud
* **MongoDB Compass** – công cụ để quản lý MongoDB
* **MongoDB Shell (Mongosh)** – thực hiện các lệnh MongoDB

---

## 3. Cách chạy
1. Tạo tài khoản **MongoDB Atlas** và tạo một **Cluster miễn phí**.
2. Kết nối Cluster với **MongoDB Compass**.
3. Mở **MongoDB Compass Shell (Mongosh)**.
4. Chạy các lệnh MongoDB có trong file `lab1.js`.
5. Quan sát kết quả trực tiếp trên MongoDB Compass.


---

# 4. Kết quả đầu ra

Sau khi thực hiện các bước trên:

* Database `MSSV-IE213` được tạo
* Collection `employees` chứa các document nhân viên
* Field `id` được thiết lập unique
* Có thể truy vấn dữ liệu theo điều kiện
* Các document được cập nhật organization
* Có thể tính tổng tuổi và tuổi trung bình theo organization

---

# 5. Giải thích phần chính đã thực hiện

Trong bài lab này, sử dụng MongoDB để thực hiện các thao tác CRUD cơ bản.
* **InsertMany** được dùng để thêm nhiều document vào collection.
* **Find** được sử dụng để truy vấn dữ liệu theo điều kiện.
* **UpdateMany với $set** giúp cập nhật hoặc thêm field mới cho document.
* **$unset** dùng để xóa field khỏi document.
* **Aggregation với $group** cho phép nhóm dữ liệu theo organization và tính toán tổng tuổi và tuổi trung bình của nhân viên.

