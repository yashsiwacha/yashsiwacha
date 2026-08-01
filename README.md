<div align="center">
  <!-- TODO: Replace with the generated banner -->
  <img src="./assets/banner.png" alt="Yash Siwach" width="100%" />

  # Yash Siwach
  
  **Backend Engineer focused on Java, Spring Boot, Kafka and Distributed Systems.**
  
  <p>
    <a href="https://linkedin.com/in/yashsiwacha">LinkedIn</a> • 
    <a href="mailto:yashsiwach07@gmail.com">Email</a> • 
    <a href="https://github.com/yashsiwacha">Portfolio</a>
  </p>
</div>

---

## About Me

I'm a Backend Engineer focused on Java, Spring Boot, PostgreSQL, Redis and Kafka. 

I enjoy designing reliable backend systems, learning distributed systems, and contributing to open source projects like Resilience4j and Micrometer.

---

## Current Focus

**Currently Exploring**
- Distributed Systems
- JVM Internals
- Spring Ecosystem
- Observability
- Open Source

---

## Engineering Principles

- **Design for failure**: Expect network partitions, timeouts, and hardware failures.
- **Measure before optimizing**: Rely on metrics and profiles, not intuition.
- **Prefer simplicity over cleverness**: Code is read vastly more often than it is written.
- **Write tests that reproduce bugs**: Prevent regressions through deterministic testing.
- **Build observable systems**: If it's in production, it must emit metrics, logs, and traces.

---

## Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | Java (17/21), C++, SQL |
| **Backend & Frameworks** | Spring Boot, Spring WebFlux, Hibernate, REST APIs |
| **Distributed Systems** | Apache Kafka, Redis, gRPC |
| **Databases** | PostgreSQL, MySQL |
| **Infrastructure** | Docker, AWS (EC2, S3), CI/CD (GitHub Actions) |

---

## Open Source

**[Resilience4j](https://github.com/resilience4j/resilience4j)**
- Submitted PR improving Spring 6 executor creation.
- Added regression tests.
- *Currently under review.*

**[Micrometer](https://github.com/micrometer-metrics/micrometer)**
- Submitted lock-free concurrency fix.
- Added deterministic multithreaded regression tests.
- *Currently under review.*

---

## Featured Projects

### [Distributed Notification System](https://github.com/yashsiwacha/Real-Time-Notification-System)
- **Problem**: High-throughput events were being lost during downstream service outages, leading to inconsistent notification delivery.
- **Solution**: Designed an asynchronous, event-driven producer-consumer architecture using Dead Letter Queues (DLQ) and exponential backoff retries.
- **Impact**: Achieved reliable delivery for ~500 events/sec with sub-200ms p95 latency.
- **Technologies**: Java, Spring Boot, Kafka, Redis

### [Concurrent Auction System](https://github.com/yashsiwacha/Auction-System)
- **Problem**: Race conditions occurred when multiple users attempted to place bids on the same auction simultaneously.
- **Solution**: Implemented ACID-compliant transactions with precise database-level locking and application-level synchronization to guarantee data integrity.
- **Impact**: Successfully supported 50+ simultaneous concurrent bids per entity with zero data inconsistency.
- **Technologies**: Java, Spring Boot, MySQL

### [Distributed Cache Server](https://github.com/yashsiwacha/distributed-cache-server)
- **Problem**: Needed a highly concurrent, low-latency key-value store for rapid data retrieval without heavy database reliance.
- **Solution**: Developed a custom TCP socket server from scratch, implementing TTL expiration and LRU eviction policies.
- **Impact**: Handled multi-client concurrent requests efficiently without blocking read threads during asynchronous persistence snapshots.
- **Technologies**: C++, STL, POSIX Threads, Mutexes

### [Low Latency Order Management System](https://github.com/yashsiwacha/low-latency-order-management)
- **Problem**: Financial trading engine required near-instantaneous execution of buy/sell/cancel orders under heavy load.
- **Solution**: Built a thread-safe concurrent order book utilizing efficient price-time priority matching logic.
- **Impact**: Minimized lock contention and optimized memory management to ensure real-time trade execution.
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
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashsiwacha&layout=compact&theme=transparent&hide_border=true&title_color=ffffff&text_color=a0a0a0" height="150" alt="Top Languages" />
</div>
