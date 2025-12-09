---
title: "Worklog Tuần 3"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Chuyển từ quản lý database thủ công sang AWS Managed Database services
* Nắm vững Amazon RDS (Relational Database Service) với Multi-AZ deployment
* Học khái niệm NoSQL database với Amazon DynamoDB
* Triển khai in-memory caching với Amazon ElastiCache
* Xây dựng kiến trúc Highly Available Web Applications
* Hiểu AWS Managed Microsoft AD cho tích hợp doanh nghiệp

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu Amazon RDS cơ bản <br> - **Thực hành:** <br>&emsp; + Deploy RDS với MySQL/PostgreSQL <br>&emsp; + Bật Multi-AZ deployment <br>&emsp; + Tìm hiểu replication và failover  | 22/09/2025   | 22/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Tìm hiểu RDS Operations và Security <br> - **Thực hành:** <br>&emsp; + Cấu hình Security Groups <br>&emsp; + Thiết lập Automated Backups <br>&emsp; + Test Restore              | 23/09/2025   | 23/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu Amazon DynamoDB cơ bản <br> - **Thực hành:** <br>&emsp; + Thiết kế bảng DynamoDB <br>&emsp; + So sánh Provisioned vs On-Demand                                         | 24/09/2025   | 24/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu DynamoDB nâng cao <br> - **Thực hành:** <br>&emsp; + Thực hiện PutItem, GetItem, Query, Scan <br>&emsp; + Tạo Global Secondary Index                                     | 25/09/2025   | 25/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu Amazon ElastiCache <br> - **Thực hành:** <br>&emsp; + Deploy ElastiCache với Redis <br>&emsp; + Implement Lazy Loading strategy                                                 | 26/09/2025   | 26/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Tìm hiểu kiến trúc High Availability <br> - **Thực hành:** <br>&emsp; + Xây dựng kiến trúc 3-tier <br>&emsp; + Deploy ALB <br>&emsp; + Tích hợp S3                           | 27/09/2025   | 27/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Tìm hiểu AWS Managed Microsoft AD <br> - **Thực hành:** <br>&emsp; + Thiết lập Managed AD <br>&emsp; + Join Windows EC2 vào domain                                                   | 28/09/2025   | 28/09/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 3:

* Hiểu AWS là gì và nắm được các nhóm dịch vụ cơ bản: 
  * Compute
  * Storage
  * Networking 
  * Database
  * ...

* Đã tạo và cấu hình AWS Free Tier account thành công.

* Làm quen với AWS Management Console và biết cách tìm, truy cập, sử dụng dịch vụ từ giao diện web.

* Cài đặt và cấu hình AWS CLI trên máy tính bao gồm:
  * Access Key
  * Secret Key
  * Region mặc định
  * ...

* Sử dụng AWS CLI để thực hiện các thao tác cơ bản như:

  * Kiểm tra thông tin tài khoản & cấu hình
  * Lấy danh sách region
  * Xem dịch vụ EC2
  * Tạo và quản lý key pair
  * Kiểm tra thông tin dịch vụ đang chạy
  * ...

* Có khả năng kết nối giữa giao diện web và CLI để quản lý tài nguyên AWS song song.
* ...


