---
title: "Week 4 Worklog"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Automate system scalability with EC2 Auto Scaling
* Implement comprehensive monitoring with Amazon CloudWatch
* Master DNS management with Amazon Route 53
* Optimize global content delivery with Amazon CloudFront and Lambda@Edge
* Learn command line automation with AWS CLI
* Understand advanced networking with VPC Peering

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **EC2 Auto Scaling** <br> - **Practice:** <br>&emsp; + Create Launch Templates with AMI, Instance Type, Security Group <br>&emsp; + Configure Auto Scaling Groups (Min=2, Max=4, Desired=2) <br>&emsp; + Set up Target Tracking Scaling Policy (CPU 50%) <br>&emsp; + Perform stress test to observe scale-out | 09/29/2025 | 09/29/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Amazon CloudWatch Monitoring** <br> - **Practice:** <br>&emsp; + Monitor standard metrics (CPU, Disk I/O, Network) <br>&emsp; + Install CloudWatch Agent for custom metrics (Memory) <br>&emsp; + Create Alarms with SNS notifications <br>&emsp; + Configure alarm for CPU > 80% for 5 minutes | 09/30/2025 | 09/30/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **CloudWatch Logs and Dashboards** <br> - **Practice:** <br>&emsp; + Push application logs to CloudWatch Logs <br>&emsp; + Create unified Dashboard for Web/DB/Cache health <br>&emsp; + Explore Grafana integration for advanced visualization | 10/01/2025 | 10/01/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **Amazon Route 53 DNS Management** <br> - **Practice:** <br>&emsp; + Create Hosted Zones <br>&emsp; + Configure Failover Routing with Health Checks <br>&emsp; + Set up Latency-based Routing <br>&emsp; + Implement automatic DNS failover to S3 maintenance page | 10/02/2025 | 10/02/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Amazon CloudFront CDN** <br> - **Practice:** <br>&emsp; + Deploy CloudFront distribution for S3 content <br>&emsp; + Configure Origin Access Control (OAC) <br>&emsp; + Customize caching policies and TTL <br>&emsp; + Optimize global content delivery with Edge Locations | 10/03/2025 | 10/03/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **CloudFront and Lambda@Edge** <br> - **Practice:** <br>&emsp; + Write Lambda functions running at Edge Locations <br>&emsp; + Modify HTTP headers dynamically <br>&emsp; + Implement A/B testing without origin server requests <br>&emsp; + Minimize latency with edge computing | 10/04/2025 | 10/04/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **AWS CLI and VPC Peering** <br> - **Practice:** <br>&emsp; + Write Bash scripts for automation using AWS CLI <br>&emsp; + Auto-stop Dev instances <br>&emsp; + Connect two VPCs via VPC Peering <br>&emsp; + Week review and integration | 10/05/2025 | 10/05/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 4 Achievements:

* **Mastered Automatic Scalability with EC2 Auto Scaling:**
  * Created Launch Templates defining complete instance configuration
  * Configured Auto Scaling Groups with Min/Max/Desired capacity
  * Implemented Target Tracking Scaling Policy (maintain 50% CPU)
  * Successfully performed stress testing to observe automatic scale-out
  * Integrated ASG with Application Load Balancer for seamless traffic distribution
  * Achieved self-healing infrastructure (automatic instance replacement)

* **Implemented Comprehensive Monitoring System:**
  * Monitored standard EC2 metrics: CPU, Disk I/O, Network throughput
  * Deployed CloudWatch Agent for custom metrics (Memory Usage)
  * Created CloudWatch Alarms with SNS email notifications
  * Pushed application logs (/var/log/httpd) to CloudWatch Logs
  * Built unified Dashboard visualizing system health across all tiers
  * Explored advanced visualization with CloudWatch-Grafana integration

* **Achieved DNS Mastery with Amazon Route 53:**
  * Created and managed Hosted Zones for domain management
  * Configured multiple routing policies:
    - Simple Routing: Basic DNS resolution
    - Failover Routing: Automatic failover with Health Checks
    - Latency-based Routing: Direct users to lowest-latency region
  * Implemented intelligent failover to S3 static maintenance page

* **Optimized Global Content Delivery:**
  * Deployed Amazon CloudFront CDN with S3 origin
  * Configured Origin Access Control (OAC) for secure S3 access
  * Customized caching behavior with TTL settings
  * Leveraged Edge Locations for global low-latency access
  * Implemented Lambda@Edge for:
    - Dynamic HTTP header modification
    - A/B testing at the edge
    - Request routing without origin server involvement
  * Reduced latency and improved user experience worldwide

* **Advanced CLI Automation Skills:**
  * Wrote Bash automation scripts using AWS CLI
  * Automated operational tasks (e.g., auto-stop Dev instances by tags)
  * Mastered --query and --filter for precise JSON data extraction
  * Transitioned from manual Console operations to programmatic control
  * Developed skills essential for large-scale infrastructure management

* **Expanded Network Architecture Knowledge:**
  * Implemented VPC Peering for inter-VPC communication
  * Updated Route Tables to enable private network connectivity
  * Understood non-transitive peering limitations
  * Avoided internet gateway for VPC-to-VPC traffic (cost and security benefits)

* **Completed Month 1 Milestone:**
  * Built production-ready 3-tier architecture with:
    - Auto-scaling Web tier
    - Self-healing capabilities
    - Comprehensive monitoring (CloudWatch)
    - Global performance optimization (CloudFront/Route 53)
    - Automated operations (AWS CLI/ASG)
  * Achieved Well-Architected Framework pillars: Reliability, Performance, and Operational Excellence

* Acquired the ability to connect between the web interface and CLI to manage AWS resources in parallel.
* ...
