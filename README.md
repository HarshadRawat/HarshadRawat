<h1 align="center">Hi, I'm Harshad Rawat 👋</h1>

<p align="center">
  <b>Java Backend Developer</b> · Spring Boot · REST APIs · Distributed Systems Basics<br/>
  Bengaluru, India · Open to SDE / Java Developer roles
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/harshad-rawat-011406292"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:harshadrawat157@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://drive.google.com/file/d/1Xgpc4VQ2NeM81n5LkFrjUALpZd2zvHPE/view?usp=drive_link"><img src="https://img.shields.io/badge/Resume-View-2ea44f" alt="Resume"/></a>
</p>

---

I build backend systems that handle the hard parts: **concurrency, security, and real-time delivery**. I write down why I made each design decision and measure the results instead of guessing.

## 🚀 Featured Projects

### 🩸 [LifeLink](https://github.com/HarshadRawat/lifelink-blood-donor-system): Emergency Blood Donor Response Platform
`Java 17` `Spring Boot 4` `MySQL` `Redis` `RabbitMQ` `WebSocket (STOMP)` `Docker` `GitHub Actions`

Hospitals raise an emergency request and compatible donors nearby get alerted in real time.

- **9.3x faster matching** (116 ms → 12.5 ms median) on 100,000 donors, using a two-tier approach: an indexed bounding-box query in MySQL, then exact Haversine distance in the JVM. Benchmark method and results are in [`docs/BENCHMARK.md`](https://github.com/HarshadRawat/lifelink-blood-donor-system/blob/main/docs/BENCHMARK.md).
- **Prevents over-fulfilment** when many donors accept at once, using `SELECT ... FOR UPDATE` row locking. Verified with a 32-thread concurrency test.
- **Event-driven alerts** through RabbitMQ with retry backoff and a dead-letter queue, pushed to donors over STOMP WebSockets.
- **Security hardening:** 15-minute JWTs, refresh-token rotation with reuse detection, account lockout, and consent-based contact sharing.
- **Engineering practice:** 22 Architecture Decision Records, 250+ backend tests, CI with coverage and Trivy scanning, and Flyway migrations.

[Live demo](https://lifelink-blood-donor-system.vercel.app) · [API docs](https://lifelink-blood-donor-system.onrender.com/swagger-ui.html) · [Design decisions](https://github.com/HarshadRawat/lifelink-blood-donor-system/blob/main/DECISIONS.md)

---

### 🎫 [HelpDesk](https://github.com/HarshadRawat/helpdesk-backend): IT Ticket Management System
`Java` `Spring Boot` `Spring Security` `JWT` `JPA/Hibernate` `MySQL`

REST API for an ITSM portal with role-based workspaces for employees, IT agents, and admins.

- JWT authentication with BCrypt, role-based access (`CUSTOMER` / `AGENT` / `ADMIN`), and ownership checks.
- Ticket lifecycle with controlled status transitions, SLA tracking, and **optimistic locking** that returns `409 Conflict` when two agents edit the same ticket.
- Admin audit trail with before/after diffs, pagination, filtering, and centralized exception handling.
- Refresh-token flow for stateless sessions, with the API deployed on Railway and documented in Swagger UI.

[Backend repo](https://github.com/HarshadRawat/helpdesk-backend) · [Live app](https://harshadrawat.github.io/helpdesk-frontend/) · [Swagger](https://helpdesk-backend-production-7f4522ed.up.railway.app/swagger-ui/index.html)


## 🛠️ Tech Stack

| | |
|---|---|
| **Languages** | ![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?logo=mysql&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white) |
| **Backend** | ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?logo=springsecurity&logoColor=white) ![Hibernate](https://img.shields.io/badge/Hibernate-59666C?logo=hibernate&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?logo=jsonwebtokens&logoColor=white) |
| **Data & Messaging** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?logo=rabbitmq&logoColor=white) |
| **DevOps & Tools** | ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white) |

**Core CS:** Data Structures & Algorithms · OOP · DBMS · Computer Networks · System Design fundamentals

## 📈 Problem Solving

[![LeetCode](https://img.shields.io/badge/LeetCode-Harshad__Rawat12-FFA116?logo=leetcode&logoColor=white)](https://leetcode.com/u/Harshad_Rawat12/) &nbsp; **271 problems solved**

## 🎓 Education

**Bachelor of Engineering in Computer Science & Engineering**, Acharya Institute of Technology (2023 – 2027)

## 🌱 Currently

- Deepening system design: caching, message queues, and consistency trade-offs
- Adding the Transactional Outbox pattern to LifeLink
- Practising DSA on LeetCode

## 📫 Let's talk

I'm looking for **Software Development Engineer / Java Backend** roles. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/harshad-rawat-011406292) or [email](mailto:harshadrawat157@gmail.com).
