---
title: "Bản đề xuất"
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Hệ thống cho thuê xe điện tại điểm cố định  
## Phần mềm cho thuê và trả xe điện tại các điểm cố định – Giải pháp di chuyển xanh cho đô thị thông minh  

### 1. Tóm tắt điều hành  
Hệ thống EV Station-based Rental System được phát triển nhằm cung cấp một nền tảng tất cả trong một cho việc thuê và quản lý xe điện. Hệ thống tích hợp việc đặt xe theo thời gian thực, thanh toán và quản lý điểm thuê thông qua giải pháp đám mây thống nhất.
Ứng dụng bao gồm app di động React Native và backend Spring Boot triển khai trên AWS ECS Fargate, với PostgreSQL (RDS) và Redis (ElastiCache) để lưu trữ dữ liệu và tăng tốc độ truy xuất. Xác thực người dùng được quản lý qua Amazon Cognito, trong khi phân phối nội dung toàn cầu được tối ưu bằng CloudFront. Thiết kế theo AWS Well-Architected Framework giúp nền tảng đảm bảo khả năng mở rộng, độ sẵn sàng cao, bảo mật, đồng thời tối ưu chi phí vận hành. 

### 2. Tuyên bố vấn đề  
*Vấn đề hiện tại*  
Các dịch vụ thuê xe điện hiện nay còn phân mảnh, buộc người dùng phải sử dụng nhiều ứng dụng khác nhau để tìm, đặt và quản lý xe tại các điểm cố định. Điều này gây ra sự bất tiện, hiệu suất chậm và trải nghiệm thiếu tin cậy — người dùng thường đến các điểm thuê “không khả dụng” hoặc “ngoại tuyến”, dẫn đến bức xúc và mất niềm tin.

Đối với chủ xe và nhà vận hành, việc quản lý đội xe, điều phối đơn thuê và theo dõi bảo trì thủ công gây ra nhiều bất cập, giảm hiệu quả vận hành và mất doanh thu. Hiện chưa có nền tảng thống nhất và thời gian thực kết nối người thuê, chủ xe và nhà vận hành điểm thuê. 

*Giải pháp*  
Hệ thống cho thuê và trả xe điện tại điểm cố định hợp nhất việc thuê và trả xe vào một nền tảng đám mây duy nhất. Hệ thống được xây dựng với React Native cho di động và Spring Boot cho backend, cung cấp tính năng đặt xe theo thời gian thực, theo dõi phương tiện và tích hợp thanh toán.

Các dịch vụ AWS cốt lõi bao gồm ECS Fargate cho xử lý tính toán, RDS PostgreSQL cho lưu trữ dữ liệu, ElastiCache cho hiệu năng truy xuất nhanh, API Gateway và Cognito cho truy cập bảo mật, và CloudFront cho phân phối nội dung toàn cầu. Nền tảng hỗ trợ cả hình thức quản lý đội xe và chia sẻ xe P2P, cung cấp giao diện tập trung cho người dùng và nhà vận hành để quản lý việc thuê xe hiệu quả, an toàn và dễ mở rộng.

*Lợi ích và hoàn vốn đầu tư (ROI)*
Nền tảng loại bỏ sự phân mảnh ứng dụng và thao tác thủ công, mang lại trải nghiệm thống nhất, tự động cho cả người thuê và chủ xe. Dữ liệu thời gian thực đảm bảo độ tin cậy và minh bạch về tình trạng xe và điểm thuê.

Thiết kế theo AWS Well-Architected Framework giúp tối ưu chi phí vận hành thông qua mô hình serverless, trả theo mức sử dụng, đồng thời duy trì khả năng mở rộng và độ sẵn sàng 99,99%. Trong vòng 12–24 tháng, nền tảng dự kiến đạt 50.000+ người dùng hoạt động hàng tháng, hợp tác với 200+ điểm thuê, và mang lại hiệu quả đáng kể về thời gian, chi phí và vận hành cho cả người dùng và nhà vận hành. 

