---
title: "Week 6 Worklog"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Build multi-layer defense-in-depth security architecture
* Protect applications with AWS WAF (Web Application Firewall)
* Master encryption with AWS KMS (Key Management Service)
* Secure credentials with AWS Secrets Manager and automatic rotation
* Implement intelligent threat detection with AWS GuardDuty
* Integrate user authentication with Amazon Cognito
* Achieve security compliance with AWS Security Hub
* Ensure private connectivity with VPC Endpoints

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **AWS WAF (Web Application Firewall)** <br> - **Practice:** <br>&emsp; + Create Web ACL and attach to ALB/CloudFront <br>&emsp; + Configure rules to block SQL Injection and XSS <br>&emsp; + Implement rate-limiting (100 requests/5min) <br>&emsp; + Mitigate application-layer DDoS attacks | 10/13/2025 | 10/13/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **AWS KMS (Key Management Service)** <br> - **Practice:** <br>&emsp; + Create Customer Master Keys <br>&emsp; + Encrypt EBS volumes and S3 objects <br>&emsp; + Implement encryption at rest | 10/14/2025 | 10/14/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **AWS Secrets Manager** <br> - **Practice:** <br>&emsp; + Store database credentials securely <br>&emsp; + Enable automatic rotation <br>&emsp; + Integrate with applications | 10/15/2025 | 10/15/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **AWS GuardDuty** <br> - **Practice:** <br>&emsp; + Enable intelligent threat detection <br>&emsp; + Monitor security findings <br>&emsp; + Configure automated responses | 10/16/2025 | 10/16/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Amazon Cognito** <br> - **Practice:** <br>&emsp; + Implement user authentication <br>&emsp; + Configure User Pools <br>&emsp; + Integrate with applications | 10/17/2025 | 10/17/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **AWS Security Hub and VPC Endpoints** <br> - **Practice:** <br>&emsp; + Enable Security Hub for compliance <br>&emsp; + Configure VPC Endpoints <br>&emsp; + Review security best practices | 10/18/2025 | 10/18/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - **Week Review and Security Audit** <br>&emsp; + Review security implementations <br>&emsp; + Perform security audit <br>&emsp; + Prepare for next week | 10/19/2025 | 10/19/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 6 Achievements:

* **Built Application Protection with AWS WAF:**
  * Deployed Web Application Firewall on ALB and CloudFront
  * Created Web ACL with rules blocking SQL Injection and XSS attacks
  * Implemented rate-based rules (100 requests/5min) to prevent abuse
  * Mitigated application-layer DDoS attacks effectively
  * Protected web applications from OWASP Top 10 vulnerabilities
  * Achieved defense-in-depth security posture for web tier

* **Achieved Encryption Mastery with AWS KMS:**
  * Created Customer Managed Keys (CMK) for symmetric encryption
  * Configured Key Policies controlling administrative and usage permissions
  * Enabled encryption-at-rest for EBS volumes and S3 buckets
  * Separated key management from key usage responsibilities
  * Implemented cryptographic best practices for data protection
  * Achieved compliance with encryption requirements (HIPAA, PCI-DSS)

* **Secured Credentials with AWS Secrets Manager:**
  * Stored RDS passwords in centrally managed Secrets Manager
  * Configured automatic credential rotation with Lambda functions
  * Updated application code to retrieve secrets via API calls
  * Eliminated hardcoded credentials from configuration files
  * Implemented just-in-time credential access
  * Reduced credential exposure and security risks

* **Implemented Intelligent Threat Detection with GuardDuty:**
  * Enabled continuous security monitoring across AWS account
  * Analyzed CloudTrail Events, VPC Flow Logs, and DNS Logs
  * Leveraged machine learning to detect anomalous behavior
  * Identified threats: cryptocurrency mining, malicious IP access, privilege escalation
  * Configured EventBridge for automated alert notifications
  * Achieved proactive threat detection without infrastructure overhead

* **Integrated User Authentication with Amazon Cognito:**
  * Created User Pools for application user management
  * Implemented secure sign-up and sign-in workflows
  * Configured Identity Pools for AWS credential federation
  * Enabled end-users to directly upload files to S3 with temporary credentials
  * Eliminated backend server requirements for user authentication
  * Built scalable, serverless authentication system

* **Achieved Security Compliance with AWS Security Hub:**
  * Enabled centralized security findings aggregation
  * Integrated GuardDuty, Macie, and Inspector findings
  * Evaluated security posture against CIS AWS Foundations Benchmark
  * Generated compliance scores and remediation guidance
  * Unified security monitoring across multiple security services
  * Improved security governance and audit readiness

* **Ensured Private Connectivity with VPC Endpoints:**
  * Deployed S3 Gateway Endpoint for private S3 access
  * Updated Private Subnet Route Tables for endpoint routing
  * Eliminated internet gateway traversal for AWS service access
  * Reduced data transfer costs and enhanced security
  * Kept sensitive data within AWS internal network
  * Achieved zero-trust network architecture for cloud services

* **Completed Defense-in-Depth Security Architecture:**
  * Built multi-layer security spanning network, application, data layers
  * Implemented security controls: WAF, KMS, Secrets Manager, GuardDuty, Cognito
  * Achieved comprehensive threat protection and compliance posture
  * Mastered encryption, authentication, and threat detection
  * Ready for production workload security requirements
  * Established security-first mindset for cloud architecture
