---
title: "Week 7 Worklog"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Master migration strategies from on-premise to AWS cloud
* Migrate virtual machines with AWS VM Import/Export
* Execute database migration with DMS and Schema Conversion Tool
* Implement disaster recovery with AWS Elastic Disaster Recovery
* Centralize backup management with AWS Backup
* Build reliable systems with messaging (SQS and SNS)
* Understand shared storage solutions (EBS Multi-Attach and EFS)

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **VM Migration with AWS VM Import/Export** <br> - **Practice:** <br>&emsp; + Simulate on-premise environment with VirtualBox <br>&emsp; + Export VMs to .ova/.vmdk format <br>&emsp; + Upload to S3 and import as AMI <br>&emsp; + Launch EC2 from migrated AMI | 10/20/2025 | 10/20/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Database Migration - Schema Conversion Tool (SCT)** <br> - **Practice:** <br>&emsp; + Convert Oracle schema to Aurora PostgreSQL <br>&emsp; + Automatic conversion of tables, keys, indexes <br>&emsp; + Identify stored procedures requiring manual fixes | 10/21/2025 | 10/21/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **AWS Database Migration Service (DMS)** <br> - **Practice:** <br>&emsp; + Create Replication Instance <br>&emsp; + Configure Source and Target endpoints <br>&emsp; + Execute Full Load + CDC (Change Data Capture) <br>&emsp; + Minimize downtime during cutover | 10/22/2025 | 10/22/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **AWS Elastic Disaster Recovery (DRS)** <br> - **Practice:** <br>&emsp; + Install DRS Agent on source servers <br>&emsp; + Configure continuous block-level replication <br>&emsp; + Perform Recovery Drill without affecting production <br>&emsp; + Validate RTO and RPO metrics | 10/23/2025 | 10/23/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **AWS Backup Centralized Management** <br> - **Practice:** <br>&emsp; + Create Backup Plans for EC2, EBS, RDS, DynamoDB <br>&emsp; + Configure cross-region backup copy <br>&emsp; + Implement disaster recovery strategy <br>&emsp; + Manage all backups from single interface | 10/24/2025 | 10/24/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **Messaging Systems with SQS and SNS** <br> - **Practice:** <br>&emsp; + Implement decoupling with SQS queues <br>&emsp; + Handle traffic spikes with buffering <br>&emsp; + Build Fan-out pattern with SNS Topics <br>&emsp; + Trigger multiple SQS queues for parallel processing | 10/25/2025 | 10/25/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Shared Storage Solutions** <br> - **Practice:** <br>&emsp; + Test EBS Multi-Attach with io2 volumes <br>&emsp; + Share block storage across multiple Nitro instances <br>&emsp; + Deploy Amazon EFS for shared file system (NFS) <br>&emsp; + Compare block vs file storage use cases | 10/26/2025 | 10/26/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 7 Achievements:

* **Mastered VM Migration with AWS VM Import/Export:**
  * Simulated on-premise environment using VirtualBox
  * Exported virtual machines to .ova and .vmdk formats
  * Uploaded VM images to S3 using AWS CLI
  * Imported VM images as Amazon Machine Images (AMI)
  * Successfully launched EC2 instances from migrated AMIs
  * Executed lift-and-shift migration strategy effectively

* **Executed Database Schema Conversion:**
  * Used AWS Schema Conversion Tool (SCT) for database assessment
  * Converted Oracle database schema to Aurora PostgreSQL
  * Automatically transformed tables, keys, indexes, and constraints
  * Identified stored procedures requiring manual refactoring
  * Generated detailed assessment reports for migration planning
  * Understood heterogeneous database migration challenges

* **Implemented Continuous Database Migration with DMS:**
  * Created DMS Replication Instance as migration intermediary
  * Configured Source (Oracle) and Target (Aurora) endpoints
  * Executed Full Load for initial data migration
  * Enabled Change Data Capture (CDC) for ongoing replication
  * Minimized downtime during production cutover
  * Achieved near-zero downtime database migration

* **Deployed Disaster Recovery with Elastic Disaster Recovery:**
  * Installed AWS DRS Agent on source servers
  * Configured continuous block-level replication to AWS
  * Replicated data to staging area with minimal performance impact
  * Performed Recovery Drills without affecting production systems
  * Validated RTO (Recovery Time Objective) and RPO (Recovery Point Objective)
  * Established robust DR strategy for business continuity

* **Centralized Backup Management with AWS Backup:**
  * Created unified backup plans for EC2, EBS, RDS, and DynamoDB
  * Configured automated backup scheduling and retention policies
  * Implemented cross-region backup copy for disaster recovery
  * Managed all backups from single centralized interface
  * Reduced operational complexity of multi-service backups
  * Ensured compliance with data protection requirements

* **Built Reliable Systems with Messaging:**
  * Implemented decoupling pattern with Amazon SQS queues
  * Buffered requests during traffic spikes to prevent backend overload
  * Built Fan-out architecture with SNS Topics
  * Triggered multiple SQS queues for parallel processing workflows
  * Achieved asynchronous, loosely-coupled system architecture
  * Enhanced system reliability and fault tolerance

* **Explored Shared Storage Solutions:**
  * Tested EBS Multi-Attach with io2 volumes on Nitro instances
  * Shared block storage across multiple instances for cluster applications
  * Deployed Amazon EFS for NFS-based shared file systems
  * Compared block storage (EBS) vs file storage (EFS) use cases
  * Enabled multiple instances to access common data simultaneously
  * Supported stateful applications requiring shared storage

* **Completed Migration and DR Milestone:**
  * Mastered multiple migration strategies: VM, database, application
  * Implemented comprehensive disaster recovery architecture
  * Achieved business continuity readiness with backup and replication
  * Built resilient systems using messaging patterns
  * Ready for cost optimization and advanced networking challenges
  * Established foundation for cloud-first operations
