<div align="center">
  <!-- TODO: Replace with the generated banner -->
  <img src="./assets/banner.png" alt="Yash Siwach" width="100%" />

  # Yash Siwach
  
  **Backend Engineer • Java • Spring Boot • Kafka • PostgreSQL**
  <br>
  Building reliable backend systems and contributing to Open Source.
  
  <p>
    <a href="https://linkedin.com/in/yashsiwacha">LinkedIn</a> • 
    <a href="mailto:yashsiwach07@gmail.com">Email</a> • 
    <a href="https://yashsiwacha.github.io/Portfolio/">Portfolio</a>
  </p>
</div>

---

## About Me

I'm a Backend Engineer focused on Java, Spring Boot, PostgreSQL, Redis and Kafka. 

I enjoy designing reliable distributed systems, building robust backend architectures, and contributing to open source projects like Resilience4j and Micrometer. My work emphasizes system reliability and observability to ensure services run smoothly in production.

---

## Recent Work

- **Micrometer**: Contributed a lock-free concurrency fix (currently under review).
- **Resilience4j**: Contributed a Spring 6 executor configuration fix (currently under review).
- **Notification System**: Built a reliable event-driven delivery system handling ~500 events/sec.

---

## Current Focus

**Currently Exploring**
- Distributed Systems
- JVM Internals
- Spring Ecosystem
- Observability
- Open Source

---

## Experience

**EPAM Systems**
*Junior Software Engineer Intern*
Focused on production backend systems engineering, improving concurrent request processing, and increasing system reliability through structured debugging and performance tuning.

---

## Engineering Principles

1. **Design for failure**: Expect network partitions, timeouts, and hardware failures.
2. **Build observable systems**: If it's in production, it must emit metrics, logs, and traces.
3. **Measure before optimizing**: Rely on metrics and profiles, not intuition.
4. **Prefer simplicity over cleverness**: Code is read vastly more often than it is written.
5. **Write tests that reproduce bugs**: Prevent regressions through deterministic testing.

---

## Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | Java (17/21), C++, SQL |
| **Backend & Frameworks** | Spring Boot, Spring WebFlux, Hibernate, REST APIs |
| **Distributed Systems** | Apache Kafka |
| **Databases & Caching** | PostgreSQL, MySQL, Redis |
| **Infrastructure** | Docker, CI/CD (GitHub Actions) |

---

## Open Source

**[Resilience4j](https://github.com/resilience4j/resilience4j)**
- Contributed a Spring 6 executor configuration fix.
- Added deterministic regression tests.
- *PR currently under review.*

**[Micrometer](https://github.com/micrometer-metrics/micrometer)**
- Contributed a lock-free concurrency fix.
- Added deterministic multithreaded regression tests.
- *PR currently under review.*

---

## Featured Projects

### [Distributed Notification System](https://github.com/yashsiwacha/Real-Time-Notification-System)
*Asynchronous, event-driven producer-consumer architecture.*
- **Impact**: Achieved reliable delivery for ~500 events/sec with sub-200ms p95 latency.
- **Engineering**: Designed resilient delivery using Dead Letter Queues (DLQ) and exponential backoff retries.
- **Technologies**: Java, Spring Boot, Kafka, Redis

### [Concurrent Auction System](https://github.com/yashsiwacha/Auction-System)
*ACID-compliant bidding engine designed for high concurrency.*
- **Impact**: Supported 50+ simultaneous concurrent bids per entity with zero data inconsistency.
- **Engineering**: Prevented race conditions using precise database-level locking and application-level synchronization.
- **Technologies**: Java, Spring Boot, MySQL

### [Distributed Cache Server](https://github.com/yashsiwacha/distributed-cache-server)
*Custom highly concurrent, low-latency key-value store.*
- **Impact**: Handled multi-client concurrent requests efficiently without blocking read threads.
- **Engineering**: Developed a custom TCP socket server with TTL expiration, LRU eviction, and asynchronous persistence.
- **Technologies**: C++, STL, POSIX Threads, Mutexes

### [Low Latency Order Management System](https://github.com/yashsiwacha/low-latency-order-management)
*Thread-safe concurrent order book for near-instantaneous execution.*
- **Impact**: Minimized lock contention and optimized memory management to ensure real-time trade execution.
- **Engineering**: Utilized efficient price-time priority matching logic under heavy load.
- **Technologies**: C++, STL, Concurrency

---

## Currently Learning

- JVM Internals
- Java Concurrency
- Spring Source Code
- Distributed Systems
- Observability

---

## GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=yashsiwacha&show_icons=true&theme=transparent&hide_border=true&title_color=ffffff&icon_color=ffffff&text_color=a0a0a0" height="150" alt="GitHub Stats" />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=yashsiwacha&theme=transparent&hide_border=true&color=ffffff&line=58A6FF&point=ffffff&hide_title=true" height="250" alt="Contribution Graph" />
</div>
