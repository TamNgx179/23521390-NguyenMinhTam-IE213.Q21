# Lab 4 - Thiết lập Frontend với ReactJS

# 1. Mục tiêu bài thực hành

Trong bài lab này sẽ xây dựng **frontend cho ứng dụng Movie Reviews** bằng **ReactJS**.

Các nội dung chính:

- Tạo project frontend bằng React
- Cài đặt Bootstrap để xây dựng giao diện
- Cài đặt React Router DOM để điều hướng giữa các trang
- Xây dựng Navigation Header
- Tạo các component giao diện cho ứng dụng
- Thiết lập định tuyến cho các trang
- Quản lý trạng thái đăng nhập bằng React Hook

---

# 2. Công cụ / môi trường sử dụng

Các công cụ được sử dụng trong lab:

- **ReactJS** – thư viện xây dựng giao diện người dùng
- **NodeJS** – môi trường chạy JavaScript
- **Bootstrap** – framework hỗ trợ thiết kế UI
- **React Router DOM** – thư viện định tuyến trong React
- **Visual Studio Code** – môi trường lập trình
- **Web Browser** – kiểm tra ứng dụng

---

# 3. Cách chạy

1. Di chuyển vào thư mục frontend
2. Cài đặt các thư viện: `npm install`
3. Chạy ứng dụng React: `npm start`
4. Mở trình duyệt tại: `http://localhost:3000`

---

# 4. Kết quả đầu ra

- Ứng dụng React chạy thành công
- Navigation bar hiển thị trên giao diện
- Có thể điều hướng giữa các trang
- Các component giao diện được hiển thị

---

# 5. Giải thích phần chính đã thực hiện

## React Components

Trong thư mục `components` tạo các component:

- `movies-list.js`
- `movie.js`
- `add-review.js`
- `login.js`

Các component này được import vào `App.js`.

---

## Navigation Bar

Navigation bar được xây dựng bằng **React Bootstrap**.

Thanh navigation bao gồm:

- Logo: Movie Reviews
- Link Movies
- Link Login / Logout

---

## React Router

Sử dụng **React Router DOM** để thiết lập định tuyến:

- `/` → MoviesList
- `/movies/:id` → Movie
- `/movies/:id/review` → AddReview
- `/login` → Login

---

## React Hook

Sử dụng **useState** để lưu trạng thái đăng nhập của người dùng:
Nếu user tồn tại → hiển thị Logout  
Nếu user null → hiển thị Login.

---

