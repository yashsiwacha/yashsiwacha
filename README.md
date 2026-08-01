<div align="center">
  <img src="./assets/banner.png?v=4" alt="Yash Siwach - Backend & Distributed Systems Engineer" width="100%" style="aspect-ratio: 1584 / 396; width: 100%; height: auto; display: block; border-radius: 8px;" />

  <br>

  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Yash_Siwach-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/yashsiwacha)
  [![Email](https://img.shields.io/badge/Email-yashsiwach07@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yashsiwach07@gmail.com)
  [![Portfolio](https://img.shields.io/badge/Portfolio-yashsiwacha.github.io-10B981?style=for-the-badge&logo=vercel&logoColor=white)](https://yashsiwacha.github.io/Portfolio/)
</div>

---

## ⚡ Executive Summary

I am a **Backend Engineer** specializing in high-concurrency JVM microservices, event-driven architectures, and distributed systems. 

My work centers on designing reliable systems that guarantee strict data consistency under heavy concurrent traffic. I actively contribute upstream fixes to core JVM ecosystem frameworks—such as **Micrometer** and **Resilience4j**—and engineer event-driven pipelines utilizing **Kafka**, **Redis Lua distributed claim-checks**, and **JPA optimistic/pessimistic concurrency controls**.

---

## 🌟 Upstream Open Source Contributions

| Framework | Target Repository | Engineering Impact & Fix | Status |
| :--- | :--- | :--- | :--- |
| **Micrometer** | `micrometer-metrics/micrometer` | **Lock-Free Concurrency Fix**: Contributed a thread-safe update mechanism in `StepFunctionCounter` & `StepFunctionTimer` to prevent concurrent over-counting under heavy thread contention (`commit 6fa8bdc17`). Added deterministic multi-threaded unit tests. | [Under Review / Active PR](https://github.com/micrometer-metrics/micrometer) |
| **Resilience4j** | `resilience4j/resilience4j` | **Spring 6 Executor Aspect Thread Mode**: Fixed custom thread executor mode resolution (virtual threads vs. platform threads) across `RetryAspect` and `TimeLimiterAspect` in Spring Boot 3 / Spring 6 (`commit 4a3bd58`). Added deterministic aspect tests. | [Under Review / Active PR](https://github.com/resilience4j/resilience4j) |

---

## 🚀 Featured Engineering Projects

### 1. [Distributed Real-Time Notification Platform](https://github.com/yashsiwacha/Real-Time-Notification-System)
> *Production-grade event-driven notification infrastructure built with Spring Boot 3, Kafka, Redis, and WebSockets.*

- **Distributed Idempotency**: Engineered atomic `claim-check` mechanics via Redis Lua scripts (`claim.lua` / `complete.lua`), preventing race conditions on duplicate Kafka offsets during consumer rebalances.
- **Optimistic Concurrency**: Implemented JPA `@Version` optimistic locking to guarantee atomic database updates during simultaneous retry storms; benchmarked **1,000 concurrent update requests** with **0 race conditions**.
- **Performance & Latency**: Sustained **500+ events/sec** with sub-200ms p95 end-to-end delivery latency and **<25ms STOMP WebSocket dispatch latency**.
- **Observability**: Instrumenting cross-boundary correlation IDs (`X-Request-ID`) in MDC structured logs, custom Micrometer counters, and custom Grafana dashboard telemetry.
- **Stack**: Java 17, Spring Boot 3, Apache Kafka, Redis, PostgreSQL, STOMP WebSockets, Docker Compose, Render.

### 2. [High-Concurrency Auction Platform](https://github.com/yashsiwacha/Auction-System)
> *ACID-compliant concurrent bidding engine designed for zero data inconsistency under high bid volume.*

- **Concurrency Control**: Combined Java critical synchronization with pessimistic database locking (`SELECT FOR UPDATE`), eliminating race conditions in concurrent bid execution.
- **Stress-Tested Reliability**: Validated correctness under a **50-thread JMeter load profile (1,000+ bid events)** with zero double-allocation or state corruption.
- **Database Optimization**: Sub-50ms query execution achieved by eliminating N+1 query patterns via joined fetch strategies and composite indexing.
- **Stack**: Java 11/17, Spring Boot, Spring Security (JWT), MySQL/PostgreSQL, Thymeleaf, JMeter, Render.

### 3. [ProjectEcho — Career Intelligence Engine](https://github.com/yashsiwacha/project-echo)
> *Modular monolith architecture executing formal enterprise architecture standards (FGM, CIF, EAF).*

- **Architecture**: Domain-driven modular monolith enforcing clean boundary isolation across career evidence verification, metrics ingestion, and governance engines.
- **Stack**: Java 17, Spring Boot 3, Maven, Domain-Driven Design (DDD).

---

## 💼 Work Experience

**EPAM Systems** — *Junior Software Engineer Intern* `[Jan 2026 – Apr 2026]`
- **Database Optimization**: Reduced average query execution time by **40%** on high-traffic payment ledger tables via composite indexing and SQL query rewriting (`EXPLAIN ANALYZE`).
- **Idempotency & Reliability**: Implemented transaction idempotency validation with `@Transactional` rollback semantics, preventing double-submission payment errors during network retries.
- **API Extension**: Developed cursor-based pagination and `@Valid` request validation across REST endpoints with 30+ JUnit/Mockito tests integrated into GitHub Actions CI/CD.

---

## 🛠️ Technical Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | Java (17/21), SQL, C++, Python |
| **Backend Frameworks** | Spring Boot 3, Spring WebFlux, Spring Data JPA / Hibernate, REST APIs |
| **Distributed Systems** | Apache Kafka, Event-Driven Architecture, Redis Distributed Caching, Lua Scripts |
| **Databases** | PostgreSQL, MySQL, Redis, Query Optimization (`EXPLAIN ANALYZE`) |
| **Concurrency & Control** | Multithreading, CompletableFuture, Lock-Free Concurrency, Optimistic & Pessimistic Locking |
| **Observability & Testing**| Micrometer, Prometheus, Grafana, MDC Tracing, JUnit 5, Mockito, JMeter |
| **DevOps & Infrastructure**| Docker, Docker Compose, GitHub Actions CI/CD, AWS (EC2/S3), Render |

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
