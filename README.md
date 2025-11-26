# 🛒 Báo cáo Đồ án: Kiểm thử Hệ thống Thương mại Điện tử ProShop

![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen?style=for-the-badge&logo=react)
![Test Coverage](https://img.shields.io/badge/Coverage-85%25-green?style=for-the-badge&logo=jest)
![Postman](https://img.shields.io/badge/API_Testing-Postman-orange?style=for-the-badge&logo=postman)
![JMeter](https://img.shields.io/badge/Performance-JMeter-red?style=for-the-badge&logo=apachejmeter)

> **Môn học:** Kiểm thử Phần mềm (Software Testing)  
> **Mã học phần:** 841408  
> **Giảng viên hướng dẫn:** ThS. Từ Lãng Phiêu

---

## 👨‍💻 Thông tin Sinh viên thực hiện

| STT | Họ và Tên | MSSV | Vai trò |
| :---: | :--- | :--- | :--- |
| **1** | **Hoàng Sỹ Khiêm** | **3121410263** | **Leader / Fullstack Tester** |

---

## 📖 Giới thiệu Dự án (Project Overview)

**ProShop** là một nền tảng thương mại điện tử (eCommerce) đầy đủ tính năng được xây dựng dựa trên kiến trúc Monolithic hiện đại với **MERN Stack** (MongoDB, Express, React, Node.js).

Dự án này được lựa chọn làm đối tượng nghiên cứu để áp dụng quy trình **Kiểm thử Phần mềm Toàn diện (Full-cycle Testing)**, từ kiểm thử đơn vị, kiểm thử tích hợp đến kiểm thử hiệu năng và bảo mật.

### 🛠 Công nghệ sử dụng:
* **Frontend:** React.js, Redux Toolkit, React Bootstrap.
* **Backend:** Node.js, Express.js.
* **Database:** MongoDB (Atlas/Local).
* **Testing Tools:** Jest, Postman, Newman, Apache JMeter, Selenium (optional).

---

## 🧪 Phạm vi & Kỹ thuật Kiểm thử (Testing Scope)

Báo cáo tập trung vào 4 cấp độ kiểm thử chính:

### 1. Kiểm thử Hộp đen (Black-box Testing)
* **Kỹ thuật áp dụng:** Phân hoạch tương đương (EP), Phân tích giá trị biên (BVA), Bảng quyết định (Decision Table), Kiểm thử chuyển đổi trạng thái (State Transition).
* **Chức năng kiểm thử:** Đăng ký/Đăng nhập, Tìm kiếm sản phẩm, Giỏ hàng, Quy trình thanh toán (Checkout flow).

### 2. Kiểm thử Hộp trắng (White-box Testing)
* **Công cụ:** Jest Framework.
* **Phạm vi:** Kiểm thử dòng điều khiển (Control Flow) và logic nghiệp vụ tại các Controller quan trọng (`OrderController`, `AuthController`).
* **Kết quả:** Đạt độ bao phủ mã nguồn (Code Coverage) > 85%.

### 3. Kiểm thử Tích hợp & API (Integration Testing)
* **Công cụ:** Postman & Newman CLI.
* **Phạm vi:** 25+ RESTful API Endpoints.
* **Mục tiêu:** Kiểm tra tính toàn vẹn dữ liệu, luồng xác thực JWT (HttpOnly Cookie) và phân quyền Admin/User.

### 4. Kiểm thử Hiệu năng (Performance Testing)
* **Công cụ:** Apache JMeter 5.5.
* **Kịch bản:** * **Load Test:** 500 người dùng truy cập trang chủ đồng thời.
    * **Stress Test:** 100 người dùng thực hiện đặt hàng cùng lúc.
* **Kết quả:** Hệ thống hoạt động ổn định với thời gian phản hồi trung bình (Avg Response Time) < 200ms.

---

## 📂 Tài liệu Báo cáo (Documentation)

Toàn bộ quá trình phân tích yêu cầu, thiết kế Test Case, Test Script và kết quả thực nghiệm được trình bày chi tiết trong báo cáo đồ án.

* 📄 **Xem Báo cáo (PDF):** [Click để tải xuống](https://github.com/khiemHoang1410/Software-Testing-BookCart/blob/main/BAO_CAO_TESTING.pdf)
* 🔗 **Xem trực tuyến (Overleaf):** [>> Link Project Overleaf <<](https://www.overleaf.com/read/jpdndpqfzpxb#bdc356)

---

## 🚀 Hướng dẫn Cài đặt & Chạy Project (Local)

Để giảng viên và các bạn có thể chạy thử nghiệm dự án, vui lòng thực hiện theo các bước sau:

### Bước 1: Clone dự án và Cài đặt thư viện
```bash
# Clone source code
git clone [https://github.com/zehel-dev/proshop-v2.git](https://github.com/zehel-dev/proshop-v2.git)
cd proshop-v2

# Cài đặt dependencies cho Backend
npm install

# Cài đặt dependencies cho Frontend
cd frontend
npm install
cd ..