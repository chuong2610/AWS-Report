---
title: "Worklog Tuần 4"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Tự động hóa khả năng mở rộng hệ thống với EC2 Auto Scaling
* Triển khai giám sát toàn diện với Amazon CloudWatch
* Nắm vững quản lý DNS với Amazon Route 53
* Tối ưu hóa phân phối nội dung toàn cầu với Amazon CloudFront và Lambda@Edge
* Học tự động hóa command line với AWS CLI
* Hiểu advanced networking với VPC Peering

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu EC2 Auto Scaling <br> - **Thực hành:** <br>&emsp; + Tạo Launch Templates <br>&emsp; + Cấu hình Auto Scaling Groups <br>&emsp; + Thiết lập Scaling Policy              | 29/09/2025   | 29/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Tìm hiểu Amazon CloudWatch <br> - **Thực hành:** <br>&emsp; + Theo dõi standard metrics <br>&emsp; + Cài CloudWatch Agent <br>&emsp; + Tạo Alarms với SNS                    | 30/09/2025   | 30/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu CloudWatch Logs và Dashboards <br> - **Thực hành:** <br>&emsp; + Đẩy logs lên CloudWatch <br>&emsp; + Tạo Dashboard                                                       | 01/10/2025   | 01/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu Amazon Route 53 <br> - **Thực hành:** <br>&emsp; + Tạo Hosted Zones <br>&emsp; + Cấu hình Failover Routing <br>&emsp; + Thiết lập Health Checks                    | 02/10/2025   | 02/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu Amazon CloudFront <br> - **Thực hành:** <br>&emsp; + Deploy CloudFront distribution <br>&emsp; + Cấu hình OAC <br>&emsp; + Tối ưu hóa caching                       | 03/10/2025   | 03/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Tìm hiểu Lambda@Edge <br> - **Thực hành:** <br>&emsp; + Viết Lambda functions <br>&emsp; + Sửa đổi HTTP headers <br>&emsp; + Implement A/B testing                                   | 04/10/2025   | 04/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Tìm hiểu AWS CLI và VPC Peering <br> - **Thực hành:** <br>&emsp; + Viết scripts tự động hóa <br>&emsp; + Kết nối VPC Peering <br>&emsp; + Ôn tập tuần 4               | 05/10/2025   | 05/10/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 4:

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


