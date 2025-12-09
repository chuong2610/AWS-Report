---
title: "Week 8 Worklog"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Master cost optimization and FinOps practices for cloud financial management
* Analyze spending patterns with AWS Cost Explorer and Cost & Usage Reports
* Implement right-sizing recommendations to eliminate resource waste
* Understand commitment-based pricing with Savings Plans and Reserved Instances
* Manage service quotas proactively to prevent deployment failures
* Build centralized network architecture with AWS Transit Gateway
* Monitor network traffic with VPC Flow Logs for security and troubleshooting
* Delegate billing access with proper IAM controls
* Automate EBS lifecycle management for backup optimization

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Cost Visualization and Analytics** <br> - **Practice:** <br>&emsp; + Analyze costs by Service, Region, and Tags with Cost Explorer <br>&emsp; + Enable Cost and Usage Report (CUR) export to S3 <br>&emsp; + Create hourly granular cost reports <br>&emsp; + Identify top spending services and resources | 10/27/2025 | 10/27/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Advanced Cost Analytics with Athena** <br> - **Practice:** <br>&emsp; + Query CUR data using AWS Glue and Athena <br>&emsp; + Analyze data transfer costs between specific instances <br>&emsp; + Create custom cost allocation queries <br>&emsp; + Generate detailed cost breakdowns by hour/day | 10/28/2025 | 10/28/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **Right-Sizing with EC2 Resource Optimization** <br> - **Practice:** <br>&emsp; + Use AWS Compute Optimizer for instance recommendations <br>&emsp; + Analyze 14-day historical utilization data <br>&emsp; + Identify over-provisioned instances <br>&emsp; + Install CloudWatch Agent for memory metrics <br>&emsp; + Implement downsizing recommendations (m5.large → m5.medium) | 10/29/2025 | 10/29/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **Cost Savings with Savings Plans and Reserved Instances** <br> - **Practice:** <br>&emsp; + Compare EC2 Instance Savings Plans vs Compute Savings Plans <br>&emsp; + Analyze commitment flexibility vs discount rates <br>&emsp; + Plan 1-year commitment for base workload <br>&emsp; + Calculate potential savings (up to 72%) <br>&emsp; + Purchase Savings Plan for production workloads | 10/30/2025 | 10/30/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Managing Quotas with Service Quotas** <br> - **Practice:** <br>&emsp; + Review current service limits (vCPU, VPC, EIP) <br>&emsp; + Set up CloudWatch alarms for quota utilization (80% threshold) <br>&emsp; + Request quota increases proactively <br>&emsp; + Prevent deployment failures due to limits | 10/31/2025 | 10/31/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **Centralized Network Management with Transit Gateway** <br> - **Practice:** <br>&emsp; + Replace mesh VPC Peering with hub-and-spoke model <br>&emsp; + Connect 3 VPCs and 1 VPN to Transit Gateway <br>&emsp; + Configure Transit Gateway route tables <br>&emsp; + Implement network segmentation (Dev/Prod isolation) <br>&emsp; + Allow Shared Services VPC access from all environments | 11/01/2025 | 11/01/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Network Monitoring and Billing Delegation** <br> - **Practice:** <br>&emsp; + Enable VPC Flow Logs for traffic analysis <br>&emsp; + Create IAM roles for finance team <br>&emsp; + Grant billing access <br>&emsp; + Review week 8 achievements | 11/02/2025 | 11/02/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 8 Achievements:

* **Mastered Cost Visualization and Analytics:**
  * Analyzed spending patterns by Service, Region, and custom Tags
  * Enabled Cost and Usage Report (CUR) for detailed cost data export
  * Generated hourly granular cost reports exported to S3
  * Identified top spending services and cost optimization opportunities
  * Created cost allocation tracking for projects and teams
  * Established FinOps foundation for continuous cost management

