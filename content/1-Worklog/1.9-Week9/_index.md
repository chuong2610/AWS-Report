---
title: "Week 9 Worklog"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Master containerization fundamentals with Docker
* Deploy serverless containers with Amazon ECS and AWS Fargate
* Automate ECS infrastructure with AWS CDK
* Learn Kubernetes on AWS with Amazon EKS
* Deploy applications to EKS clusters
* Build CI/CD pipelines for containerized applications
* Explore Red Hat OpenShift Service on AWS (ROSA)

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learn **Containerization with Docker** <br> - **Practice:** <br>&emsp; + Write optimized Dockerfile with multi-stage builds <br>&emsp; + Build and test Docker images locally <br>&emsp; + Create Amazon ECR repository <br>&emsp; + Push images to ECR for secure private storage <br>&emsp; + Reduce image size with optimization techniques | 11/03/2025 | 11/03/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn **Amazon ECS and AWS Fargate** <br> - **Practice:** <br>&emsp; + Create ECS Task Definitions (CPU/RAM allocation) <br>&emsp; + Choose Fargate launch type (serverless) <br>&emsp; + Deploy ECS Service with desired replica count <br>&emsp; + Integrate with Application Load Balancer <br>&emsp; + Achieve zero infrastructure management | 11/04/2025 | 11/04/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Learn **Infrastructure as Code for ECS with CDK** <br> - **Practice:** <br>&emsp; + Use ApplicationLoadBalancedFargateService construct <br>&emsp; + Deploy complete architecture (VPC, ALB, ECS) with 20 lines of code <br>&emsp; + Automate ECS infrastructure deployment <br>&emsp; + Leverage high-level CDK constructs for rapid development | 11/05/2025 | 11/05/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn **Getting Started with Amazon EKS** <br> - **Practice:** <br>&emsp; + Initialize EKS Control Plane with eksctl or CDK <br>&emsp; + Configure Managed Node Groups for worker nodes <br>&emsp; + Automate node patching and upgrades <br>&emsp; + Set up kubectl for cluster management <br>&emsp; + Understand Kubernetes on AWS architecture | 11/06/2025 | 11/06/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Learn **Deploying Applications to Amazon EKS** <br> - **Practice:** <br>&emsp; + Write Kubernetes manifests (Deployment, Service, Ingress) <br>&emsp; + Deploy applications using kubectl apply <br>&emsp; + Install AWS Load Balancer Controller <br>&emsp; + Auto-create ALB from Ingress resources <br>&emsp; + Manage application lifecycle on Kubernetes | 11/07/2025 | 11/07/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 7   | - Learn **CI/CD Pipelines for ECS and EKS** <br> - **Practice:** <br>&emsp; + Build pipeline: CodeCommit → CodeBuild → ECR → ECS/EKS <br>&emsp; + Automate image building and testing <br>&emsp; + Implement Blue/Green deployment strategy <br>&emsp; + Minimize deployment risk with automated rollback <br>&emsp; + Achieve continuous delivery for containers | 11/08/2025 | 11/08/2025      | <https://cloudjourney.awsstudygroup.com/> |
| CN  | - Learn **Red Hat OpenShift Service on AWS (ROSA)** <br> - **Practice:** <br>&emsp; + Understand managed OpenShift on AWS <br>&emsp; + Explore migration path for existing OpenShift workloads <br>&emsp; + Compare ROSA vs EKS features <br>&emsp; + Identify use cases for enterprise OpenShift customers | 11/09/2025 | 11/09/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 9 Achievements:

* **Mastered Docker Containerization Fundamentals:**
  * Wrote optimized Dockerfiles with multi-stage build patterns
  * Built lightweight container images with minimal layers
  * Tested applications locally in Docker containers
  * Created private Amazon ECR repositories
  * Pushed Docker images to ECR with secure authentication
  * Achieved portable, consistent application deployment across environments

* **Deployed Serverless Containers with ECS and Fargate:**
  * Created ECS Task Definitions specifying CPU and memory requirements
  * Selected Fargate launch type for zero infrastructure management
  * Deployed ECS Services maintaining desired replica count
  * Integrated ECS with Application Load Balancer for traffic distribution
  * Achieved automatic container orchestration without managing EC2 instances
  * Eliminated server management overhead while maintaining control

* **Automated ECS Infrastructure with AWS CDK:**
  * Leveraged ApplicationLoadBalancedFargateService L3 construct
  * Deployed complete containerized architecture (VPC, ALB, ECS Cluster, Service) with ~20 lines of code
  * Automated infrastructure provisioning with programming language advantages
  * Achieved rapid development and deployment of container infrastructure
  * Reduced infrastructure code complexity by 80% vs CloudFormation
  * Established reusable patterns for container deployments

* **Launched Production-Grade Kubernetes with Amazon EKS:**
  * Initialized EKS Control Plane using eksctl and CDK EKS Blueprints
  * Configured Managed Node Groups with automated patching and upgrades
  * Set up kubectl for Kubernetes cluster management
  * Understood EKS architecture: Control Plane (AWS-managed), Data Plane (Customer VPC)
  * Eliminated Kubernetes control plane operational overhead
  * Achieved enterprise-grade Kubernetes without infrastructure complexity

* **Deployed Applications to EKS Successfully:**
  * Wrote standard Kubernetes manifests (Deployment, Service, Ingress YAML)
  * Deployed multi-replica applications with kubectl apply
  * Installed AWS Load Balancer Controller for AWS integration
  * Automatically created Application Load Balancers from Ingress resources
  * Managed rolling updates and rollbacks with Kubernetes native tools
  * Achieved cloud-native application deployment on Kubernetes

* **Built Complete CI/CD Pipelines for Containers:**
  * Designed end-to-end pipeline: CodeCommit → CodeBuild → ECR → CodeDeploy
  * Automated Docker image building, testing, and security scanning
  * Implemented Blue/Green deployment strategy for zero-downtime updates
  * Configured automatic rollback on deployment failures
  * Integrated with ECS and EKS for seamless container updates
  * Achieved continuous delivery with deployment automation

* **Explored Enterprise OpenShift on AWS:**
  * Understood Red Hat OpenShift Service on AWS (ROSA)
  * Evaluated ROSA as managed OpenShift alternative to EKS
  * Identified migration path for on-premise OpenShift workloads
  * Compared OpenShift developer experience vs vanilla Kubernetes
  * Recognized use cases for enterprises with OpenShift expertise
  * Expanded container orchestration options for hybrid cloud

* **Completed Container Technology Milestone:**
  * Transitioned from virtual machines to containerized architectures
  * Mastered both ECS (AWS-native) and EKS (Kubernetes-based) platforms
  * Implemented serverless containers eliminating infrastructure management
  * Built automated CI/CD pipelines for container deployments
  * Achieved modern, scalable application deployment patterns
  * Ready for serverless and event-driven architecture challenges
  * Established foundation for cloud-native application development

