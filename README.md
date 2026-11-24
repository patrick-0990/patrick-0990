<h1 align="center">Hey, I'm Patrick!</h1>

<p align="center">
  <b>Back-end Developer · Java/Spring & C#/.NET · Python · Systems Analysis and Development Student</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/kau%C3%AApatrickgodoi/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:kauepatrickbrito@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<p align="center">
  <a href="https://github.com/patrick-0990/patrick-0990/blob/main/README.md">🇧🇷 Leia em português</a>
</p>

---

## About me

I'm a back-end developer building internal automation platforms and CRMs for the legal and financial sectors, using **Java/Spring Boot** and **C#/.NET**.

If there's something that fascinates me in computing, it's two things: **software architecture** and **algorithms**. I like understanding why a solution scales, why it's the right choice for a given context, and how to organize a system so it stays easy to evolve. Day to day, that shows up in my work with concurrency, queues, asynchronous processing and resilient integrations.

I'm currently studying Systems Analysis and Development and going deeper into **system design** and **artificial intelligence**.

<details>
<summary><b>Architecture and design patterns</b></summary>

<br>

I have a solid foundation in design patterns: I know the creational, structural and behavioral patterns well, such as Factory, Builder, Adapter and Template Method, and I've applied several of them in production, such as Strategy, Specification and Observer (domain events), as well as resilience patterns like Circuit Breaker and Bulkhead.

I also have solid experience with software architecture: I've built projects using Clean Architecture, DDD, CQRS and Hexagonal Architecture (the well-known Ports & Adapters).

</details>

<details>
<summary><b>What I've built professionally</b></summary>

<br>

> Proprietary projects (built at the company I work for): solutions are described generically, without code.

- **Workflow orchestration**: an asynchronous pipeline with 10+ sequential steps modeled as a state machine, using the Strategy Pattern (new steps are added without touching the orchestrator), job tracking, retries and protection against duplicate execution. *The biggest challenge here was modeling the states and understanding the domain rules behind each routine.*

- **Applied AI**: document analysis and summarization with LLMs using structured output (JSON Schema), a chat with pluggable context per subject, and token cost tracking per feature.

- **Concurrency**: domain locks, pessimistic and optimistic locking, dedicated executors and fan-out with `CompletableFuture`; a persistent queue in PostgreSQL using `FOR UPDATE SKIP LOCKED` with graceful shutdown of workers.

- **Resilient integrations**: circuit breaker, bulkhead and rate limiter (Polly v8) on a critical third-party API integration, with exponential backoff, `Retry-After` handling and automatic token renewal. *This one took real work: it was needed because of ongoing instability with one of our data providers.*

- **Integrations**: declarative HTTP clients (OpenFeign and Refit) with several external systems, mTLS, Idempotency-Key, SFTP, AWS Lambda and S3 with pre-signed URLs. *These integrations had their own layer in the codebase, a sibling of the Infrastructure layer in traditional Clean Architecture.*

- **ETL and data quality**: event-driven bulk CSV import with encoding detection, per-row error reports, selective reprocessing and plug-and-play data enrichment. *I built it around a staging table, which saved a lot of rework: it was much easier for users when they knew exactly which data was wrong.*

- **RPA and web scraping**: automations with Playwright (headless Chromium), with execution evidence stored in S3. *I've worked both on RPA automations with Selenium and Playwright and on HTML scraping.*

- **Document processing**: .docx generation (OpenXML), DOCX → PDF conversion with headless LibreOffice, text extraction (PDFBox), adaptive PDF compression and spreadsheets (Apache POI, ClosedXML).

- **Security**: password hashing with Argon2id and JWT authentication with single-use rotating refresh tokens. *Security by design, always!*

- **Reporting engine**: a generic engine for reports and CSV templates based on a configurable catalog, reused across several modules. *This one was really fun to build: there was a lot of data available and very little flexibility in the reports.*

</details>

<details>
<summary><b>A challenge that stuck with me</b></summary>

<br>

One of my biggest challenges so far came right at the beginning of my career as a developer. The case-filing system needed the exact names of courthouses and judicial districts to file a case, and there was no standardized source for that data.

To solve it, I built an internal relational structure from scratch to store this information, and collected it through scraping court websites, phone directories and PDFs I found online. On top of all the collection and data modeling work, the names rarely matched exactly from one source to another, so I implemented Levenshtein distance to do fuzzy matching between them.

</details>

---

## Main stack

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-191919?style=for-the-badge&logo=anthropic&logoColor=white)

<sub>Also experienced with: GraphQL · MySQL · SQL Server · JPA/Hibernate · EF Core · Flyway · Terraform · JUnit · xUnit · Testcontainers · Playwright</sub>

---

## Interests and what I'm studying

- **System Design**: distributed systems, queues and messaging (SQS, Outbox Pattern), idempotency, scalability, consistency and fault tolerance.
- **Artificial Intelligence**: AI agents (LLMs, tool use, RAG and agent orchestration) and machine learning algorithms (supervised and unsupervised learning, model evaluation).

---

## Featured project

| Project | Description | Stack |
|---|---|---|
| [ETL-Pipeline-ERP-Database-Manager](https://github.com/patrick-0990/ETL-Pipeline-ERP-Database-Manager) | ETL pipeline in pure Python that migrates legacy ERP data (CSV) into a relational database, with data cleaning and referential integrity | Python · SQLite |

---

<p align="center"><i>Thanks for reading this far!</i></p>
