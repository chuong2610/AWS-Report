---
title: "Event 3"
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Comprehensive Report: AWS Cloud Mastery Series #2
**Focus:** FROM DEVOPS, IaC TO CONTAINER & OBSERVABILITY

## 1. Core Objectives

The event focused on revolutionizing software development and operations workflows on the Cloud platform:

* **Mindset Shift:** Balancing feature release speed (Speed) and system stability (Stability) through DevOps culture and the Value Cycle.
* **Infrastructure Modernization:** Eliminating manual management risks (ClickOps) through Infrastructure as Code (IaC) methodology.
* **Containerization Strategy:** Providing a reference framework for selecting appropriate orchestration platforms: from simple (App Runner), specialized (ECS) to open standards (EKS).
* **Deep Observability:** Transitioning from passive monitoring to proactive system behavior analysis with CloudWatch and X-Ray.

## 2. Featured Speakers

* **AWS Expert Team:** Provided foundational knowledge and practical demo best practices.
* **Trần Vĩ & Long Quy Nghiêm** (FCJers 2024): Shared real-world experiences from the perspective of participants actively engaged in the First Cloud Journey program.

---

## 3. In-Depth Content

### 3.1. DevOps Mindset & CI/CD Pipeline: Foundation of Speed

DevOps is not just a tool but a philosophy optimizing value flow:

* **The Value Cycle:** Closed-loop process from *Insight* (Ideas) to *Delivery* (Handover).
* **Redefining CI/CD:**
    * *Continuous Integration (CI):* Daily code commits, fail fast to detect errors early.
    * *Continuous Delivery:* Automated deployment to Staging, but Production requires manual approval.
    * *Continuous Deployment:* 100% automation to Production if all tests pass.
* **Pipeline Principles:**
    * *Build Once, Deploy Anywhere:* Package source code once (Artifact) to ensure consistency across all environments.
    * *Measurement (DORA Metrics):* Focus on 4 golden metrics: Deployment frequency, Lead time for changes, Change failure rate, and Mean time to recovery (MTTR).

### 3.2. Infrastructure as Code (IaC): From ClickOps to Code

Mandatory shift from manual Console operations to Code-based management for Version Control and reusability:

* **AWS CloudFormation:** Native tool using YAML/JSON. Manages resources by Stack, clean deletion when removed.
* **Terraform:** Open-source (HCL), optimized for Multi-cloud. *Plan -> Apply* workflow allows previewing changes, safe for operations.
* **AWS CDK:** Uses modern programming languages (Python, Java...) to build infrastructure. Supports Constructs (L1-L3) enabling complex system construction with just a few lines of code.
* **Drift Detection:** Critical feature detecting discrepancies between Code configuration and reality.

### 3.3. Containerization: Choosing the Right Platform

There's no best tool, only the most suitable tool for your needs:

* **Amazon ECS:** Simple, deeply integrated with AWS, for teams wanting to focus on Apps rather than Cluster management.
* **Amazon EKS:** International Kubernetes standard, for large systems requiring deep customization or Hybrid-cloud.
* **AWS App Runner:** "Zero-ops" solution, direct deployment from Code/Image to HTTPS URL without infrastructure concerns.
* **Compute Options:**
    * *EC2:* Server management (High control, operational overhead).
    * *Fargate:* Serverless for Containers (No OS management, just run Apps).

### 3.4. Observability: Beyond Monitoring

Shifting from "Is the system alive?" to "Why is the system slow?":

* **Amazon CloudWatch:** Central hub collecting Metrics, Logs, and Alarms (Alerts/Auto-scaling).
* **AWS X-Ray (Distributed Tracing):** Solves the "black box" problem in Microservices by mapping request paths, pinpointing latency bottlenecks or error origins precisely.

---

## 4. Personal Lessons and Reflections

This specialized session reshaped my thinking about the role of Cloud engineers:

1.  **From Ops to Platform Engineering:** The modern role isn't about manual deployment chasing but building platforms (Platform Builders). The goal is creating safe CI/CD "highways" for Developer self-service.
2.  **Operational Discipline:** Stability comes from discipline. The *Immutability* principle and banning manual fixes (ClickOps) on Production are vital for smooth system operations, avoiding human errors.
3.  **Tool Selection Thinking:** Understanding each tool's pros and cons (CloudFormation vs Terraform, ECS vs EKS) helps me make accurate architectural decisions, optimizing costs and resources for projects.

## 5. Conclusion

The **"DevOps & IaC Mastery"** event equipped me with a comprehensive maturation roadmap:

* **Thinking:** Systematize and measure with data.
* **Tools:** Control infrastructure with Code (IaC).
* **Operations:** Optimize with Containers and Observability.

These are indispensable pieces for building and operating large-scale, sustainable systems on AWS.

