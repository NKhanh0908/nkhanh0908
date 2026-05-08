<div align="center">

# Nguyen Quoc Khanh
### Java Backend Developer · Database Engineering · System Design

[![Profile Views](https://komarev.com/ghpvc/?username=NKhanh0908&label=Profile%20views&color=1a3a5c&style=flat)](https://github.com/NKhanh0908)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/khanh-nguyen-quoc-13110a324)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:khanhnq0908@gmail.com)

</div>

---

## About Me

4th-year **Information Systems** student at Saigon University (GPA 8.0/10.0), with 5 months of backend internship experience at **VINIPR**. I focus on building systems that are not just functional, but correct — from query execution plans to service layer design.

What drives me: turning a 3-second query into a 30ms one, designing service boundaries that survive change, and understanding *why* something works, not just *that* it works.

**Short-term goal:** Join a backend team where I can contribute to production systems and deepen expertise in distributed architecture within the next year.  
**Long-term goal:** Grow into a Senior Backend Engineer specializing in high-performance, scalable systems.

---

## Work Experience

### Backend Java Developer Intern — VINIPR CO., LTD.
`Aug 2025 – Dec 2025 · Ho Chi Minh City`

- Designed and maintained **20+ RESTful APIs** across 3 e-commerce modules (product, order, user management) using Spring Boot + MySQL, documented with Swagger for team-wide clarity
- Collaborated in an **Agile/Scrum** team across 4 sprint cycles — daily stand-ups, peer code reviews, sprint planning
- Refactored legacy service classes and resolved **N+1 query patterns** using SOLID principles, reducing redundant DB calls across core modules
- Used **AI-assisted tools** (GitHub Copilot / Claude) to accelerate scaffolding and code review cycles

---

## Featured Projects

### Dating Website
`Spring Boot · Spring Security · JWT · WebSocket (STOMP) · Redis · MySQL · ReactJS`  
`Feb 2026 – Present · Team of 3 (Fullstack)` · [GitHub](https://github.com/NKhanh0908/dating-website)

A real-time dating platform — the main challenge was building low-latency communication and a fast discovery search over a large user dataset.

**What I built & why it matters:**

| Area | What I did | Result |
|------|-----------|--------|
| Real-time Chat | Replaced HTTP polling with **WebSocket (STOMP)**; secured handshake with JWT interception | Bidirectional low-latency messaging |
| Auth & Security | Spring Security + JWT + custom rate-limiting filter on sensitive endpoints | Brute-force protection on login/match endpoints |
| Discovery Search | Composite index on `(gender, age, city)` + Redis profile caching on high-traffic endpoints | Response time ~55ms → ~5ms on 50k rows (verified via `EXPLAIN ANALYZE`) |
| Reliability | Unit & integration tests with **JUnit 5 + Mockito** covering matching logic and auth flows | Regression bugs reduced across core flows |

<details>
<summary>Technical decisions & tradeoffs</summary>

**Why WebSocket over polling?**  
Polling creates unnecessary DB reads and HTTP overhead at scale. WebSocket gives us a persistent connection with far lower latency, at the cost of connection state management — a worthwhile tradeoff for a chat feature.

**Why composite index on `(gender, age, city)` and not separate indexes?**  
MySQL's index merge is often less efficient than a well-ordered composite index for multi-column filter queries. By ordering columns from lowest to highest cardinality in the discovery query pattern, the composite index allows the engine to skip large portions of the table in a single B-tree traversal.

**Why Redis cache-aside and not write-through?**  
User profiles are read far more often than they are updated. Cache-aside lets us populate the cache lazily on reads and invalidate on writes, without paying the write overhead on every profile update.

</details>

---

### Human Resource Management System (ERP)
`Spring Boot · Spring Security · Data JPA · Redis · JavaMail · Cloudinary · Docker · Grafana`  
`Jun 2025 – Jul 2025 · Personal Project` · [GitHub](https://github.com/NKhanh0908/hrm)

A self-studied full ERP system covering the complete employee lifecycle. Built independently to close the gap between academic knowledge and real-world backend architecture.

**Scope:** 5 modules · 30+ REST endpoints

| Module | Key Implementation |
|--------|--------------------|
| Recruitment | Job posting → application → offer pipeline via REST |
| Employee | Profile management, department/org structure |
| Attendance | Tracking with configurable rules |
| Payroll | Salary calculation engine with configurable rules; batch job monitored via Grafana |
| Training | Course assignment and completion tracking |

**Engineering highlights:**

- **SOLID architecture:** Loosely coupled service interfaces — new ERP modules plug in without modifying existing logic
- **Security:** RBAC via Spring Security across all modules; OTP recovery with Redis TTL + brute-force lockout + async email (JavaMail)
- **Observability:** Spring Actuator + Grafana dashboards for JVM memory, HTTP throughput, and payroll batch job performance — catching degradation before it becomes an incident
- **Infrastructure:** Multi-stage Dockerfile for lightweight prod images; Docker Compose managing app + MySQL + Redis with proper network isolation

<details>
<summary>What I learned that surprised me</summary>

- **Schema design under change:** HR domains look simple until you model historical salary data. Horizontal partitioning for `salary_history` by year prevented the table from becoming a performance bottleneck as data grew.
- **The gap between "working" and "maintainable":** Refactoring God Service classes mid-project taught me more about SOLID than any textbook. When you feel the pain of a 400-line service class during a feature addition, the principles stop being abstract.
- **Observability is not optional:** Adding Grafana late in the project showed me metrics I hadn't noticed — a payroll batch job that spiked memory predictably at month-end. Monitoring revealed behavior that code review never could.

</details>

---

## Tech Stack

### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![JPA/Hibernate](https://img.shields.io/badge/JPA_Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-764ABC?style=flat-square&logo=redux&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

### Databases & Caching
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

### Messaging & Real-time
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat-square&logo=socketdotio&logoColor=white)

### DevOps & Observability
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black)

### AI-Augmented Development
![Claude](https://img.shields.io/badge/Claude-CC785C?style=flat-square&logo=anthropic&logoColor=white)
![GitHub Copilot](https://img.shields.io/badge/GitHub_Copilot-000000?style=flat-square&logo=github&logoColor=white)

*Using AI tools for code scaffolding, refactoring, and review — with an emphasis on understanding the output, not just accepting it.*

---

## Currently Exploring

```
Database Internals     Query execution plans, index strategies, B-tree mechanics
Schema Design          Normalization trade-offs, partitioning for write-heavy tables  
Event-Driven Systems   Kafka for async decoupling, Outbox pattern for reliability
Distributed Patterns   Saga pattern, idempotency, eventual consistency
Microservices          Service decomposition, inter-service auth, API gateway patterns
```

---

## Education

**Saigon University** · Bachelor of Information Systems · `2022 – Present`  
GPA: **8.0 / 10.0**

Coursework: OOP · Data Structures & Algorithms · Database Systems · MVC Architecture · RESTful API Design · Enterprise Software Development

Academic research: *Prompt engineering for AI-assisted software development* — optimizing developer workflows with LLM tools, based on English-language technical sources.

---

<div align="center">

*"Great code is built on a strong foundation — let's make systems that last."*

**Open to Junior / Mid Backend Java Developer opportunities in Ho Chi Minh City.**

</div>
