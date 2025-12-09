---
title: "Worklog Tuần 7"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Nắm vững chiến lược migration từ on-premise lên AWS cloud
* Migration máy ảo với AWS VM Import/Export
* Thực hiện database migration với DMS và Schema Conversion Tool
* Triển khai disaster recovery với AWS Elastic Disaster Recovery
* Tập trung hoá quản lý backup với AWS Backup
* Xây dựng hệ thống đáng tin cậy với messaging (SQS và SNS)
* Hiểu các giải pháp shared storage (EBS Multi-Attach và EFS)

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tìm hiểu VM Migration với AWS VM Import/Export <br> - **Thực hành:** <br>&emsp; + Export VMs từ VirtualBox <br>&emsp; + Import lên AWS                                               | 20/10/2025   | 20/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Tìm hiểu Schema Conversion Tool <br> - **Thực hành:** <br>&emsp; + Convert Oracle schema sang Aurora PostgreSQL                                                                       | 21/10/2025   | 21/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu AWS DMS <br> - **Thực hành:** <br>&emsp; + Tạo Replication Instance <br>&emsp; + Cấu hình endpoints <br>&emsp; + Thực hiện migration                               | 22/10/2025   | 22/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu AWS Disaster Recovery <br> - **Thực hành:** <br>&emsp; + Cài DRS Agent <br>&emsp; + Cấu hình replication <br>&emsp; + Thực hiện Recovery Drill                    | 23/10/2025   | 23/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu AWS Backup <br> - **Thực hành:** <br>&emsp; + Tạo Backup Plans <br>&emsp; + Cấu hình cross-region backup                                                                  | 24/10/2025   | 24/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Tìm hiểu SQS và SNS <br> - **Thực hành:** <br>&emsp; + Triển khai decoupling <br>&emsp; + Xây dựng Fan-out pattern                                                                | 25/10/2025   | 25/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Tìm hiểu Shared Storage <br> - **Thực hành:** <br>&emsp; + Test EBS Multi-Attach <br>&emsp; + Deploy Amazon EFS                                                                           | 26/10/2025   | 26/10/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 7:

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


