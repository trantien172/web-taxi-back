
Google Maps / GPS
## Giới thiệu

Hệ thống đặt xe taxi trực tuyến là ứng dụng web được xây dựng nhằm kết nối khách hàng với tài xế thông qua nền tảng số. Hệ thống hỗ trợ đặt xe, theo dõi hành trình theo thời gian thực, quản lý tài xế, thanh toán trực tuyến và thống kê hoạt động kinh doanh.

Dự án được phát triển dựa trên mô hình hoạt động của các nền tảng gọi xe công nghệ hiện nay như Grab, Be và Gojek.

---

# Mục tiêu dự án

Mục tiêu của dự án là xây dựng một hệ thống quản lý và điều phối xe trực tuyến giúp:

* Đơn giản hóa quy trình đặt xe.
* Kết nối khách hàng với tài xế nhanh chóng.
* Theo dõi vị trí và trạng thái chuyến đi theo thời gian thực.
* Hỗ trợ thanh toán điện tử.
* Cung cấp công cụ quản trị và báo cáo cho doanh nghiệp vận tải.

---

# Đối tượng sử dụng

## Khách hàng (Client)

* Đăng ký, đăng nhập tài khoản.
* Đặt xe trực tuyến.
* Chọn điểm đón và điểm đến.
* Theo dõi hành trình xe.
* Thanh toán trực tuyến.
* Xem lịch sử chuyến đi.
* Đánh giá chất lượng dịch vụ.

## Tài xế (Driver)

* Nhận thông báo chuyến đi mới.
* Chấp nhận hoặc từ chối chuyến xe.
* Cập nhật trạng thái chuyến đi.
* Theo dõi lịch sử hoạt động.
* Xem đánh giá từ khách hàng.

## Quản trị viên (Admin)

* Quản lý khách hàng.
* Quản lý tài xế.
* Quản lý phương tiện.
* Quản lý chuyến đi.
* Quản lý giá cước và khuyến mãi.
* Theo dõi doanh thu.
* Xem báo cáo và thống kê.

---

# Chức năng chính

## Xác thực và phân quyền

* Đăng ký tài khoản.
* Đăng nhập.
* JWT Authentication.
* Phân quyền theo vai trò (Client, Driver, Admin).

## Quản lý người dùng

* Quản lý khách hàng.
* Quản lý tài xế.
* Quản lý tài khoản quản trị.
* Phân quyền người dùng.

## Quản lý chuyến đi

* Tạo yêu cầu đặt xe.
* Ghép tài xế với khách hàng.
* Theo dõi trạng thái chuyến đi.
* Lưu lịch sử chuyến xe.
* Hủy chuyến.

## Theo dõi vị trí thời gian thực

* WebSocket.
* Cập nhật vị trí tài xế.
* Theo dõi lộ trình di chuyển.
* Đồng bộ trạng thái chuyến đi theo thời gian thực.

## Bản đồ và điều hướng

* Hiển thị vị trí trên bản đồ.
* Tìm đường từ điểm đón đến điểm trả khách.
* Tính khoảng cách và thời gian dự kiến.

## Thanh toán

* Thanh toán trực tuyến.
* Theo dõi lịch sử thanh toán.
* Quản lý doanh thu chuyến xe.

## Quản lý dịch vụ

* Quản lý giá cước.
* Quản lý ưu đãi.
* Cấu hình loại xe và dịch vụ.

## Báo cáo và thống kê

* Thống kê số lượng chuyến đi.
* Thống kê doanh thu.
* Phân tích hiệu suất hoạt động.
* Xuất báo cáo quản trị.

---

# Quy trình đặt xe

1. Khách hàng đăng nhập.
2. Nhập điểm đón và điểm đến.
3. Hệ thống tính toán tuyến đường.
4. Gửi yêu cầu đến tài xế phù hợp.
5. Tài xế nhận chuyến.
6. Khách hàng theo dõi hành trình.
7. Hoàn thành chuyến đi.
8. Thanh toán và đánh giá dịch vụ.

---

# Kiến trúc hệ thống

```text
Client Web Application
          │
          ▼
 REST API + WebSocket
          │
          ▼
        Backend
          │
          ▼
       Database
```

Hệ thống sử dụng REST API cho các nghiệp vụ thông thường và WebSocket cho các tính năng yêu cầu cập nhật thời gian thực như theo dõi vị trí và trạng thái chuyến đi.

---

# Công nghệ sử dụng

## Backend

* Node.js
* ExpressJS
* TypeScript
* MySQL
* JWT Authentication
* WebSocket

## Frontend

* ReactJS / NextJS
* TypeScript
* TailwindCSS

## Công cụ hỗ trợ

* Git
* GitHub
* Postman
* Figma

---

# Các module chính

* Authentication Module
* User Module
* Driver Module
* Ride Module
* Payment Module
* Service Module
* Promotion Module
* Report Module
* Media Module
* Notification Module

---

# Tài liệu hệ thống

```text
docs/
├── architecture
├── database
├── use-cases
├── workflows
├── screenshots
└── api
```

---

# Hướng phát triển

* Ứng dụng di động cho khách hàng.
* Ứng dụng di động cho tài xế.
* Tích hợp AI gợi ý tài xế tối ưu.
* Dự báo nhu cầu theo khu vực.
* Tích hợp nhiều cổng thanh toán.
* Theo dõi vị trí GPS chính xác hơn.

---

# Tác giả

Trần Tiến

Sinh viên Công nghệ Thông tin

Backend Developer | Fullstack Developer
