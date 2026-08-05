---
title: "Bản đề xuất"
date: 2026-06-22
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

Tại phần này, em trình bày đề xuất triển khai dự án **EduWallet** trên nền tảng Amazon Web Services (AWS). Nội dung bao gồm tổng quan dự án, kiến trúc hệ thống, kế hoạch triển khai, ngân sách dự kiến và các rủi ro có thể gặp phải trong quá trình thực hiện.

# EduWallet
## Hệ thống quản lý tài chính cá nhân trên nền tảng AWS

### 1. Tóm tắt điều hành

EduWallet là một ứng dụng quản lý tài chính cá nhân dành cho sinh viên, giúp người dùng ghi nhận các khoản thu nhập, chi tiêu, quản lý ngân sách và theo dõi tình hình tài chính hằng ngày.

Dự án được đề xuất triển khai trên nền tảng Amazon Web Services (AWS) nhằm tận dụng các dịch vụ điện toán đám mây để xây dựng một hệ thống có khả năng mở rộng, an toàn và dễ dàng quản lý. Bên cạnh mục tiêu xây dựng một ứng dụng thực tế, dự án còn giúp áp dụng các kiến thức đã học trong chương trình thực tập AWS First Cloud AI Journey.

---

### 2. Tuyên bố vấn đề

#### Vấn đề hiện tại

Hiện nay nhiều sinh viên vẫn quản lý chi tiêu bằng sổ tay hoặc bảng tính Excel, dẫn đến một số hạn chế như:

- Khó theo dõi các khoản thu và chi hằng ngày.
- Không có hệ thống lưu trữ dữ liệu tập trung.
- Dữ liệu dễ bị mất khi thay đổi thiết bị.
- Khó lập kế hoạch ngân sách cá nhân.
- Không có công cụ thống kê và theo dõi tình hình tài chính.

#### Giải pháp đề xuất

EduWallet được xây dựng như một hệ thống quản lý tài chính cá nhân trên nền tảng AWS.

Người dùng có thể đăng nhập an toàn, quản lý các khoản thu chi, lưu trữ hình ảnh hóa đơn và theo dõi dữ liệu tài chính thông qua một cơ sở dữ liệu tập trung. Hệ thống cũng sử dụng các dịch vụ giám sát của AWS nhằm đảm bảo hoạt động ổn định.

#### Lợi ích mang lại

- Quản lý tài chính cá nhân thuận tiện.
- Đăng nhập và xác thực người dùng an toàn.
- Lưu trữ dữ liệu tập trung trên nền tảng Cloud.
- Nâng cao khả năng triển khai ứng dụng trên AWS.
- Tạo nền tảng để phát triển các tính năng phân tích tài chính bằng AI trong tương lai.

---

### 3. Kiến trúc giải pháp

Dự án được xây dựng theo mô hình kiến trúc 3 lớp gồm:

- Presentation Layer
- Application Layer
- Database Layer

**Sơ đồ kiến trúc**

![EduWallet Architecture](/images/AWS_EduWallet.drawio.png)

### Dịch vụ AWS sử dụng

- **Amazon EC2**
  - Triển khai ứng dụng Backend.

- **Amazon RDS PostgreSQL**
  - Lưu trữ dữ liệu người dùng và các giao dịch tài chính.

- **Amazon S3**
  - Lưu trữ hình ảnh hóa đơn và các tệp đính kèm.

- **Amazon Cognito**
  - Xác thực và quản lý tài khoản người dùng.

- **Amazon CloudWatch**
  - Theo dõi hoạt động của hệ thống, ghi log và giám sát tài nguyên.

### Thiết kế thành phần

- Người dùng truy cập hệ thống thông qua trình duyệt web.
- Amazon Cognito xử lý việc đăng nhập và xác thực.
- Backend được triển khai trên Amazon EC2.
- Dữ liệu được lưu trong Amazon RDS PostgreSQL.
- Hình ảnh hóa đơn được lưu trên Amazon S3.
- Amazon CloudWatch theo dõi log và tình trạng hoạt động của hệ thống.

---

### 4. Triển khai kỹ thuật

#### Các giai đoạn triển khai

