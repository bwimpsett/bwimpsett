# Brian Wimpsett

**Senior .NET Software Engineer** | Distributed Systems, Event-Driven Architecture & SQL Server | Chicago, IL

[![GitHub](https://img.shields.io/badge/GitHub-bwimpsett-181717?logo=github)](https://github.com/bwimpsett)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin)](https://www.linkedin.com/in/brianwimpsett)

Software engineer with **15+ years of experience** designing, modernizing, and scaling enterprise **.NET** platforms, high-throughput **SQL Server** databases, and **Azure** cloud microservices. Focused on clean domain boundaries, resilient asynchronous messaging, and high-performance data access.

---

## Featured Projects

### [ClaimStream](https://github.com/bwimpsett/ClaimStream) — Event-Driven .NET 10 Microservices Platform
[![.NET 10](https://img.shields.io/badge/.NET-10.0%20LTS-512BD4?logo=dotnet&logoColor=white)](https://github.com/bwimpsett/ClaimStream)
[![MassTransit](https://img.shields.io/badge/MassTransit-Outbox%20%26%20Inbox-008080)](https://github.com/bwimpsett/ClaimStream)
[![Azure](https://img.shields.io/badge/Azure-Container%20Apps%20%7C%20Service%20Bus%20%7C%20SQL-0078D4?logo=microsoftazure&logoColor=white)](https://github.com/bwimpsett/ClaimStream)

An insurance claims intake, adjudication, and notification system demonstrating production distributed-systems patterns on **.NET 10 (LTS)**:
* **Transactional Outbox & Idempotent Inbox:** Guarantees atomic SQL Server writes and integration event publishing with MassTransit and EF Core, preventing dual-write inconsistencies and deduplicating at-least-once deliveries.
* **Zero-Code Broker Portability:** Runs locally via Docker Compose on **RabbitMQ** and switches to **Azure Service Bus** with passwordless Microsoft Entra ID (`DefaultAzureCredential`) authentication through configuration alone.
* **Edge Gateway & Fault Isolation:** Routes traffic through a **YARP** reverse proxy with correlation ID propagation and IP rate limiting, backed by exponential retry backoff and Dead-Letter Queue (`_error`) handling.
* **Real-Infrastructure Testing & IaC:** Verified end-to-end with **xUnit** and **Testcontainers** (real SQL Server + RabbitMQ containers) and provisioned via modular **Azure Bicep** templates.

---

### [CloudBunny](https://github.com/bwimpsett/CloudBunny) — WAF Origin-IP Reconnaissance CLI
[![Python](https://img.shields.io/badge/Python-Security%20%26%20OSINT-3776AB?logo=python&logoColor=white)](https://github.com/bwimpsett/CloudBunny)
[![CLI](https://img.shields.io/badge/Interface-CLI%20Automation-4EAA25)](https://github.com/bwimpsett/CloudBunny)

A Python command-line reconnaissance tool built to uncover origin server IP addresses behind Web Application Firewalls (WAFs) during authorized security assessments:
* **Multi-Engine Intelligence Correlation:** Queries and cross-references host, SSL/TLS certificate, and HTTP title records across **Shodan**, **Censys**, and **ZoomEye** APIs.
* **Chunked Query & Rate-Limit Handling:** Batches large certificate result sets into configurable chunks and adapts search filters cleanly for both free and paid API tiers.

---

## Core Technical Stack

| Domain | Technologies |
| :--- | :--- |
| **Backend & Frameworks** | C#, .NET 10 / .NET 8, ASP.NET Core Web API, Minimal APIs, YARP, Razor, VB.NET |
| **Data & Persistence** | SQL Server, T-SQL, Query & Index Tuning, EF Core (Unit of Work & Migrations), Dapper |
| **Messaging & Architecture** | MassTransit, RabbitMQ, Azure Service Bus, Transactional Outbox/Inbox, Microservices |
| **Cloud, Containers & DevOps** | Microsoft Azure (Container Apps, App Services, Functions, Key Vault), Docker, Bicep, GitHub Actions, Azure DevOps |
| **Frontend & Scripting** | Angular, TypeScript, JavaScript, Python, PowerShell, Bash |
| **Testing & Observability** | xUnit, Testcontainers, Application Insights, Structured Logging |

---

## Beyond Code
* **Amateur Radio:** FCC Amateur Extra Class operator (**KZ4WJ**), active in digital packet/HF modes and Winlink communications.
* **Hardware & Electronics:** Hands-on circuit building, soldering, and PC/embedded hardware diagnostics.