### 3. Kiến trúc giải pháp  
Nền tảng VoltGo được xây dựng trên kiến trúc AWS serverless an toàn, linh hoạt và được quản lý hoàn toàn. Các dịch vụ backend được triển khai trên Amazon ECS Fargate với image container được lưu trữ trong Amazon ECR. Hệ thống sử dụng Aurora PostgreSQL Serverless v2 làm cơ sở dữ liệu quan hệ chính và ElastiCache Serverless (Valkey/Redis) để caching và quản lý session với độ trễ thấp. Tất cả các dịch vụ được vận hành trong private subnet trên nhiều Availability Zones và được truy cập an toàn thông qua Amazon API Gateway tích hợp với Application Load Balancer qua AWS PrivateLink. Xác thực người dùng được quản lý bằng Amazon Cognito với hỗ trợ JWT và MFA. Phần frontend được lưu trữ trên Amazon S3 và phân phối toàn cầu thông qua Amazon CloudFront, kết hợp với AWS WAF và ACM để bảo mật SSL/TLS. Các tính năng AI được triển khai bằng Amazon Bedrock thông qua AWS Lambda, trong khi Amazon Location Service được sử dụng để hiển thị bản đồ và tìm kiếm trạm gần nhất. Việc giám sát và ghi log được tập trung tại Amazon CloudWatch, và toàn bộ hạ tầng được triển khai tự động bằng Terraform nhằm đảm bảo tính nhất quán và dễ mở rộng.

![Voltgo Station Architecture](/images/2-Proposal/voltgo_architecure.png)

### AWS Services Used
- **Amazon ECS Fargate**: Serverless container orchestration for backend microservices.
- **Amazon PostgreSQL**: Relational database.
- **Amazon ElastiCache Serverless (Valkey)**: In-memory caching for low-latency data access.
- **Amazon API Gateway**: Secure REST API entry point integrated via PrivateLink.
- **Amazon Cognito**: User authentication and authorization with JWT and MFA.
- **Amazon CloudFront + S3**: Global content delivery and static hosting with WAF protection.
- **Amazon CloudWatch**: Unified monitoring, logging, and alerting for all services.
- **Amazon ACM**: Edge-level security and SSL/TLS certificate management.
- **Amazon Application Load Balancer**: Route traffic forward to target group
- **Amazon Location Service**: Providing map and places (index) for frontend allow user search and check station nearly.
- **Amazon Bedrock**: Handling chatting support user for QA and find nearby station base on user's location
- **Amazon EC2**: Bastion Server connect RDS to config extension and running script
- **Amazon Lambda**: Bridge connect with Bedrock to handle api in QA from user
- **Amazon ECR**: Repository store image for ecs task

### 4. Triển khai kỹ thuật  
*Các giai đoạn triển khai*  
Dự án gồm 2 phần — thiết lập trạm thời tiết biên và xây dựng nền tảng thời tiết — mỗi phần trải qua 4 giai đoạn:  
1. *Nghiên cứu và vẽ kiến trúc*: Nghiên cứu Raspberry Pi với cảm biến ESP32 và thiết kế kiến trúc AWS Serverless (1 tháng trước kỳ thực tập).  
2. *Tính toán chi phí và kiểm tra tính khả thi*: Sử dụng AWS Pricing Calculator để ước tính và điều chỉnh (Tháng 1).  
3. *Điều chỉnh kiến trúc để tối ưu chi phí/giải pháp*: Tinh chỉnh (ví dụ tối ưu Lambda với Next.js) để đảm bảo hiệu quả (Tháng 2).  
4. *Phát triển, kiểm thử, triển khai*: Lập trình Raspberry Pi, AWS services với CDK/SDK và ứng dụng Next.js, sau đó kiểm thử và đưa vào vận hành (Tháng 2–3).  

*Yêu cầu kỹ thuật*  
- *Trạm thời tiết biên*: Cảm biến (nhiệt độ, độ ẩm, lượng mưa, tốc độ gió), vi điều khiển ESP32, Raspberry Pi làm thiết bị biên. Raspberry Pi chạy Raspbian, sử dụng Docker để lọc dữ liệu và gửi 1 MB/ngày/trạm qua MQTT qua Wi-Fi.  
- *Nền tảng thời tiết*: Kiến thức thực tế về AWS Amplify (lưu trữ Next.js), Lambda (giảm thiểu do Next.js xử lý), AWS Glue (ETL), S3 (2 bucket), IoT Core (gateway và rules), và Cognito (5 người dùng). Sử dụng AWS CDK/SDK để lập trình (ví dụ IoT Core rules tới S3). Next.js giúp giảm tải Lambda cho ứng dụng web fullstack.  

### 5. Lộ trình & Mốc triển khai  
- *Trước thực tập (Tháng 0)*: 1 tháng lên kế hoạch và đánh giá trạm cũ.  
- *Thực tập (Tháng 1–3)*:  
    - Tháng 1: Học AWS và nâng cấp phần cứng.  
    - Tháng 2: Thiết kế và điều chỉnh kiến trúc.  
    - Tháng 3: Triển khai, kiểm thử, đưa vào sử dụng.  
