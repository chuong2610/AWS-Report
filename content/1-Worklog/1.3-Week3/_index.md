---
title: "Week 3 Worklog"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Transition from self-managed databases to AWS Managed Database services
* Master Amazon RDS (Relational Database Service) with Multi-AZ deployment
* Learn NoSQL database concepts with Amazon DynamoDB
* Implement in-memory caching with Amazon ElastiCache
* Build Highly Available Web Applications architecture
* Understand AWS Managed Microsoft AD for enterprise integration

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Amazon RDS Essentials** <br> - **Practice:** <br>&emsp; + Deploy RDS with MySQL/PostgreSQL engine <br>&emsp; + Enable Multi-AZ deployment for high availability <br>&emsp; + Understand synchronous replication and automatic failover | 09/22/2025 | 09/22/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **RDS Operations and Security** <br> - **Practice:** <br>&emsp; + Configure Security Groups for database access <br>&emsp; + Customize DB configurations via Parameter Groups <br>&emsp; + Set up Automated Backups and Manual Snapshots <br>&emsp; + Test Restore procedures (RPO validation) | 09/23/2025 | 09/23/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **Amazon DynamoDB NoSQL Essentials** <br> - **Practice:** <br>&emsp; + Design DynamoDB tables with Partition Keys <br>&emsp; + Compare Provisioned vs On-Demand capacity modes <br>&emsp; + Understand schemaless data model | 09/24/2025 | 09/24/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **Advanced DynamoDB Operations** <br> - **Practice:** <br>&emsp; + Perform PutItem, GetItem, Query, and Scan operations <br>&emsp; + Create Global Secondary Index (GSI) <br>&emsp; + Optimize queries to avoid expensive Scan operations | 09/25/2025 | 09/25/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Amazon ElastiCache for In-Memory Caching** <br> - **Practice:** <br>&emsp; + Deploy ElastiCache with Redis engine <br>&emsp; + Implement Lazy Loading caching strategy <br>&emsp; + Place cache in Private Subnet for security | 09/26/2025 | 09/26/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **Highly Available Web Applications Architecture** <br> - **Practice:** <br>&emsp; + Build 3-tier architecture (Web/App/DB) <br>&emsp; + Deploy Application Load Balancer (ALB) <br>&emsp; + Configure Multi-AZ deployment with RDS <br>&emsp; + Integrate S3 for static content | 09/27/2025 | 09/27/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **AWS Managed Microsoft AD** <br> - **Practice:** <br>&emsp; + Set up AWS Managed Microsoft AD <br>&emsp; + Join Windows EC2 instances to domain <br>&emsp; + Implement Group Policy Objects (GPO) <br>&emsp; + Simulate enterprise environment migration | 09/28/2025 | 09/28/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 3 Achievements:

* **Mastered Managed Relational Databases with Amazon RDS:**
  * Deployed MySQL and PostgreSQL RDS instances
  * Configured Multi-AZ deployment for automatic failover
  * Understood synchronous replication mechanism
  * Secured database with Security Group restrictions (no public internet access)
  * Customized database parameters via Parameter Groups
  * Implemented automated backup and point-in-time recovery

* **Acquired NoSQL Database Skills with Amazon DynamoDB:**
  * Designed tables with appropriate Partition Keys
  * Understood schemaless/flexible data model advantages
  * Compared Provisioned (predictable traffic) vs On-Demand (unpredictable traffic) capacity modes
  * Performed CRUD operations: PutItem, GetItem, Query, Scan
  * Created Global Secondary Indexes (GSI) for flexible querying
  * Recognized performance impact of Scan vs Query operations

* **Implemented In-Memory Caching:**
  * Deployed Amazon ElastiCache with Redis engine
  * Applied Lazy Loading pattern (cache-aside strategy)
  * Reduced database load through effective caching
  * Placed cache in Private Subnet for low latency and security

* **Built Production-Ready Highly Available Architecture:**
  * Designed and implemented 3-tier architecture:
    - Web Tier: EC2 instances in multiple AZs behind ALB
    - Application Tier: EC2 instances with app logic
    - Database Tier: RDS Multi-AZ for data persistence
  * Configured Application Load Balancer for traffic distribution
  * Integrated S3 for static content delivery
  * Achieved fault tolerance and high availability

* **Integrated Enterprise Directory Services:**
  * Set up AWS Managed Microsoft AD
  * Joined Windows EC2 instances to Active Directory domain
  * Implemented Group Policy Objects (GPO) for centralized management
  * Simulated traditional on-premise environment migration to AWS

* **Understood the transition benefits:**
  * From self-managed to managed services (reduced operational overhead)
  * From single-AZ to Multi-AZ (improved availability)
  * From SQL-only to SQL + NoSQL (flexibility in data modeling)
  * From disk-based to in-memory storage (performance optimization)
  * Storage
  * Networking 
  * Database
  * ...

* Successfully created and configured an AWS Free Tier account.

* Became familiar with the AWS Management Console and learned how to find, access, and use services via the web interface.

* Installed and configured AWS CLI on the computer, including:
  * Access Key
  * Secret Key
  * Default Region
  * ...

* Used AWS CLI to perform basic operations such as:

  * Check account & configuration information
  * Retrieve the list of regions
  * View EC2 service
  * Create and manage key pairs
  * Check information about running services
  * ...

* Acquired the ability to connect between the web interface and CLI to manage AWS resources in parallel.
* ...
