# Hey, I'm Venkatesh 👋

**Backend Engineer** focused on building reliable, production-grade systems in Java and Python.

Currently at **Razorpay**, working deep in the payments infrastructure space — debugging real-money transaction failures, stabilizing merchant integrations across Payout and Fund Account Validation APIs, and contributing to platform reliability at scale.

Previously at **Brane Enterprises**, where I built a multi-tenant workflow automation platform from the ground up using Java and Spring Boot — microservices, REST APIs, query optimization, the works.

---

## 🔧 What I Work With

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Apache Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)
![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white)

---

## 🚀 Featured Projects

### 🏦 Financial Validation Engine
> *Java · Spring Boot · MySQL · JWT · HMAC · Async Processing*

A fault-tolerant backend system that validates bank accounts and VPAs through external payment provider APIs — built to mirror how real fintech backends handle async flows and failure recovery.

**What's interesting about this one:**
- Fully asynchronous validation pipeline using background workers — the API returns immediately, processing happens in the background
- State-driven lifecycle (`INITIATED → PROCESSING → COMPLETED/FAILED`) that prevents duplicate processing and enables safe retries
- Webhook ingestion secured with HMAC signature verification — only trusted provider callbacks are accepted
- Scheduler-based reconciliation that auto-recovers validations when webhooks are delayed or never arrive
- JWT-secured API layer

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

## 📌 What I'm Focused On

- Deepening my understanding of **distributed systems** — consistency, fault tolerance, and async patterns
- Exploring **system design** at scale — how real payment and platform systems are architected
- Getting better at writing backend code that is not just functional but **observable, recoverable, and maintainable**

---

## 🏆 Recognition

**BU Open House — Rookie MVP** · Razorpay · 2025
> Awarded for outstanding backend contribution and measurable impact within the first 3 months at Razorpay.

---

## 📬 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yangala-venkatesh/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/venky_1502/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:venkatesh.careerjourney@gmail.com)