Dự án được chia thành bốn giai đoạn chính:

**Giai đoạn 1: Phân tích yêu cầu**

- Thu thập yêu cầu.
- Thiết kế cơ sở dữ liệu.
- Phân tích chức năng hệ thống.

**Giai đoạn 2: Chuẩn bị hạ tầng**

- Khởi tạo Amazon EC2.
- Cấu hình Amazon RDS.
- Tạo Amazon S3 Bucket.
- Thiết lập Amazon Cognito.

**Giai đoạn 3: Phát triển ứng dụng**

- Xây dựng Backend.
- Kết nối cơ sở dữ liệu.
- Xây dựng chức năng xác thực.
- Xây dựng chức năng tải ảnh hóa đơn.

**Giai đoạn 4: Kiểm thử và hoàn thiện**

- Kiểm thử chức năng.
- Kiểm tra kết nối các dịch vụ AWS.
- Hoàn thiện tài liệu Workshop và báo cáo.

#### Yêu cầu kỹ thuật

- Tài khoản AWS.
- Amazon EC2.
- Amazon RDS PostgreSQL.
- Amazon S3.
- Amazon Cognito.
- Amazon CloudWatch.
- Visual Studio Code.
- Git và GitHub.

---

### 5. Lộ trình triển khai

| Tuần | Nội dung |
|------|----------|
| Tuần 1 | Tìm hiểu AWS và chuẩn bị môi trường phát triển |
| Tuần 2 | Tìm hiểu IAM, VPC và các dịch vụ mạng |
| Tuần 3 | Nghiên cứu Database và Solution Architecture |
| Tuần 4 | Tìm hiểu Amazon S3 và các dịch vụ lưu trữ |
| Tuần 5 | Tìm hiểu triển khai ứng dụng và Serverless |
| Tuần 6 | Phân tích yêu cầu và thiết kế hệ thống EduWallet |
| Tuần 7 | Hoàn thiện Proposal và kiến trúc hệ thống |
| Tuần 8 | Triển khai Workshop và hoàn thiện báo cáo |

---

### 6. Ước tính ngân sách

Trong giai đoạn phát triển, dự án chủ yếu sử dụng AWS Free Tier.

| Dịch vụ AWS | Chi phí dự kiến |
|-------------|----------------:|
| Amazon EC2 | Free Tier |
| Amazon RDS PostgreSQL | Free Tier |
| Amazon S3 | Free Tier |
| Amazon Cognito | Free Tier |
| Amazon CloudWatch | Free Tier |

**Tổng chi phí dự kiến:** khoảng **0 – 10 USD/tháng** trong quá trình phát triển.

---

### 7. Đánh giá rủi ro

#### Các rủi ro có thể gặp

- Cấu hình sai dịch vụ AWS.
- Phát sinh chi phí ngoài dự kiến.
- Mất dữ liệu.
- Người dùng truy cập trái phép.

#### Biện pháp giảm thiểu

- Áp dụng AWS Best Practices.
- Theo dõi chi phí bằng AWS Free Tier.
- Sao lưu cơ sở dữ liệu định kỳ.
- Áp dụng nguyên tắc phân quyền tối thiểu (Least Privilege).

#### Kế hoạch dự phòng

- Khôi phục dữ liệu từ bản sao lưu.
- Triển khai lại hệ thống khi xảy ra lỗi.
- Theo dõi hệ thống thông qua Amazon CloudWatch.

---

### 8. Kết quả kỳ vọng

#### Về mặt kỹ thuật

- Xây dựng thành công hệ thống quản lý tài chính cá nhân trên nền tảng AWS.
- Áp dụng các dịch vụ AWS vào một dự án thực tế.
- Hiểu quy trình triển khai ứng dụng trên Cloud.
- Nâng cao kỹ năng thiết kế và quản lý hệ thống AWS.

#### Định hướng phát triển

Trong tương lai, EduWallet có thể được mở rộng với các chức năng như:

- Phân tích thói quen chi tiêu bằng AI.
- Báo cáo tài chính trực quan.
- Gợi ý kế hoạch tiết kiệm.
- Phát triển ứng dụng trên nền tảng di động.