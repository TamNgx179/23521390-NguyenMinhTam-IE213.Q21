# Lab 3 - Hoàn thiện Backend cho ứng dụng minh họa

# 1. Mục tiêu bài thực hành
Trong bài lab này sẽ tiếp tục phát triển backend cho ứng dụng **Movie Reviews**.

Các nội dung chính:

- Thiết lập API thêm review cho movie
- Thiết lập API cập nhật review
- Thiết lập API xóa review
- Lấy thông tin movie theo id kèm danh sách review
- Lấy danh sách rating của movie

---

# 2. Công cụ / môi trường sử dụng

Các công cụ được sử dụng trong lab:

- **NodeJS** – môi trường chạy JavaScript phía server
- **ExpressJS** – framework xây dựng web server
- **MongoDB Atlas** – hệ quản trị cơ sở dữ liệu NoSQL trên cloud
- **MongoDB Compass** – công cụ quản lý MongoDB
- **Visual Studio Code** – môi trường lập trình
- **Postman / Insomnia** – kiểm tra API

---

# 3. Cách chạy
1. Sử dụng các tài nguyên có sẵn đã có ở lab2
2. Thêm các file theo yêu cầu
3. Chạy server
4. Kiểm tra API bằng PostmanSau khi thực hiện các bước:

---

# 4. Kết quả đầu ra

- Server NodeJS chạy thành công
- Backend kết nối được với MongoDB Atlas
- API thêm / sửa / xóa review hoạt động
- API lấy thông tin movie theo id hoạt động
- API lấy danh sách rating hoạt động

Các endpoint chính:

### Thêm review
### Cập nhật review
### Xóa review
### Lấy thông tin movie theo id
### Lấy danh sách rating

---

# 5. Giải thích phần chính đã thực hiện
Trong bài lab này, backend được xây dựng theo kiến trúc tách lớp:
## Route

File `movies.route.js` định nghĩa các endpoint:

- `/review`
- `/id/:id`
- `/ratings`

---

## Controller

### ReviewsController

Xử lý các request liên quan đến review:

- `apiPostReview()` – thêm review
- `apiUpdateReview()` – cập nhật review
- `apiDeleteReview()` – xóa review

Controller sẽ nhận request từ client và gọi các phương thức trong **ReviewsDAO**.

---

### MoviesController

Cung cấp các API:

- `apiGetMovieById()` – lấy thông tin movie theo id
- `apiGetRatings()` – lấy danh sách rating

---

## DAO (Data Access Object)

### ReviewsDAO

Chịu trách nhiệm thao tác với collection **reviews**.

Các phương thức chính:

- `addReview()` – thêm review
- `updateReview()` – cập nhật review
- `deleteReview()` – xóa review

---

### MoviesDAO

Thực hiện truy vấn dữ liệu movie:

- `getMovieById()` – lấy thông tin movie kèm review (sử dụng **aggregation pipeline** với `$match` và `$lookup`)
- `getRatings()` – lấy danh sách rating từ collection movies.

---