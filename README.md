<h1 align="center">Hi there, I'm Khanh 👋</h1>

<p align="center">
  <b>Backend Developer · Spring Boot · Database Engineering</b>
</p>

<p align="center">
  <a href="https://github.com/NKhanh0908">
    <img src="https://komarev.com/ghpvc/?username=NKhanh0908&label=Profile%20views&color=0e75b6&style=flat" alt="profile views" />
  </a>
  <!-- TODO: Thêm badge LinkedIn nếu có -->
  <a href="https://www.linkedin.com/in/khanh-nguyen-quoc-13110a324"><img src="https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin" /></a>
</p>

---

##  About Me

-  I'm **Nguyen Quoc Khanh** — a 4th-year Computer Science student at **Saigon University**, based in **Ho Chi Minh City**
- Intern Backend Developer — actively learning and growing every day
- Deeply interested in **database internals** — from query optimization to scaling strategies
-  Exploring **system design** concepts: caching, messaging, and distributed patterns
-  Enjoy digging into how things work under the hood — not just making it run, but making it *right*
-  Reach me at: **khanhnq0908@gmail.com**
-  Fun fact: Nothing satisfies me more than turning a 3s query into a 30ms one 🚀

---

##  Featured Projects

###  [Human Resource Management (HRM)](https://github.com/NKhanh0908/hrm)
> A self-studied HRM system built to practice real-world backend architecture with Java & Spring Boot.

- **Employee Management** — REST APIs for managing employee profiles, departments, and organizational structure
- **Payroll Module** — Salary calculation logic with configurable rules, built from scratch based on self-research
- **Authentication & Authorization** — Secured with Spring Security, role-based access control per endpoint
- **Hands-on Learning** — Designed independently to understand how enterprise HR systems are structured; may not reflect all production-grade conventions, but built with intention to learn the right way

<details>
<summary> What I learned building this</summary>

- Structuring a multi-module Spring Boot project from scratch
- Designing relational schemas.
- Implementing JWT-based auth and role/permission management with Spring Security
- Handling global exceptions and clean REST API design with Spring MVC
- Understanding the gap between textbook knowledge and real-world backend conventions
- **Performance Optimization & Scalability**:
    - **Distributed Caching with Redis**: Implementing Cache-aside pattern to reduce database load for high-frequency read operations like Department lists and Employee profiles.
    - **Database Indexing & Partitioning Strategy**: Designing effective B-Tree and Composite indexes for complex HR queries; applying Horizontal Partitioning for historical payroll data (Salary History) to maintain performance as data grows.
    - **Query Optimization**: Analyzing execution plans (EXPLAIN ANALYZE) to eliminate N+1 problems and optimize heavy JOIN operations in reporting modules.
- **DevOps & Infrastructure**:
    - **Containerization with Docker**: Writing multi-stage Dockerfiles to create lightweight production images.
    - **Orchestration with Docker Compose**: Managing a full-stack local environment including Spring Boot app, MySQL, and Redis with seamless networking.
    - **Environment Configuration**: Managing externalized configurations for different environments (Dev, Staging, Prod).
</details>

---

### 🛒 [Sale Store Manager](https://github.com/kunengineer/sale-store-manager)
> A full-stack store management system — React frontend connected to a Spring Boot backend, built to explore end-to-end product development.

- 🖥️ **POS & Order Management** — Point-of-sale interface with real-time order tracking, area/table management, and customer handling
- 📦 **Product & Staff Management** — CRUD operations for products, staff, and customers with role-based access
- 📊 **Dashboard & Reports** — Sales overview and reporting module for business insights
- 🔗 **Full-stack Integration** — React frontend communicates with Spring Boot REST APIs; first hands-on experience connecting FE and BE end-to-end

<details>
<summary>📚 What I learned building this</summary>

- **Frontend (React)**:
  - Building SPA architecture with React Router v6 — nested routes and layout wrapping
  - Managing server state efficiently with React Query (stale time, cache strategy, retry policy)
  - Structuring reusable components and shared context with React Context API
  - HTML/CSS/JS fundamentals applied in a real UI — layouts, responsiveness, and event handling

- **Backend (Spring Boot)**:
  - Designing relational database schemas for a retail domain from scratch
  - Simplifying entity-to-DTO mapping with MapStruct — reducing boilerplate and improving maintainability
  - Building clean REST APIs consumed by a real frontend client

- **General**:
  - Understanding the full request lifecycle — from UI interaction to DB and back
  - Debugging cross-layer issues between frontend and backend

</details>
---

## 🛠️ Tech Stack

### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![Spring MVC](https://img.shields.io/badge/Spring_MVC-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![JPA/Hibernate](https://img.shields.io/badge/JPA_Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Databases & Caching
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

### Messaging & Real-time
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

### DevOps & Tools
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

---

##  What I'm Exploring

```
  Database Deep Dives    — Query execution plans, index strategies, slow query analysis
  Schema Design           — Normalization, partitioning, and planning for scale
  Caching Layer           — Redis for session, rate-limiting, and hot-data acceleration
  Event-Driven Systems    — Kafka for async messaging and decoupled architecture
  Distributed Patterns   — Microservices, Saga pattern, Outbox pattern (hands-on in banking project)
  Backend Fundamentals    — Spring Security, REST API design, exception handling
```

---

##  GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=NKhanh0908&show_icons=true&theme=tokyonight&hide_border=true" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=NKhanh0908&layout=compact&theme=tokyonight&hide_border=true" height="165" />
</p>

---

##  Let's Connect

<p align="left">
  <a href="https://github.com/NKhanh0908">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/khanh-nguyen-quoc-13110a324">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:khanhnq0908@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

<p align="center">
  <i>"Great code is built on a strong foundation — let's make systems that last!"</i>
</p>
