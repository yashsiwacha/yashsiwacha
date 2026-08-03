<div align="center">
  <img src="./assets/banner.png?v=4" alt="Yash Siwach - Backend & Distributed Systems Engineer" width="100%" style="aspect-ratio: 1584 / 396; width: 100%; height: auto; display: block; border-radius: 8px;" />

  <br>

  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Yash_Siwach-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/yashsiwacha)
  [![Email](https://img.shields.io/badge/Email-yashsiwach07@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yashsiwach07@gmail.com)
  [![Portfolio](https://img.shields.io/badge/Portfolio-portfolio--rust--xi--90.vercel.app-10B981?style=for-the-badge&logo=vercel&logoColor=white)](https://portfolio-rust-xi-90.vercel.app)
</div>

---

## ⚡ Executive Summary

I am a **Backend Engineer** specializing in high-concurrency JVM microservices, event-driven architectures, and distributed systems. 

My work centers on designing reliable systems that guarantee strict data consistency under heavy concurrent traffic. I actively engineer event-driven pipelines utilizing **Kafka**, **Redis Lua distributed claim-checks**, and **JPA optimistic/pessimistic concurrency controls**, alongside upstream contributions to core JVM frameworks like **Micrometer** and **Resilience4j**.

---

## 🚀 Featured Engineering Projects

### 1. [Distributed Real-Time Notification Platform](https://github.com/yashsiwacha/Real-Time-Notification-System)
> *Production-grade event-driven notification infrastructure built with Spring Boot 3, Kafka, Redis, and WebSockets.*

- **Distributed Idempotency**: Engineered atomic `claim-check` mechanics via Redis Lua scripts (`claim.lua` / `complete.lua`), preventing race conditions on duplicate Kafka offsets during consumer rebalances.
- **Optimistic Concurrency**: Implemented JPA `@Version` optimistic locking to guarantee atomic database updates during simultaneous retry storms; benchmarked **1,000 concurrent update requests** demonstrating DB contention limits.
- **Performance & Latency**: Sustained **500+ events/sec** with sub-200ms p95 end-to-end delivery latency and **<25ms STOMP WebSocket dispatch latency**.
- **Observability & Deployment**: Instrumenting cross-boundary correlation IDs (`X-Request-ID`) in MDC structured logs, custom Micrometer counters, and automated deployment via GitHub Actions CI pipeline.
- **Stack**: Java 17, Spring Boot 3, Apache Kafka, Redis, PostgreSQL, STOMP WebSockets, Docker Compose, Render.

### 2. [High-Concurrency Auction Platform](https://github.com/yashsiwacha/Auction-System)
> *ACID-compliant concurrent bidding engine designed for zero data inconsistency under high bid volume.*

- **Concurrency Control**: Combined Java critical synchronization with pessimistic database locking (`SELECT FOR UPDATE`), validating transactional consistency under a **1,000+ concurrent bid event stress profile**.
- **Database Optimization**: Sub-50ms query execution achieved by eliminating N+1 query patterns via joined fetch strategies and composite indexing.
- **Security & Authorization**: Secured REST endpoints with Spring Security and stateless JWT authentication; enforced role-based access control (RBAC) at the method level.
- **Stack**: Java 11/17, Spring Boot, Spring Security (JWT), MySQL/PostgreSQL, Thymeleaf, k6, Render.

### 3. [ProjectEcho — Career Intelligence Engine](https://github.com/yashsiwacha/project-echo)
> *Modular monolith architecture executing formal enterprise architecture standards (FGM, CIF, EAF).*

- **Architecture**: Domain-driven modular monolith enforcing clean boundary isolation across career evidence verification, metrics ingestion, and governance engines.
- **Stack**: Java 17, Spring Boot 3, Maven, Domain-Driven Design (DDD).

---

## 💼 Work Experience

**EPAM Systems** — *Junior Software Engineer Intern* `[Jan 2026 – Apr 2026]`
- **Idempotency & Reliability**: Implemented transaction idempotency validation with `@Transactional` rollback semantics, preventing double-submission payment errors during network retries.
- **Database Optimization**: Reduced average query execution time by **40%** on high-traffic payment ledger tables via composite indexing and SQL query rewriting (`EXPLAIN ANALYZE`).
- **API Extension**: Extended transaction-history REST APIs with cursor-based pagination and `@Valid` request validation across REST endpoints with 30+ JUnit/Mockito tests integrated into GitHub Actions CI/CD.

---

## 🌟 Upstream Open Source Contributions

| Framework | Target Repository | Engineering Impact & Fix | Status |
| :--- | :--- | :--- | :--- |
| **Micrometer** | `micrometer-metrics/micrometer` | **Lock-Free Concurrency Fix**: Contributed a thread-safe update mechanism in `StepFunctionCounter` & `StepFunctionTimer` to prevent concurrent over-counting under heavy thread contention (`commit 6fa8bdc17`). Added deterministic multi-threaded unit tests. | Open Source Contribution |
| **Resilience4j** | `resilience4j/resilience4j` | **Spring 6 Executor Aspect Thread Mode**: Fixed custom thread executor mode resolution (virtual threads vs. platform threads) across `RetryAspect` and `TimeLimiterAspect` in Spring Boot 3 / Spring 6 (`commit 4a3bd58`). Added deterministic aspect tests. | Open Source Contribution |

---

## 🛠️ Technical Stack

**Languages & Core Frameworks**<br>
![Java](https://img.shields.io/badge/Java_17%2B-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

**Distributed Systems & Databases**<br>
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**DevOps, Observability & Testing**<br>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![JMeter](https://img.shields.io/badge/JMeter-D22128?style=for-the-badge&logo=apachejmeter&logoColor=white)

<br>**Engineering Concepts:** *Optimistic/Pessimistic Locking, Dead Letter Queues (DLQ), Lua Scripting Idempotency, MDC Tracing, Lock-Free Concurrency, Query Optimization.*

---

## 📐 Engineering Principles

1. **Design for Failure**: Assume network partitions, consumer rebalances, and DB timeouts will occur. Build exponential backoff and Dead Letter Queues (DLQ).
2. **Atomic Idempotency**: Side-effects in distributed workers must be guarded by atomic claim-check locks before execution.
3. **Empirical Measurement**: Benchmark latency and throughput using JMeter stress profiles and flame graphs before drawing conclusions.
4. **Observable Production Systems**: If a microservice is deployed, it must emit correlated logs (`X-Request-ID`), structured metrics, and health checks.

---

## 📊 GitHub Analytics

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=yashsiwacha&theme=dark&background=0d1117&ring=10b981&fire=10b981&currStreakNum=ffffff&sideNums=9ca3af&sideLabels=9ca3af&border=30363d" alt="GitHub Streak Stats" height="175" />
  <br><br>
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=yashsiwacha&theme=react-dark&bg_color=0d1117&color=10b981&line=10b981&point=ffffff&hide_border=true" alt="Contribution Graph" width="100%" />
</div>
