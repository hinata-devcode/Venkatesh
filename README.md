# Hey, I'm Venkatesh 👋

**Backend Engineer** at **Razorpay** — working in payments infrastructure where correctness isn't optional and failures have real financial consequences.

Day to day: debugging live transaction failures, stabilizing merchant integrations across Payout and Fund Account Validation APIs, and contributing to platform reliability at scale.

Before Razorpay, I built a multi-tenant workflow automation platform from scratch at **Brane Enterprises** — microservices, Spring Boot, REST APIs, query optimization across the full lifecycle.

I gravitate toward problems where **async systems, failure recovery, and distributed consistency** actually matter.

---

## 🔧 What I Work With

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Apache Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white)

---

## 🚀 Featured Projects

### 🏦 Financial Validation Engine
> *Java · Spring Boot · MySQL · Redis · Resilience4j · JWT · HMAC · Docker · AWS*

A fault-tolerant, **distributed-ready** backend system that validates bank accounts and VPAs through external payment provider APIs — built to mirror how real fintech backends handle async flows, distributed consistency, and failure recovery.

I recently upgraded this significantly and would genuinely love for you to take a look 👇

**What's under the hood:**
- Fully **asynchronous** validation pipeline — API returns immediately, workers process in the background
- **Multi-instance safe**: designed to run across 5+ Docker containers with no race conditions on state transitions or retries
- **Distributed rate limiting** via Redis + Bucket4j — limits enforced uniformly across all instances
- **Circuit breaker** (Resilience4j) protecting the system from cascading failures when providers degrade
- **Idempotency controls** — safe retries with no duplicate processing, critical for financial correctness
- State-driven lifecycle (`INITIATED → PROCESSING → COMPLETED/FAILED`) preventing inconsistent updates
- Webhook ingestion secured with **HMAC signature verification**
- Scheduler-based **reconciliation** that auto-recovers validations when webhooks are delayed or never arrive
- Fully containerized with Docker Compose, deployed on AWS EC2

**This project directly mirrors the Fund Account Validation system I work with at Razorpay — built to understand it from the inside out.**

📂 [View Repository](https://github.com/hinata-devcode/validation-service) · 🎥 [Watch Demo](https://drive.google.com/file/d/1sAMhtqYEhAUSptF8p_Rug2sZc9L6B98m/view?usp=sharing)

---

### 🤖 Enterprise RAG Support System
> *Python · FastAPI · LangChain · ChromaDB · Gemini · Azure OpenAI (GPT-4o)*

A multi-tenant, enterprise-grade Retrieval-Augmented Generation backend — built with a modular monolith architecture and production-level reliability patterns.

**What's interesting about this one:**
- RBAC enforced at the **vector database layer** via metadata filtering — external users physically cannot retrieve internal knowledge chunks, regardless of what they query
- Circuit-breaker model routing: if Gemini 2.5 Pro hits rate limits, traffic auto-falls to Gemini Flash, then Azure OpenAI GPT-4o — zero downtime
- Self-healing knowledge injection: admins can push hardcoded Q&A corrections directly into the vector store without any model retraining
- Clean client-server separation — Streamlit UI is a pure presentation layer, zero AI or DB logic on the frontend

📂 [View Repository](https://github.com/hinata-devcode/RAG-Application)

---

## 📌 What I'm Thinking About

- How **distributed systems** stay consistent under failure — not just in theory, but in the specific ways payment systems break in production
- The gap between "it works" and **"it's observable, recoverable, and safe to operate"** — and how to close it through better architecture choices
- How large-scale platforms like Razorpay's Payouts handle correctness guarantees at volume

---

## 🏆 Recognition

**BU Open House — Rookie MVP** · Razorpay · 2025
> Awarded for outstanding backend contribution and measurable impact within the first 3 months at Razorpay.

---

## 📬 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yangala-venkatesh/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/venky_1502/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:venkatesh.careerjourney@gmail.com)
