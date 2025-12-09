---
title: "Event 1"
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Event Report: "Vietnam Cloud Day 2025: Ho Chi Minh City Connect Edition for Builders"

**Focus Track:** GenAI & Data (Generative Artificial Intelligence & Data)

### I. PARTICIPATION OBJECTIVES

Attending this event aimed to stay current with the latest AWS trends and solutions, focusing on four primary goals:

1. **Comprehensive GenAI Strategy:** Understanding how to build AI-driven software development lifecycles (AI-DLC) and explore cutting-edge GenAI strategies
2. **Enterprise Security:** Deep dive into securing GenAI and AI Agents to ensure data protection
3. **Data Foundation:** Learning to construct a Unified Data Foundation optimized for Analytics and AI workloads
4. **Expert Networking:** Direct engagement with AWS engineers and specialists

**Speaker Lineup:**

AWS Team: Jun Kai Loke (AI/ML Specialist), Kien Nguyen, Tamelly Lim, Binh Tran, Taiki Dang (Solutions Architects), Michael Armentano (Principal WW GTM Specialist).

### II. CORE TECHNICAL CONTENT

#### 1. Unified Data Platform

For AI to function effectively, data must flow seamlessly. AWS emphasizes the Zero-ETL model and breaking down data silos:

- **End-to-End Workflow:** From Ingestion $\rightarrow$ Storage $\rightarrow$ Processing $\rightarrow$ Access $\rightarrow$ Governance
- **Service Ecosystem:** Tight integration among Amazon S3, Glue, Redshift, Lake Formation, and OpenSearch
- **Self-Service Philosophy:** Empowering project teams to leverage data independently while maintaining compliance standards

#### 2. GenAI Strategy & Amazon Bedrock

- **Amazon Bedrock:** Central platform for Foundation Model selection, RAG (Retrieval-Augmented Generation) deployment, and cost/latency optimization
- **AgentCore & Amazon Nova:** Strong support for modern Agent frameworks like CrewAI, LangGraph, and LlamaIndex, enabling complex automation workflows

#### 3. Multi-Layered Security for GenAI

Security extends beyond infrastructure through a "Defense in Depth" model:

- **Three Security Layers:** Infrastructure $\rightarrow$ Model $\rightarrow$ Application
- **Five Core Pillars:** Compliance, Privacy, Controls, Risk Management, and Resilience
- **Practical Tools:** Bedrock Guardrails for content filtering and OpenTelemetry for observability

#### 4. AI-Driven Development Lifecycle (AI-DLC)

This represents a fundamental shift in software development thinking:

- **Evolution:** Progressing from AI-Assisted (AI helps code) $\rightarrow$ AI-Driven (AI leads) $\rightarrow$ AI-Managed (AI manages operations)
- **Implementation:** Integrating AI across all phases: IaC (Infrastructure as Code), automated testing, to risk management

#### 5. Amazon SageMaker – Unified Studio

- Consolidated environment for Data, Analytics, and AI with Lakehouse architecture support
- Comprehensive MLOps integration (Pipelines, Registry, Monitoring) accelerating GenAI application deployment  

### III. LESSONS LEARNED & KEY INSIGHTS

From the above content, I extracted three fundamental lessons for project development:

#### Design Thinking:

- Build Data & AI systems with "End-to-End" thinking from the start to avoid fragmentation
- Governance principles must align with self-service capabilities

#### Technical Architecture:

- Maximize Zero-ETL usage (S3 $\leftrightarrow$ Redshift/Aurora/DynamoDB integration) to minimize data pipeline overhead
- Utilize AI Agents for workflow automation rather than treating AI as just a chatbot tool

#### Reliability and Accuracy:

- To reduce AI hallucinations, combine: Prompt Engineering + RAG + Fine-tuning
- Standard RAG workflow: $Input \rightarrow Embedding \rightarrow Context \rightarrow LLM \rightarrow Output$

### IV. WORK APPLICATION PLAN

Based on the acquired knowledge, I propose specific application directions:

#### 1. For Current Projects

- **Features:** Experiment with integrating AI Agents into Customer Support workflows and authentication processes
- **Safety:** Apply Bedrock Guardrails and validation layers to prevent AI from generating sensitive or misleading content

#### 2. For Development Processes (Team & Learning)

- **AI-DLC Model:** Clear task division: AI handles code generation and documentation; humans focus on Review and Approval
- **Infrastructure:** Carefully evaluate Serverless (AWS Lambda) for short-lived tasks versus Containers (ECS/Fargate) for long-running/complex workloads

#### 3. Personal Direction (Intern/Developer Role)

- **Business-First:** Always ask "What's the business value?" before writing code or gathering requirements. Technology must serve business objectives
- **Data Mindset:** Recognize that a clean, structured data foundation is a prerequisite for effective GenAI performance  

### Event Experience

Attending the **“GenAI-powered App-DB Modernization”** workshop was extremely valuable, giving me a comprehensive view of modernizing applications and databases using advanced methods and tools. Key experiences included:

#### Learning from highly skilled speakers
- Experts from AWS and major tech organizations shared **best practices** in modern application design.  
- Through real-world case studies, I gained a deeper understanding of applying **DDD** and **Event-Driven Architecture** to large projects.  

#### Hands-on technical exposure
- Participating in **event storming** sessions helped me visualize how to **model business processes** into domain events.  
- Learned how to **split microservices** and define **bounded contexts** to manage large-system complexity.  
- Understood trade-offs between **synchronous and asynchronous communication** and integration patterns like **pub/sub, point-to-point, streaming**.  

#### Leveraging modern tools
- Explored **Amazon Q Developer**, an AI tool for SDLC support from planning to maintenance.  
- Learned to **automate code transformation** and pilot serverless with **AWS Lambda** to improve productivity.  

#### Networking and discussions
- The workshop offered opportunities to exchange ideas with experts, peers, and business teams, enhancing the **ubiquitous language** between business and tech.  
- Real-world examples reinforced the importance of the **business-first approach** rather than focusing solely on technology.  

#### Lessons learned
- Applying DDD and event-driven patterns reduces **coupling** while improving **scalability** and **resilience**.  
- Modernization requires a **phased approach** with **ROI measurement**; rushing the process can be risky.  
- AI tools like Amazon Q Developer can significantly **boost productivity** when integrated into the current workflow.  



> Overall, the event not only provided technical knowledge but also helped me reshape my thinking about application design, system modernization, and cross-team collaboration.
