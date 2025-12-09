---
title: "Worklog Tuần 8"
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Nắm vững tối ưu hóa chi phí và thực hành FinOps cho quản lý tài chính cloud
* Phân tích mẫu chi tiêu với AWS Cost Explorer và Cost & Usage Reports
* Triển khai right-sizing recommendations để loại bỏ lãng phí tài nguyên
* Hiểu giá dựa trên cam kết với Savings Plans và Reserved Instances
* Quản lý service quotas chủ động để tránh lỗi triển khai
* Xây dựng kiến trúc mạng tập trung với AWS Transit Gateway
* Giám sát traffic mạng với VPC Flow Logs cho bảo mật và troubleshooting
* Ủy quyền truy cập billing với kiểm soát IAM phù hợp
* Tự động hóa quản lý EBS lifecycle để tối ưu backup

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu Cost Explorer và CUR <br> - **Thực hành:** <br>&emsp; + Phân tích chi phí theo Service, Region, Tags <br>&emsp; + Bật CUR export                                | 27/10/2025   | 27/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Tìm hiểu Cost Analytics với Athena <br> - **Thực hành:** <br>&emsp; + Query CUR data <br>&emsp; + Phân tích data transfer costs                                                   | 28/10/2025   | 28/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu Right-Sizing <br> - **Thực hành:** <br>&emsp; + Sử dụng Compute Optimizer <br>&emsp; + Triển khai downsizing                                                                | 29/10/2025   | 29/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu Savings Plans <br> - **Thực hành:** <br>&emsp; + So sánh các loại Savings Plans <br>&emsp; + Tính toán tiết kiệm                                                 | 30/10/2025   | 30/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu Service Quotas <br> - **Thực hành:** <br>&emsp; + Review service limits <br>&emsp; + Thiết lập CloudWatch alarms                                                                | 31/10/2025   | 31/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Tìm hiểu Transit Gateway <br> - **Thực hành:** <br>&emsp; + Kết nối VPCs qua Transit Gateway <br>&emsp; + Cấu hình route tables                                                 | 01/11/2025   | 01/11/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Tìm hiểu VPC Flow Logs và Billing Delegation <br> - **Thực hành:** <br>&emsp; + Bật VPC Flow Logs <br>&emsp; + Tạo IAM roles cho finance team                             | 02/11/2025   | 02/11/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 8:

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


