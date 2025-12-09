---
title: "Week 5 Worklog"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Eliminate manual operations with operational thinking and Infrastructure as Code
* Master AWS Systems Manager for fleet management
* Learn secure server access with Session Manager (no SSH required)
* Deep dive into CloudFormation and AWS CDK for infrastructure automation
* Implement resource organization with Tags and Resource Groups
* Apply Attribute-Based Access Control (ABAC) with IAM and Tags

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **AWS Systems Manager (SSM)** <br> - **Practice:** <br>&emsp; + Configure IAM Role with AmazonSSMManagedInstanceCore <br>&emsp; + Use Run Command to execute shell commands on multiple instances <br>&emsp; + Collect software inventory across fleet for audit | 10/06/2025 | 10/06/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Session Manager for Secure Access** <br> - **Practice:** <br>&emsp; + Access instances without SSH/RDP ports <br>&emsp; + Log sessions to S3 and CloudWatch Logs <br>&emsp; + Implement secure server access | 10/07/2025 | 10/07/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **CloudFormation Infrastructure as Code** <br> - **Practice:** <br>&emsp; + Write YAML templates for VPC and EC2 <br>&emsp; + Use Change Sets for safe updates <br>&emsp; + Implement Drift Detection | 10/08/2025 | 10/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **AWS CDK for Advanced Infrastructure** <br> - **Practice:** <br>&emsp; + Use TypeScript/Python for infrastructure <br>&emsp; + Leverage high-level constructs <br>&emsp; + Build custom reusable constructs | 10/09/2025 | 10/09/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Resource Organization with Tags** <br> - **Practice:** <br>&emsp; + Implement tagging strategy <br>&emsp; + Create Resource Groups <br>&emsp; + Track costs by tags | 10/10/2025 | 10/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **ABAC with IAM and Tags** <br> - **Practice:** <br>&emsp; + Implement Attribute-Based Access Control <br>&emsp; + Use tags for access policies <br>&emsp; + Review week 5 achievements | 10/11/2025 | 10/11/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - **Week Review and Practice** <br>&emsp; + Review operational automation concepts <br>&emsp; + Practice IaC skills <br>&emsp; + Prepare for next week | 10/12/2025 | 10/12/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 5 Achievements:

* **Mastered AWS Systems Manager for Fleet Management:**
  * Configured IAM Role with AmazonSSMManagedInstanceCore policy
  * Executed Run Command to manage multiple instances simultaneously
  * Automated software inventory collection across entire fleet
  * Eliminated need for individual SSH connections to each server
  * Implemented centralized patch management and compliance tracking
  * Achieved scalable operational efficiency for large instance fleets

* **Secured Server Access with Session Manager:**
  * Deployed Remote Server Access without SSH/RDP ports
  * Closed port 22 on Security Groups for enhanced security
  * Accessed instances via HTTPS protocol with IAM authentication
  * Logged all session activity to S3 and CloudWatch Logs for audit compliance
  * Implemented gold standard for secure server access
  * Eliminated bastion host requirements and reduced attack surface

* **Infrastructure as Code Mastery with CloudFormation:**
  * Wrote YAML templates to define VPC and EC2 infrastructure
  * Managed complete infrastructure lifecycle (Create/Update/Delete)
  * Implemented Change Sets for safe infrastructure updates
  * Utilized Drift Detection to identify manual configuration changes
  * Achieved repeatable, version-controlled infrastructure deployments
  * Eliminated manual configuration errors and inconsistencies

* **Advanced Infrastructure Automation with AWS CDK:**
  * Used TypeScript/Python for imperative infrastructure definition
  * Leveraged high-level L2/L3 Constructs for rapid development
  * Created VPC with single line of code vs dozens in CloudFormation
  * Built custom reusable Constructs for organizational standards
  * Solved circular dependencies and managed environment context
  * Accelerated infrastructure development with programming language features

* **Implemented Resource Organization with Tags:**
  * Established consistent tagging strategy (CostCenter, Environment, Owner)
  * Created Resource Groups based on tag queries
  * Enabled cost allocation tracking by project/team
  * Simplified management of related resource collections
  * Automated resource discovery and operational tasks
  * Improved governance and cost visibility across organization

* **Applied Attribute-Based Access Control (ABAC):**
  * Implemented IAM policies using resource tags for access control
  * Created policies allowing actions only on resources with matching tags
  * Enabled developers to manage only their tagged resources
  * Eliminated need to update IAM policies for each new resource
  * Achieved dynamic, scalable access control system
  * Reduced IAM policy complexity and administrative overhead

* **Achieved Operational Excellence Milestone:**
  * Transitioned from manual operations to automated infrastructure
  * Eliminated configuration drift with IaC practices
  * Implemented secure, auditable server access patterns
  * Built foundation for enterprise-scale operations
  * Mastered both declarative (CloudFormation) and imperative (CDK) IaC approaches
  * Ready for advanced security and migration challenges
