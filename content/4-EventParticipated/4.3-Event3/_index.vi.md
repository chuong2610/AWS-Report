---
title: "Event 3"
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Báo Cáo Tổng Kết: AWS Cloud Mastery Series #2
**Chủ đề:** TỪ DEVOPS, IaC ĐẾN CONTAINER & OBSERVABILITY

## 1. Mục Tiêu Cốt Lõi

Sự kiện tập trung vào cuộc cách mạng hóa quy trình vận hành và phát triển phần mềm trên nền tảng Cloud:

* **Chuyển đổi tư duy (Mindset Shift):** Cân bằng giữa tốc độ ra mắt tính năng (Speed) và sự ổn định hệ thống (Stability) thông qua văn hóa DevOps và Vòng đời giá trị (Value Cycle).
* **Hiện đại hóa hạ tầng:** Loại bỏ rủi ro của quản trị thủ công (ClickOps) bằng phương pháp quản trị hạ tầng như mã nguồn (Infrastructure as Code - IaC).
* **Chiến lược Container hóa:** Đưa ra khung tham chiếu để lựa chọn nền tảng điều phối phù hợp: từ đơn giản (App Runner), chuyên biệt (ECS) đến chuẩn mở (EKS).
* **Thấu hiểu hệ thống (Deep Observability):** Chuyển từ giám sát thụ động sang chủ động phân tích hành vi hệ thống với CloudWatch và X-Ray.

## 2. Diễn Giả Tham Gia

* **Đội ngũ chuyên gia AWS:** Cung cấp kiến thức nền tảng và các bài demo thực chiến (Best Practices).
* **Anh Trần Vĩ & Anh Long Quy Nghiêm** (FCJers 2024): Chia sẻ kinh nghiệm thực tế từ góc nhìn của người đang trực tiếp tham gia chương trình First Cloud Journey.

---

## 3. Nội Dung Chuyên Sâu

### 3.1. DevOps Mindset & CI/CD Pipeline: Nền Tảng Của Tốc Độ

DevOps không chỉ là công cụ, mà là triết lý tối ưu dòng chảy giá trị:

* **The Value Cycle:** Quy trình khép kín từ *Insight* (Ý tưởng) đến *Delivery* (Chuyển giao).
* **Định nghĩa lại CI/CD:**
    * *Continuous Integration (CI):* Cam kết code hàng ngày, fail fast để phát hiện lỗi sớm.
    * *Continuous Delivery:* Tự động deploy đến Staging, nhưng ra Production cần phê duyệt (Manual Approval).
    * *Continuous Deployment:* Tự động hóa 100% đến Production nếu vượt qua mọi bài test.
* **Nguyên tắc Pipeline:**
    * *Build Once, Deploy Anywhere:* Đóng gói mã nguồn 1 lần duy nhất (Artifact) để đảm bảo tính nhất quán trên mọi môi trường.
    * *Đo lường (DORA Metrics):* Tập trung vào 4 chỉ số vàng: Tần suất triển khai, Thời gian thay đổi (Lead time), Tỷ lệ lỗi (Change Failure Rate), và Thời gian khôi phục (MTTR).

### 3.2. Infrastructure as Code (IaC): Từ ClickOps Sang Code

Chuyển dịch bắt buộc từ thao tác tay trên Console sang quản lý bằng Code để có Version Control và khả năng tái sử dụng:

* **AWS CloudFormation:** Công cụ native, dùng YAML/JSON. Quản lý tài nguyên theo Stack, dọn dẹp sạch sẽ khi xóa.
* **Terraform:** Mã nguồn mở (HCL), tối ưu cho Multi-cloud. Quy trình *Plan -> Apply* giúp xem trước thay đổi, an toàn khi vận hành.
* **AWS CDK:** Dùng ngôn ngữ lập trình hiện đại (Python, Java...) để dựng hạ tầng. Hỗ trợ các Construct (L1-L3) giúp dựng hệ thống phức tạp chỉ với vài dòng code.
* **Drift Detection:** Tính năng quan trọng giúp phát hiện sự sai lệch giữa cấu hình trong Code và thực tế.

### 3.3. Containerization: Lựa Chọn Nền Tảng Phù Hợp

Không có công cụ tốt nhất, chỉ có công cụ phù hợp nhất với nhu cầu:

* **Amazon ECS:** Đơn giản, tích hợp sâu với AWS, dành cho team muốn tập trung vào App thay vì quản lý Cluster.
* **Amazon EKS:** Chuẩn Kubernetes quốc tế, dành cho hệ thống lớn, cần tùy chỉnh sâu hoặc Hybrid-cloud.
* **AWS App Runner:** Giải pháp "Zero-ops", deploy trực tiếp từ Code/Image ra URL HTTPS mà không cần lo về hạ tầng.
* **Compute Options:**
    * *EC2:* Quản lý máy chủ (Kiểm soát cao, vận hành vất vả).
    * *Fargate:* Serverless cho Container (Không cần quản lý OS, chỉ lo chạy App).

### 3.4. Observability: Hơn Cả Monitoring

Chuyển từ câu hỏi "Hệ thống có sống không?" sang "Tại sao hệ thống chậm?":

* **Amazon CloudWatch:** Trung tâm thu thập Metrics (Chỉ số), Logs (Nhật ký) và Alarms (Cảnh báo/Tự động scale).
* **AWS X-Ray (Distributed Tracing):** Giải quyết bài toán "hộp đen" trong Microservices bằng cách vẽ bản đồ đường đi của request, giúp xác định chính xác điểm nghẽn (Latency) hoặc nơi phát sinh lỗi.

---

## 4. Bài Học Và Suy Ngẫm Cá Nhân

Buổi chuyên đề đã tái định hình tư duy của tôi về vai trò của kỹ sư Cloud:

1.  **Từ Ops sang Platform Engineering:** Vai trò hiện đại không phải là người chạy theo deploy thủ công, mà là người xây dựng nền tảng (Platform Builders). Mục tiêu là tạo ra "đường cao tốc" CI/CD an toàn để Developer tự phục vụ (Self-service).
2.  **Kỷ luật vận hành (Operational Discipline):** Sự ổn định đến từ kỷ luật. Nguyên tắc *Immutability* (Bất biến) và việc cấm sửa lỗi thủ công (ClickOps) trên Production là yếu tố sống còn để hệ thống vận hành trơn tru, tránh lỗi con người.
3.  **Tư duy chọn công cụ:** Hiểu rõ ưu nhược điểm của từng công cụ (CloudFormation vs Terraform, ECS vs EKS) giúp tôi đưa ra các quyết định kiến trúc chính xác, tối ưu chi phí và nguồn lực cho dự án.

## 5. Kết Luận

Sự kiện **"DevOps & IaC Mastery"** đã trang bị cho tôi một lộ trình trưởng thành toàn diện:

* **Tư duy:** Hệ thống hóa và đo lường bằng dữ liệu.
* **Công cụ:** Kiểm soát hạ tầng bằng Code (IaC).
* **Vận hành:** Tối ưu hóa bằng Container và Observability.

Đây là những mảnh ghép không thể thiếu để xây dựng và vận hành các hệ thống quy mô lớn, bền vững trên AWS.