- *Sau triển khai*: Nghiên cứu thêm trong vòng 1 năm.  

### 6. Ước tính ngân sách  
Có thể xem chi phí trên [AWS Pricing Calculator](https://calculator.aws/#/estimate?id=621f38b12a1ef026842ba2ddfe46ff936ed4ab01)  
Hoặc tải [tệp ước tính ngân sách](../attachments/budget_estimation.pdf).  

*Chi phí hạ tầng*  
- AWS Lambda: 0,00 USD/tháng (1.000 request, 512 MB lưu trữ).
---
title: "Proposal"
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# The EV Station-based Rental System
## Electric Vehicle Rental and Return Software at Fixed Stations – A Green Mobility Solution for Smart Cities

### 1. Executive Summary
The EV Station-based Rental System is developed to provide an all-in-one platform for electric vehicle rental and charging management. It integrates real-time rental, payment, and charging station access through a unified cloud-native solution. The system features a React Native mobile app and a Spring Boot backend deployed on AWS ECS Fargate, with PostgreSQL (RDS) and Redis (ElastiCache) for data and caching. User authentication is managed via Amazon Cognito, and global delivery is optimized using CloudFront. Designed under the AWS Well-Architected Framework, the platform ensures scalability, high availability, and security while maintaining cost efficiency.

### 2. Problem Statement
### What’s the Problem?
Current electric vehicle (EV) rental services are fragmented, requiring users to switch between multiple apps to locate, book, and manage rentals at fixed points. This creates inconvenience, slow performance, and unreliable experiences — users often arrive at “unavailable” or “offline” rental points, leading to frustration and loss of trust.

For vehicle owners and operators, manual fleet management, booking coordination, and maintenance tracking result in operational inefficiencies and lost revenue. Currently, there is no unified, real-time platform connecting renters, vehicle owners, and rental point operators.

### The Solution
The EV Station-based Rental System consolidates EV rental and return at fixed points into a single, cloud-native platform. Built with React Native for mobile and Spring Boot for backend, the system delivers real-time booking, vehicle tracking, and payment integration.

Key AWS services include ECS Fargate for compute, RDS PostgreSQL for data storage, ElastiCache for low-latency performance, API Gateway and Cognito for secure access, and CloudFront for global content delivery. The platform supports both fleet-based and peer-to-peer (P2P) vehicle registration, providing a centralized interface for users and operators to manage rentals efficiently, securely, and at scale.

### Benefits and Return on Investment
The platform eliminates manual coordination and fragmented applications, offering a unified, automated experience for renters and fleet owners. Real-time data ensures reliability and transparency regarding vehicle availability and rental point status.

Designed under the AWS Well-Architected Framework, the system minimizes operational costs with a serverless, pay-per-use model while maintaining scalability and 99.99% uptime. Within 1 months, the platform is projected to reach 1,000+ monthly active users, onboard 200+ rental points, and deliver significant time, cost, and operational efficiencies for both users and operators.

### 3. Solution Architecture
The VoltGo platform is built on a secure, scalable, and fully managed AWS serverless architecture. Backend services are deployed on Amazon ECS Fargate with container images stored in Amazon ECR. The system uses Aurora PostgreSQL Serverless v2 for the main relational database and ElastiCache Serverless (Valkey/Redis) for low-latency caching and session management. All services operate within private subnets across multiple Availability Zones and are securely exposed through Amazon API Gateway integrated with Application Load Balancer via AWS PrivateLink. User authentication is handled by Amazon Cognito with JWT and MFA support. The frontend is hosted on Amazon S3 and delivered globally through Amazon CloudFront with AWS WAF and ACM SSL/TLS protection. AI-powered features are implemented using Amazon Bedrock integrated via AWS Lambda, while Amazon Location Service provides map and nearby station search functionality. Monitoring and logging are centralized in Amazon CloudWatch, and the entire infrastructure is provisioned using Terraform for automated and consistent deployments.


![Voltgo Platform Architecture](/images/2-Proposal/voltgo_architecture.png)

### AWS Services Used
- **Amazon ECS Fargate**: Serverless container orchestration for backend microservices.
- **Amazon PostgreSQL**: Relational database.
- **Amazon ElastiCache Serverless (Valkey)**: In-memory caching for low-latency data access.
- **Amazon API Gateway**: Secure REST API entry point integrated via PrivateLink.
- **Amazon Cognito**: User authentication and authorization with JWT and MFA.
- **Amazon CloudFront + S3**: Global content delivery and static hosting with WAF protection.
- **Amazon CloudWatch**: Unified monitoring, logging, and alerting for all services.
- **Amazon ACM**: Edge-level security and SSL/TLS certificate management.
- **Amazon Application Load Balancer**: Route traffic forward to target group
- **Amazon Location Service**: Providing map and places (index) for frontend allow user search and check station nearly.
- **Amazon Bedrock**: Handling chatting support user for QA and find nearby station base on user's location
- **Amazon EC2**: Bastion Server connect RDS to config extension and running script
- **Amazon Lambda**: Bridge connect with Bedrock to handle api in QA from user
- **Amazon ECR**: Repository store image for ecs task

### Component Design
- **Frontend**:React web application hosted on Amazon S3 and delivered via CloudFront, secured ACM SSL/TLS certificates.
- **API Layer**: Amazon API Gateway provides the public API endpoint.
- **Compute Layer**:  Amazon ECS Fargate runs containerized across multiple Availability Zones, scaling automatically based on CPU and memory utilization.
- **Database Layer**:Amazon PostgreSQL stores relational data for high availability and automated scaling.
- **Caching Layer**: Amazon ElastiCache Serverless (Redis) caches session and booking data to reduce database load and improve response time.
- **Authentication**: Amazon Cognito handles user registration, login, and JWT-based authorization with optional MFA support.
- **Storage**: Amazon S3 manages static assets and user uploads, accessible only through CloudFront via Origin Access Control (OAC).
- **Monitoring & Security**: Amazon CloudWatch tracks logs and performance metrics, while AWS Secrets Manager securely stores credentials with automatic rotation.

### 4. Technical Implementation
**Implementation Phases**
This project has two main parts—developing the backend locally and deploying it to the AWS cloud—each following four key phases:
   - 1.Build and Design Architecture:
 Develop and test backend services locally using Docker Compose, PostgreSQL, and Redis. Design the AWS serverless architecture including ECS Fargate, Aurora Serverless, ElastiCache, and API Gateway with PrivateLink connections. (Pre-deployment phase)
   - 2.Estimate Cost and Validate Feasibility:
 Use AWS Pricing Calculator to estimate the monthly cost of ECS tasks, Aurora capacity units, and CloudFront bandwidth. Adjust design decisions to ensure cost-effectiveness and smooth migration.
   - 3.Configure and Deploy Infrastructure:
 Build and deploy cloud infrastructure using Terraform for IaC. Configure VPC, ECS, Aurora, ElastiCache, Cognito, and CloudFront. Validate IAM roles, networking, and private-only access via VPC Endpoints. 
   - 4.Test, Optimize, and Release:
 Deploy Dockerized services to ECS Fargate, test API Gateway → PrivateLink → NLB → ECS flow, and verify database connections. Enable CloudWatch monitoring, auto-scaling, and WAF protection. Optimize scaling thresholds and document final architecture. 


**Technical Requirements**
- Backend Services:
 Node.js or Spring Boot microservices for Auth, Booking, and Payment, containerized with Docker and deployed to ECS Fargate (2–10 tasks, auto-scaling).
- Database Layer:
 Amazon Aurora PostgreSQL Serverless v2 with writer and reader instances, supporting automatic scaling and multi-AZ high availability.
- Caching Layer:
 Amazon ElastiCache Serverless (Redis 7.1) for session caching and frequently accessed data.
- Authentication:
 Amazon Cognito manages user registration, JWT-based authentication, and optional MFA, integrated with API Gateway.
- Storage & Content Delivery:
 Frontend hosted on Amazon S3 and distributed via CloudFront, protected by AWS WAF and ACM SSL/TLS certificates.
- Secrets & Monitoring:
 AWS Secrets Manager for storing credentials (DB, Redis, JWT keys) with 30-day rotation. Amazon CloudWatch for logging, metrics, and scaling alarms.


### 5. Timeline & Milestones
**Project Timeline**
- Phase 1: Foundation & Design (Weeks 1-2)
  - Week 1: Finalize MVP scope (P0 User Stories), define user flows, and approve the AWS architecture.
  - Week 2: FE Lead finalizes UI/UX mockups. Backend provisions core AWS (VPC, S3, ECR, Aurora).
- Phase 2: Core MVP Development (Weeks 3-8)
- Weeks 3-4: Backend builds User Auth (Cognito) & core APIs (API Gateway, ECS).
    - Weeks 5-6: All teams (FE/BE/Mobile) build core screens (Login, Search, Details) and the Booking Engine APIs.
    - Weeks 7-8: Integration of KYC flow (Lambda, Textract, Rekognition) and Payment Gateway integration.
- Phase 3: Testing & UAT (Weeks 9-10)
    - Week 9: Full End-to-End (E2E) testing. QA is performed by the 5-person dev team, as no dedicated QA is allocated.
    - Week 10: Stakeholder User Acceptance Testing (UAT) and final critical bug fixing.
- Phase 4: Launch (Week 11)
    - Week 11: Production deployment, Go-live, and intensive Hypercare monitoring via CloudWatch. 


### 6. Budget Estimation
This budget estimate is based on the provided AWS architecture diagram and the "cheapest possible" MVP launch strategy, maximizing Free Tier usage.

### Infrastructure Costs
- AWS Services (Monthly Estimate):
    - Amazon Route 53: $0.50/month (1 hosted zone).
    - AWS WAF: $6.00/month (1 WebACL + 1 Rule + minimal requests).
    - AWS S3 Standard: $0.00/month (Stays within 5GB Always Free tier).
    - Amazon CloudFront: $0.00/month (Stays within 1TB/10M request Always Free tier).
    - AWS Cognito: $0.00/month (Stays within 10,000 MAU free tier).
    - Amazon API Gateway: $0.00/month (Stays within 1M request 12-month free tier).
    - AWS Lambda: $0.00/month (Stays within 1M request Always Free tier).
    - Amazon Textract/Rekognition: $0.00/month (Stays within 12-month free tier for KYC).
    - Application Load Balancer: $17.52/month (1 ALB, minimal processing).
    - VPC Endpoint (PrivateLink): $7.30/month (1 Endpoint, 1 AZ, 1GB data).
    - Amazon ECS on Fargate: ~$20.00/month (Assumes 2 minimal 24/7 containers, e.g., 0.25 vCPU/0.5GB RAM).
    - Amazon Aurora Serverless v2: ~$25.00/month (Minimal ACUs, configured to scale to near-zero).
    - Amazon ElastiCache Serverless: ~$10.00/month (Minimal usage).
    - Amazon CloudWatch: $0.00/month (Stays within 5GB log Always Free tier).
    - Amazon ECR: ~$0.10/month (Minimal storage over 500MB free tier).

Total: ~$86.42/month, ~$1,037.04/12 months


### 7. Risk Assessment
#### Risk Matrix
- System Downtime: High impact, medium probability.
- Data Sync Errors (Between Stations & Server): Medium impact, high probability.
- OCR Verification Failure: Medium impact, medium probability.
- Vehicle Shortage or Low Battery at Stations: High impact, high probability.
- Operational Mistakes by Staff: Medium impact, medium probability.
- Cost Overruns: Medium impact, low probability.

#### Mitigation Strategies
- System: Use load-balanced cloud servers with auto-scaling and failover backup.
- Data Sync: Implement offline caching and periodic background synchronization.
- OCR Verification: Combine AI-based ID recognition with manual approval option.
- Vehicle Management: Real-time tracking of battery and vehicle status; predictive restocking via analytics.
- Staff Operations: Provide training and digital checklists to reduce human error.
- Cost: Set up cloud cost monitoring and optimization alerts.

#### Contingency Plans
- Enable offline mode for station staff when Internet is unavailable.
- Activate backup servers in case of major downtime.
- Provide manual check-in/out workflow for rentals during system outages.
- Deploy mobile maintenance team to handle vehicle or battery issues at stations.
- Suspend or limit reservations dynamically if vehicle supply falls below safe threshold.

### 8. Expected Outcomes
#### Technical Improvements: 
- Real-time monitoring of all EV stations and rental status.
- Automated verification and e-contract signing replace manual paperwork.
- Centralized dashboard for admins to manage fleet, customers, and staff.
- System scalable to 20+ rental stations in the next deployment phase.
#### Long-term Value
- Establishes a reliable EV mobility infrastructure for urban areas.
- Builds data foundation for future AI-powered demand forecasting.
- Enables integration with smart city and green transportation networks.
- Serves as a reusable platform for expanding to nationwide EV-sharing projects.
#### Short to Medium-term Benefits
- Faster customer onboarding (from 15 mins → <5 mins).
- Increased fleet utilization rate by 30% through data-driven scheduling.
- Improved accuracy of rental records and payment reconciliation.
- Enhanced user satisfaction via seamless booking and transparent billing.