* **Implemented Advanced Cost Analysis with Athena:**
  * Used AWS Glue to catalog CUR data in S3
  * Queried complex cost patterns with Amazon Athena SQL
  * Analyzed data transfer costs between specific instances
  * Created custom cost allocation reports by hour and day
  * Answered detailed cost questions: "How much did data transfer between two instances cost?"
  * Achieved granular cost visibility for optimization decisions

* **Optimized Resources with Right-Sizing:**
  * Leveraged AWS Compute Optimizer for instance recommendations
  * Analyzed 14-day historical CPU, memory, and network utilization
  * Identified over-provisioned instances wasting resources
  * Installed CloudWatch Agent for accurate memory metrics
  * Implemented downsizing: m5.large → m5.medium for underutilized workloads
  * Achieved 30-50% cost savings on compute resources

* **Maximized Savings with Commitment-Based Pricing:**
  * Compared EC2 Instance Savings Plans (highest discount, least flexibility)
  * Evaluated Compute Savings Plans (flexibility across EC2/Fargate/Lambda)
  * Planned 1-year commitment for predictable base workload
  * Calculated potential savings: up to 72% vs On-Demand pricing
  * Purchased Savings Plans for production workloads
  * Balanced cost savings with workload flexibility requirements

* **Proactively Managed Service Quotas:**
  * Reviewed current service limits: vCPU, VPC, Elastic IPs, etc.
  * Set up CloudWatch Alarms for quota utilization at 80% threshold
  * Submitted quota increase requests before reaching limits
  * Prevented deployment failures and business disruptions
  * Established proactive capacity planning process
  * Avoided emergency quota increase requests

* **Built Centralized Network with Transit Gateway:**
  * Replaced complex mesh VPC Peering with hub-and-spoke architecture
  * Connected 3 VPCs (Dev/Staging/Prod) and 1 VPN to Transit Gateway
  * Configured Transit Gateway route tables for traffic control
  * Implemented network segmentation: Dev cannot access Prod
  * Enabled all environments to access Shared Services VPC
  * Simplified network management and reduced peering complexity

* **Enhanced Network Visibility with VPC Flow Logs:**
  * Enabled Flow Logs for comprehensive traffic analysis
  * Debugged connection issues by analyzing ACCEPT/REJECT status
  * Identified Security Groups and NACLs blocking traffic
  * Detected network anomalies and suspicious traffic patterns
  * Improved security posture with network monitoring
  * Reduced mean time to resolution (MTTR) for network issues

* **Implemented Billing Access Delegation:**
  * Created IAM roles with billing-only permissions for finance team
  * Granted cost dashboard access without technical resource permissions
  * Enforced separation of duties principle
  * Enabled finance team to analyze costs independently
  * Maintained security while improving financial visibility
  * Achieved compliance with organizational governance requirements

* **Automated EBS Lifecycle Management:**
  * Configured Data Lifecycle Manager for automated snapshot creation
  * Set retention policies: keep last 7 days, automatically delete older backups
  * Scheduled snapshot creation during low-usage windows
  * Reduced storage costs by eliminating manual snapshot management
  * Ensured consistent backup coverage without human error
  * Improved backup reliability and cost efficiency

* **Deployed Backup Anomaly Detection:**
  * Enabled anomaly detection for EBS backup monitoring
  * Identified unusual backup patterns indicating potential issues
  * Detected early signs of ransomware or system failures
  * Configured automated alerts for backup anomalies
  * Enhanced data protection with intelligent monitoring
  * Achieved proactive incident response for backup systems

* **Completed Cost Optimization and Advanced Networking Milestone:**
  * Mastered FinOps practices for cloud financial management
  * Achieved 30-70% cost savings through right-sizing and commitments
  * Built scalable, centralized network architecture
  * Implemented comprehensive cost visibility and governance
  * Established automated backup lifecycle and anomaly detection
  * Ready for containerization and modernization challenges in Month 3
  * Transitioned from "building and securing" to "optimizing and modernizing"

