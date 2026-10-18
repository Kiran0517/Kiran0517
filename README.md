# Kiran Reddy

### Full-stack engineer building real-time applications and reliable backend systems.

[Portfolio](https://portfolio-kiranreddy.vercel.app/) · [LinkedIn](http://www.linkedin.com/in/bodhireddykiranreddy) · [Email](mailto:kiranreddy321ms@gmail.com)

I work across **React / TypeScript interfaces**, **Java / Spring Boot and Node.js services**, and the databases and infrastructure behind them. I enjoy the parts where those layers meet: getting live data onto a dashboard, finding out why an API slowed down, or making a retry safe.

Currently building user-facing workflows and backend services at **Saayam For All**. Previously, I worked on real-time analytics at **Swapt** and distributed services at **Tata Consultancy Services**.

Based in **Boston, MA** · **M.S. Information Systems, Northeastern University**

---

## Featured work

### [Incident Lab](https://github.com/Kiran0517/incident-lab)
An order platform I deliberately break to understand how distributed systems fail.

`Java 21` `Spring Boot` `PostgreSQL` `Docker` `OpenTelemetry` `k6` `Toxiproxy`

I built three services for orders, inventory, and payments, instrumented them with traces, metrics, and structured logs, then tested bad deployments, network latency, and service crashes.

- Sustained approximately **1,200 orders/sec at p95 below 50 ms** in k6 load tests with 20 virtual users and **3M+ historical records**.
- Traced a **41× throughput drop** to a missing database index and verified recovery after rollback.
- Found **119 orders stuck after successful payments**. Added an explicit unknown-payment state and reconciliation, then repeated the experiment: **119 stuck orders → 0**.

**What made it interesting:** the most useful bugs weren't the ones I planted. The experiments exposed port exhaustion, an observability outage, and a timeout-handling bug introduced by an earlier fix.

### [Cosmo Plan](https://github.com/Kiran0517/My-Personal-Projects-/tree/main/CosmoPlan-DMDD-main)
A full-stack space exploration management application with tenant-aware services and role-based access.

`React` `Java` `Spring Boot` `PostgreSQL` `Redis` `Jest` `Cypress`

- Designed multi-tenant backend services with OAuth 2.0 / JWT access control.
- Used PostgreSQL indexing and Redis caching to achieve **sub-100 ms indexed queries across 500K+ records**.
- Added automated application tests and a GitHub Actions pipeline.

### NestKnowledge
A learning platform built with React, Node.js, MongoDB, and AWS.

`React` `Node.js` `MongoDB` `Redis` `AWS` `GitHub Actions`

- Scaled to **10,000+ users** with Redis-cached reads and EC2 autoscaling.
- Kept peak-traffic **p95 time-to-first byte below 500 ms**.
- Integrated Cypress end-to-end tests into CI/CD to catch regressions before deployment.

---

## My stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-20232A?style=flat-square&logo=nextdotjs&logoColor=white)
![Java](https://img.shields.io/badge/Java-E76F00?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

- **Frontend:** React, Next.js, TypeScript, JavaScript, React Native.
- **Backend & data:** Java, Spring Boot, Node.js, Python, Go, REST, GraphQL, WebSockets, PostgreSQL, MongoDB, Redis, Kafka.
- **Cloud & delivery:** AWS, Docker, Kubernetes, GitHub Actions, Jenkins, Maven.
- **Testing & observability:** Jest, Cypress, k6, Toxiproxy, OpenTelemetry, Prometheus, Jaeger, Grafana, Datadog.

## How I work

**Start with the workflow.** At Swapt, customer feedback came through our product lead. I used it to guide frontend and backend improvements, including dashboards with reporting delays under three seconds.

**Measure the whole path.** A fast interface depends on rendering, APIs, queries, and infrastructure. I like following that path rather than guessing where the bottleneck is.

**Verify the fix.** A passing health check isn't enough. I repeat the load or failure conditions that exposed the problem. I also use Claude Code, Cursor, and GitHub Copilot for test drafting and debugging, and review the generated code.

---

If you're working on full-stack products, real-time systems, or reliability problems, [let's connect](http://www.linkedin.com/in/bodhireddykiranreddy).
