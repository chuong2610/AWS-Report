---
title: "Worklog Tuần 6"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Xây dựng kiến trúc bảo mật đa lớp defense-in-depth
* Bảo vệ ứng dụng với AWS WAF (Web Application Firewall)
* Nắm vững mã hóa với AWS KMS (Key Management Service)
* Bảo mật credentials với AWS Secrets Manager và tự động rotation
* Triển khai phát hiện mối đe dọa thông minh với AWS GuardDuty
* Tích hợp xác thực người dùng với Amazon Cognito
* Đạt được tuân thủ bảo mật với AWS Security Hub
* Đảm bảo kết nối riêng tư với VPC Endpoints

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu AWS WAF <br> - **Thực hành:** <br>&emsp; + Tạo Web ACL <br>&emsp; + Chặn SQL Injection và XSS <br>&emsp; + Triển khai rate-limiting                                          | 13/10/2025   | 13/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Tìm hiểu AWS KMS <br> - **Thực hành:** <br>&emsp; + Tạo Customer Master Keys <br>&emsp; + Mã hóa EBS và S3 <br>&emsp; + Triển khai encryption                                 | 14/10/2025   | 14/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu AWS Secrets Manager <br> - **Thực hành:** <br>&emsp; + Lưu trữ credentials an toàn <br>&emsp; + Bật automatic rotation                                                | 15/10/2025   | 15/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu AWS GuardDuty <br> - **Thực hành:** <br>&emsp; + Bật threat detection <br>&emsp; + Theo dõi security findings                                                                  | 16/10/2025   | 16/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu Amazon Cognito <br> - **Thực hành:** <br>&emsp; + Triển khai user authentication <br>&emsp; + Cấu hình User Pools                                                            | 17/10/2025   | 17/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Tìm hiểu Security Hub và VPC Endpoints <br> - **Thực hành:** <br>&emsp; + Bật Security Hub <br>&emsp; + Cấu hình VPC Endpoints                                                 | 18/10/2025   | 18/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Ôn tập và kiểm tra bảo mật <br>&emsp; + Review security implementations <br>&emsp; + Chuẩn bị tuần tiếp                                                                           | 19/10/2025   | 19/10/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 6:
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


