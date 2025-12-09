---
title: "Week 2 Worklog"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Master Amazon EC2 (Elastic Compute Cloud) fundamentals and instance management
* Understand block storage with Amazon EBS and Windows workloads on AWS
* Learn cloud-based development with AWS Cloud9
* Deep dive into Amazon S3 object storage and security best practices
* Explore simplified compute solutions with Amazon Lightsail and container deployment

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Compute Essentials with Amazon EC2** <br> - **Practice:** <br>&emsp; + Analyze instance type families (T3, C5, R5) <br>&emsp; + Launch EC2 instances with Amazon Linux 2023 <br>&emsp; + Configure SSH access and manage Key Pairs | 09/15/2025 | 09/15/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn about **Elastic Block Store (EBS)** <br> - Learn **Windows Workloads on AWS** <br> - **Practice:** <br>&emsp; + Create and attach EBS volumes (gp3) <br>&emsp; + Deploy Windows Server 2022 with IIS <br>&emsp; + Create EBS Snapshots for backup | 09/16/2025 | 09/16/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **AWS Cloud9 Development Environment** <br> - **Practice:** <br>&emsp; + Set up Cloud9 IDE <br>&emsp; + Utilize pre-installed AWS CLI, SAM, and Docker <br>&emsp; + Practice remote code editing via browser | 09/17/2025 | 09/17/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **S3 Fundamentals - Object Storage** <br> - **Practice:** <br>&emsp; + Create S3 buckets and upload objects <br>&emsp; + Configure Static Website Hosting <br>&emsp; + Write Bucket Policies for public access control | 09/18/2025 | 09/18/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Advanced S3 Features and Security Best Practices** <br> - **Practice:** <br>&emsp; + Configure Storage Classes (Standard, IA, Glacier) <br>&emsp; + Set up Lifecycle Policies <br>&emsp; + Enable Versioning and Default Encryption (SSE-S3) <br>&emsp; + Configure Block Public Access | 09/19/2025 | 09/19/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **Amazon Lightsail Simplified Compute** <br> - **Practice:** <br>&emsp; + Deploy WordPress using Lightsail Blueprint <br>&emsp; + Compare Lightsail vs EC2 (cost and features) <br>&emsp; + Understand LAMP stack deployment | 09/20/2025 | 09/20/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Container Deployment with Amazon Lightsail Containers** <br> - **Practice:** <br>&emsp; + Build Docker images for Node.js application <br>&emsp; + Deploy containerized app to Lightsail Container Service <br>&emsp; + Understand container basics before ECS/EKS | 09/21/2025 | 09/21/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 2 Achievements:

* **Mastered Amazon EC2 Compute Service:**
  * Understood instance type families: T3 (Burstable), C5 (Compute Optimized), R5 (Memory Optimized)
  * Successfully launched EC2 instances with Amazon Linux 2023 AMI
  * Configured secure SSH access using Key Pairs (.pem files)
  * Managed instance lifecycle (Start, Stop, Terminate)

* **Practiced Block Storage with Amazon EBS:**
  * Created and attached EBS volumes (gp3 type) to running EC2 instances
  * Performed mount operations on Linux instances
  * Created EBS Snapshots for backup (incremental backup mechanism)
  * Understood EBS persistence independent of EC2 lifecycle

* **Deployed Windows Workloads on AWS:**
  * Launched Windows Server 2022 instances
  * Connected via Remote Desktop Protocol (RDP)
  * Installed and configured IIS Web Server on Windows

* **Set up Cloud-based Development Environment:**
  * Configured AWS Cloud9 IDE in browser
  * Utilized pre-installed tools: AWS CLI, SAM, Docker
  * Experienced remote code editing without opening SSH ports publicly
  * Eliminated "works on my machine" syndrome

* **Deep Understanding of Amazon S3 Object Storage:**
  * Created S3 buckets and uploaded various media files
  * Configured Static Website Hosting for HTML/CSS/JS websites
  * Wrote JSON Bucket Policies for granular access control (s3:GetObject)
  * Implemented S3 Security Best Practices:
    - Enabled Block Public Access at account level
    - Activated Versioning for data protection
    - Configured Default Encryption (SSE-S3)
    - Set up Lifecycle Policies (auto-transition to Glacier after 30 days)

* **Explored Simplified Compute Solutions:**
  * Deployed WordPress using Amazon Lightsail Blueprint (LAMP stack)
  * Compared Lightsail vs EC2 trade-offs (simplicity vs control)
  * Built Docker images for Node.js applications locally
  * Deployed containerized applications to Lightsail Container Service

* **Acquired hands-on experience with:**
  * Multiple compute options: EC2, Lightsail, Cloud9
  * Storage solutions: EBS (block), S3 (object)
  * Both Linux and Windows workloads on AWS
  * Basic containerization concepts preparing for ECS/EKS
  * ...

* Acquired the ability to connect between the web interface and CLI to manage AWS resources in parallel.
* ...
