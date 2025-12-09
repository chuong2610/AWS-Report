---
title: "Week 11 Worklog"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Master application modernization strategies from monolith to microservices
* Apply Strangler Fig Pattern for incremental migration
* Build independent microservices with database-per-service pattern
* Implement asynchronous microservices communication with messaging
* Build complete CI/CD pipelines for continuous delivery
* Adopt DevOps culture and practices with AWS tools
* Deploy simplified applications with AWS Elastic Beanstalk
* Build enterprise-grade WordPress architecture on AWS

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Monolith to Microservices Migration Strategy** <br> - **Practice:** <br>&emsp; + Analyze monolithic application architecture <br>&emsp; + Identify bounded contexts for service decomposition <br>&emsp; + Apply Strangler Fig Pattern for incremental migration <br>&emsp; + Select Shopping Cart module for extraction <br>&emsp; + Plan migration without full system rewrite | 11/17/2025 | 11/17/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Create and Deploy Microservice** <br> - **Practice:** <br>&emsp; + Rewrite Shopping Cart module as independent microservice <br>&emsp; + Implement microservice with Node.js on Lambda or Fargate <br>&emsp; + Separate microservice database (DynamoDB) from monolith DB <br>&emsp; + Apply database-per-service pattern <br>&emsp; + Achieve data independence and loose coupling | 11/18/2025 | 11/18/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **Microservices Messaging and Eventing** <br> - **Practice:** <br>&emsp; + Replace synchronous HTTP calls with asynchronous messaging <br>&emsp; + Implement event-driven communication via EventBridge <br>&emsp; + Use SNS/SQS for service-to-service messaging <br>&emsp; + Eliminate tight coupling between microservices <br>&emsp; + Improve resilience and scalability | 11/19/2025 | 11/19/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **CI/CD for Application Release** <br> - **Practice:** <br>&emsp; + Build complete pipeline: Source → Build → Test → Deploy <br>&emsp; + Use CodeCommit for source control <br>&emsp; + Automate builds with CodeBuild <br>&emsp; + Deploy with CodeDeploy <br>&emsp; + Add manual approval gate before production deployment | 11/20/2025 | 11/20/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **DevOps Culture with AWS CodePipeline** <br> - **Practice:** <br>&emsp; + Integrate security testing in build phase (Shift Left) <br>&emsp; + Add SAST/DAST security scans to pipeline <br>&emsp; + Automatically fail pipeline on security vulnerabilities <br>&emsp; + Implement continuous security validation <br>&emsp; + Adopt DevSecOps practices | 11/21/2025 | 11/21/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **AWS Elastic Beanstalk Workshop** <br> - **Practice:** <br>&emsp; + Deploy Node.js application to Elastic Beanstalk <br>&emsp; + Use platform-as-a-service for simplified deployment <br>&emsp; + Automatic provisioning of EC2, ALB, Auto Scaling <br>&emsp; + Compare Beanstalk (simplicity) vs ECS/EKS (control) <br>&emsp; + Evaluate trade-offs for different use cases | 11/22/2025 | 11/22/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Enterprise WordPress on AWS** <br> - **Practice:** <br>&emsp; + Design scalable WordPress architecture <br>&emsp; + Use Aurora Serverless for database <br>&emsp; + Share wp-content with Amazon EFS across instances <br>&emsp; + Implement ElastiCache for object caching <br>&emsp; + Deploy CloudFront CDN for static content <br>&emsp; + Build production-ready WordPress at scale | 11/23/2025 | 11/23/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 11 Achievements:

* **Mastered Monolith to Microservices Migration:**
  * Analyzed monolithic application identifying tight coupling and dependencies
  * Identified bounded contexts using Domain-Driven Design principles
  * Applied Strangler Fig Pattern for gradual, risk-minimized migration
  * Selected Shopping Cart module as first microservice extraction candidate
  * Avoided big-bang rewrite risks with incremental approach
  * Established migration strategy for legacy application modernization

* **Built Independent Microservices:**
  * Rewrote Shopping Cart module as standalone microservice
  * Implemented microservice using Node.js on Lambda (serverless) and Fargate (containerized)
  * Created separate DynamoDB table for Shopping Cart data
  * Applied database-per-service pattern for data independence
  * Eliminated shared database anti-pattern from monolith
  * Achieved autonomous microservice deployment and scaling

* **Implemented Event-Driven Microservices Communication:**
  * Replaced synchronous REST calls with asynchronous messaging
  * Used Amazon EventBridge for event-driven service communication
  * Implemented pub/sub pattern with SNS and SQS
  * Decoupled microservices eliminating runtime dependencies
  * Improved system resilience (failures don't cascade)
  * Enhanced scalability with asynchronous processing

* **Built Complete CI/CD Pipelines:**
  * Designed end-to-end pipeline: CodeCommit → CodeBuild → CodeDeploy
  * Automated source control with AWS CodeCommit
  * Implemented automated builds, unit tests, and integration tests
  * Deployed applications automatically to staging and production
  * Added manual approval gate before production deployment
  * Achieved continuous delivery with quality gates

* **Adopted DevSecOps Culture:**
  * Integrated security testing early in development lifecycle (Shift Left)
  * Added Static Application Security Testing (SAST) in build phase
  * Implemented Dynamic Application Security Testing (DAST) pre-deployment
  * Configured pipeline to fail on critical security vulnerabilities
  * Prevented vulnerable code from reaching production
  * Embedded security into DevOps workflow

* **Deployed Simplified Applications with Elastic Beanstalk:**
  * Deployed Node.js application using Platform-as-a-Service model
  * Achieved automatic provisioning of EC2, Load Balancer, Auto Scaling
  * Eliminated manual infrastructure configuration
  * Compared Beanstalk simplicity vs ECS/EKS control and flexibility
  * Understood trade-offs: ease of use vs customization
  * Selected appropriate deployment model for different applications

* **Built Enterprise-Grade WordPress Architecture:**
  * Designed highly available WordPress with multi-AZ deployment
  * Used Aurora Serverless for automatic database scaling
  * Shared wp-content directory with Amazon EFS across all instances
  * Implemented ElastiCache (Redis) for WordPress object caching
  * Deployed CloudFront CDN for global static content delivery
  * Achieved WordPress scalability handling millions of requests
  * Eliminated single point of failure with redundant architecture

* **Completed Application Modernization Milestone:**
  * Transformed monolithic applications into microservices architecture
  * Implemented event-driven, loosely-coupled service communication
  * Built automated CI/CD pipelines with security integration
  * Mastered both simplified (Beanstalk) and advanced (microservices) deployment models
  * Achieved DevOps maturity with continuous delivery and security
  * Ready for data analytics and AI/ML challenges
  * Established modern application development and deployment practices

