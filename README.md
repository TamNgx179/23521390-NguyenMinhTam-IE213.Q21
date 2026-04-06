# 23521390-NguyenMinhTam-IE213.Q21

## 1. Thông tin sinh viên
* Họ tên: Nguyễn Minh Tâm
* MSSV: 23521390
* Lớp: CNTT2023.2

---

## 2. Môn học
**IE213.Q21 - Kỹ thuật phát triển hệ thống Web**

---

# 3. Danh sách các Lab

| Lab   | Nội dung |
|------ |----------|
| Lab 1 | MongoDB CRUD Operation |
| Lab 2 | Thiết lập Backend với NodeJS và ExpressJS |
| Lab 3 | Hoàn thiện Backend cho ứng dụng minh họa |

---

# 4. Mô tả ngắn gọn từng Lab

## Lab 1: MongoDB CRUD Operation
Lab này mục tiêu làm quen với MongoDB Atlas, MongoDB Compass và các thao tác cơ bản với MongoDB như:

* Tạo database
* Thêm document
* Truy vấn dữ liệu
* Cập nhật dữ liệu
* Xóa field
* Thực hiện aggregation

Các thao tác được thực hiện bằng **MongoDB Shell (Mongosh)** trong **MongoDB Compass**.

---

## Lab 2: Thiết lập Backend với NodeJS và ExpressJS

Lab này tập trung vào việc xây dựng **backend server** sử dụng **NodeJS và ExpressJS** và kết nối với **MongoDB Atlas**.

Các nội dung chính thực hiện trong lab:

* Thiết lập môi trường phát triển với **NodeJS**
* Xây dựng backend server bằng **ExpressJS**
* Kết nối server với **MongoDB Atlas**
* Tổ chức project theo mô hình kiến trúc:

  - Route
  - Controller
  - DAO (Data Access Object)

* Xây dựng API để truy vấn dữ liệu **movies** từ database

---

## Lab 3: Hoàn thiện Backend cho ứng dụng minh họa

Lab 3 tiếp tục phát triển backend cho ứng dụng **Movie Reviews**.

Các nội dung chính thực hiện:

* Xây dựng API thêm review cho movie
* Xây dựng API cập nhật review
* Xây dựng API xóa review
* Xây dựng API lấy thông tin và review movie dựa trên ID
* Xây dựng API lấy danh cách các rating
* Tạo Controller để xử lý request từ client
* Tạo DAO để thao tác dữ liệu với MongoDB
* Kiểm tra API bằng Postman

--- 

# 5. Cách chạy chương trình

## Lab 1
1. Tạo tài khoản **MongoDB Atlas**
2. Tạo **Cluster miễn phí**
3. Kết nối cluster với **MongoDB Compass**
4. Mở **MongoDB Compass Shell**
5. Chạy các lệnh MongoDB trong file `lab1.js` hoặc copy vào **mongosh shell**

---

## Lab 2
1. Di chuyển vào thư mục Lab2
2. Cài đặt các thư viện cần thiết
3. Tạo file môi trường `.env` và cấu hình chuỗi kết nối MongoDB
4. Chạy server
5. Kiểm tra API bằng trình duyệt hoặc Postman

---

## Lab 3
1. Sử dụng các tài nguyên có sẵn đã có ở lab2
2. Thêm các file theo yêu cầu
3. Chạy server
4. Kiểm tra API bằng Postman

---

# 6. Kết quả thực hiện

## Lab 1
Các chức năng đã thực hiện:

* Tạo database `MSSV-IE213`
* Thêm dữ liệu vào collection `employees`
* Thiết lập `id` là unique
* Truy vấn dữ liệu theo điều kiện
* Cập nhật document
* Thực hiện aggregation để tính tổng và trung bình tuổi theo organization

---

## Lab 2
Sau khi thực hiện lab:

* Server **NodeJS + ExpressJS** được khởi tạo thành công
* Backend kết nối được với **MongoDB Atlas**
* API `/api/v1/movies` hoạt động
* Dữ liệu movie được trả về dạng **JSON**
* Có thể **phân trang** và **lọc dữ liệu** theo `title` hoặc `rated`

---

## Lab 3
Sau khi thực hiện lab:

* Backend server chạy thành công bằng **NodeJS + ExpressJS**
* Backend kết nối được với **MongoDB Atlas**
* API `/api/v1/movies/review` hoạt động
* Có thể thêm review, cập nhật review, xóa review, lấy movie theo id, lấy danh sách rating

---

# 7. Hình ảnh minh họa
Các hình ảnh minh họa được lưu trong thư mục **images** trong từng thư mục Lab tương ứng.

---

# 8. Nội dung đã hoàn thành

* Lab 1 - MongoDB CRUD Operation
* Lab 2 - Thiết lập Backend với NodeJS và ExpressJS
* Lab 3 - Hoàn thiện Backend cho ứng dụng minh họa

---

# 9. Nội dung chưa hoàn thành

* Lab 4
* Lab 5
* Lab 6