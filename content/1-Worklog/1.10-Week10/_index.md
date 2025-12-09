---
title: "Week 10 Worklog"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Master serverless computing fundamentals with AWS Lambda
* Build complete serverless backends with Lambda, API Gateway, and DynamoDB
* Implement authentication and authorization with Amazon Cognito
* Configure custom domains and SSL certificates for serverless APIs
* Design event-driven architectures with S3, SQS, and SNS
* Orchestrate complex workflows with AWS Step Functions
* Build real-time GraphQL APIs with AWS AppSync
* Monitor and trace serverless applications with AWS X-Ray
* Automate serverless deployments with AWS SAM

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Serverless Backend with Lambda, API Gateway, DynamoDB** <br> - **Practice:** <br>&emsp; + Write Lambda functions for business logic (CRUD operations) <br>&emsp; + Integrate Lambda with DynamoDB using AWS SDK <br>&emsp; + Create REST API with API Gateway <br>&emsp; + Configure Lambda proxy integration <br>&emsp; + Build complete serverless CRUD API | 11/10/2025 | 11/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Serverless Authentication with Amazon Cognito** <br> - **Practice:** <br>&emsp; + Create Cognito User Pool for authentication <br>&emsp; + Configure sign-up and sign-in workflows <br>&emsp; + Add Cognito Authorizer to API Gateway <br>&emsp; + Block unauthorized API requests <br>&emsp; + Implement JWT token validation | 11/11/2025 | 11/11/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **Custom Domains and SSL for Serverless Applications** <br> - **Practice:** <br>&emsp; + Request ACM certificates for custom domains <br>&emsp; + Configure API Gateway custom domain names <br>&emsp; + Map custom domains (api.example.com) to API stages <br>&emsp; + Replace default AWS endpoints with branded URLs <br>&emsp; + Implement SSL/TLS encryption | 11/12/2025 | 11/12/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **Event-Driven Architecture with SQS and SNS** <br> - **Practice:** <br>&emsp; + Build asynchronous order processing with SQS <br>&emsp; + Trigger Lambda from SQS queue messages <br>&emsp; + Implement Fan-out pattern with SNS <br>&emsp; + Process orders and send notifications in parallel <br>&emsp; + Achieve decoupled, scalable architecture | 11/13/2025 | 11/13/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **S3 Event-Driven Processing** <br> - **Practice:** <br>&emsp; + Configure S3 event notifications to trigger Lambda <br>&emsp; + Automatically process uploaded images <br>&emsp; + Generate thumbnails on S3 PUT events <br>&emsp; + Implement real-time file processing <br>&emsp; + Build serverless data pipelines | 11/14/2025 | 11/14/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **Workflow Orchestration with AWS Step Functions** <br> - **Practice:** <br>&emsp; + Design state machines for order approval workflow <br>&emsp; + Chain multiple Lambda functions (Check inventory → Charge card → Send email) <br>&emsp; + Implement error handling with Retry/Catch <br>&emsp; + Add conditional logic and parallel processing <br>&emsp; + Eliminate "Lambda Pinball" anti-pattern | 11/15/2025 | 11/15/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Real-Time GraphQL with AWS AppSync** <br> - **Practice:** <br>&emsp; + Create GraphQL schema and API with AppSync <br>&emsp; + Configure DynamoDB as data source <br>&emsp; + Implement GraphQL queries, mutations, subscriptions <br>&emsp; + Enable real-time updates via WebSocket <br>&emsp; + Build chat applications and live dashboards | 11/16/2025 | 11/16/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 10 Achievements:

* **Mastered Serverless Computing Fundamentals:**
  * Built complete serverless backend with Lambda + API Gateway + DynamoDB
  * Wrote Lambda functions handling business logic (CRUD operations)
  * Integrated Lambda with DynamoDB using AWS SDK (Boto3/JavaScript)
  * Created REST APIs with API Gateway and Lambda proxy integration
  * Eliminated server management and infrastructure overhead
  * Achieved automatic scaling with pay-per-request pricing

* **Implemented Serverless Authentication and Authorization:**
  * Created Amazon Cognito User Pools for user management
  * Configured secure sign-up, sign-in, and password reset workflows
  * Added Cognito Authorizer to API Gateway for JWT validation
  * Blocked unauthorized requests automatically
  * Implemented fine-grained access control with Cognito groups
  * Achieved enterprise-grade authentication without custom code

* **Configured Custom Domains and SSL Certificates:**
  * Requested and validated ACM SSL/TLS certificates
  * Configured API Gateway custom domain names
  * Mapped custom domains (api.example.com) to API stages
  * Replaced unfriendly AWS endpoints with branded URLs
  * Implemented HTTPS encryption for all API traffic
  * Enhanced professional appearance and security posture

* **Built Event-Driven Architectures:**
  * Implemented asynchronous order processing with Amazon SQS
  * Triggered Lambda functions from SQS queue messages
  * Built Fan-out pattern with SNS Topics for parallel processing
  * Processed orders, sent emails, and updated inventory simultaneously
  * Achieved loose coupling and high scalability
  * Eliminated synchronous dependencies between components

* **Implemented S3-Triggered Serverless Processing:**
  * Configured S3 event notifications to invoke Lambda automatically
  * Processed uploaded images in real-time (thumbnail generation)
  * Built serverless data pipelines triggered by file uploads
  * Implemented automatic image resizing, format conversion, metadata extraction
  * Achieved zero-latency file processing
  * Eliminated polling and manual processing workflows

* **Orchestrated Complex Workflows with Step Functions:**
  * Designed visual state machines for multi-step business processes
  * Chained Lambda functions: Check inventory → Charge payment → Send confirmation
  * Implemented error handling with automatic Retry and Catch blocks
  * Added conditional branching (if/else) and parallel execution
  * Eliminated complex Lambda coordination code ("Lambda Pinball")
  * Achieved reliable, observable workflow execution

* **Built Real-Time GraphQL APIs with AppSync:**
  * Created GraphQL schemas defining types, queries, mutations, subscriptions
  * Configured AppSync with DynamoDB as primary data source
  * Implemented flexible GraphQL queries replacing multiple REST endpoints
  * Enabled real-time updates via GraphQL Subscriptions over WebSocket
  * Built live chat applications and auto-updating dashboards
  * Achieved modern API design with real-time capabilities

* **Implemented Distributed Tracing with X-Ray:**
  * Enabled AWS X-Ray for serverless application tracing
  * Visualized service maps showing request flow: API Gateway → Lambda → DynamoDB
  * Analyzed latency breakdown for each service segment
  * Identified performance bottlenecks and cold start issues
  * Debugged distributed applications with end-to-end traces
  * Improved application performance with data-driven optimization

* **Automated Deployments with AWS SAM:**
  * Used SAM templates for Infrastructure as Code
  * Tested Lambda and API Gateway locally with `sam local start-api`
  * Debugged serverless applications on local machine with Docker
  * Deployed serverless applications with single `sam deploy` command
  * Achieved consistent, repeatable serverless deployments
  * Accelerated development with local testing capabilities

* **Completed Serverless Architecture Milestone:**
  * Transitioned from container-based to serverless architectures
  * Built production-ready serverless applications with zero server management
  * Implemented authentication, event-driven patterns, and workflow orchestration
  * Achieved automatic scaling with pay-per-use cost model
  * Mastered complete serverless technology stack
  * Ready for application modernization and microservices challenges
  * Established foundation for cloud-native, event-driven development

