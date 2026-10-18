# Kiran Reddy

### Full-stack engineer building real-time applications and reliable backend systems.

[Portfolio](https://portfolio-kiranreddy.vercel.app/) · [LinkedIn](http://www.linkedin.com/in/bodhireddykiranreddy) · [Email](mailto:kiranreddy321ms@gmail.com)

I work across **React / TypeScript interfaces**, **Java / Spring Boot and Node.js services**, and the databases and infrastructure behind them. I enjoy the parts where those layers meet: getting live data onto a dashboard, finding out why an API slowed down, or making a retry safe.

Currently building user-facing workflows and backend services at **Saayam For All**. Previously, I worked on real-time analytics at **Swapt**, reducing analytics p95 latency by **40% (800 ms → 480 ms)**, and distributed services at **Tata Consultancy Services**.

Based in **Boston, MA** · **M.S. Information Systems, Northeastern University**

---

## Featured work

### [Incident Lab](https://github.com/Kiran0517/incident-lab)
An order platform I deliberately break, and an LLM agent that investigates the failures.

`Java 21` `Spring Boot` `PostgreSQL` `Python` `Gemini API` `OpenTelemetry` `Prometheus` `Jaeger` `k6` `Toxiproxy` `Docker`

I built three services for orders, inventory, and payments, instrumented them with traces, metrics, and structured logs, then tested bad deployments, network latency, and service crashes under load.

- Sustained approximately **1,200 orders/sec at p95 below 50 ms** in k6 load tests with 20 virtual users and **3M+ historical records**.
- Traced a **41× throughput drop** to a missing database index and verified recovery after rollback.
- Found **119 orders stuck after successful payments**. Added an explicit unknown-payment state and reconciliation, then repeated the experiment: **119 stuck orders → 0**.
- Built an **LLM agent with function calling** over read-only tools for metrics, traces, logs, and deploy history. Its first diagnosis of a live latency incident blamed the wrong service; I disproved it, tightened its reasoning, and the re-run found the actual cause.

**What made it interesting:** the most useful bugs weren't the ones I planted. The experiments exposed port exhaustion, an observability outage, and a timeout-handling bug introduced by an earlier fix.

### [Cosmo Plan](https://github.com/Kiran0517/My-Personal-Projects-/tree/main/CosmoPlan-DMDD-main)
A space exploration management application with a relational data model.

`Java` `SQL` `Database Design`

- Organizes agencies, astronauts, missions, spacecraft, launch sites, launch vehicles, and payloads through dedicated application modules.
- Includes entity-relationship diagrams, logical data models, and database design documentation alongside the source code.

### [NestKnowledge](https://github.com/Kiran0517/My-Personal-Projects-/tree/main/NestKnowledge%20-%20A%20Free%20Learning%20and%20Teaching%20Platform)
A learning platform built with React, Node.js, MongoDB, and AWS.

`React` `Node.js` `MongoDB` `Redis` `AWS` `GitHub Actions`

- Scaled to **10,000+ users** with Redis-cached reads and EC2 autoscaling.
- Kept peak-traffic **p95 time-to-first byte below 500 ms**.
- Integrated Cypress end-to-end tests into CI/CD to catch regressions before deployment.

---

## My stack

- **Frontend:** React, Next.js, TypeScript, JavaScript, React Native.
- **Backend & data:** Java, Spring Boot, Node.js, Python, Go, REST, GraphQL, WebSockets, PostgreSQL, MongoDB, Redis, Kafka.
- **Cloud & delivery:** AWS, Docker, Kubernetes, GitHub Actions, Jenkins, Maven.
- **Testing & observability:** Jest, Cypress, k6, Toxiproxy, OpenTelemetry, Prometheus, Jaeger, Grafana, Datadog.

## Verify the fix

A passing health check isn't enough. I repeat the load or failure conditions that exposed the problem. I also use Claude Code, Cursor, and GitHub Copilot for test drafting and debugging, and review the generated code.

---

If you're working on full-stack products, real-time systems, or reliability problems, [let's connect](http://www.linkedin.com/in/bodhireddykiranreddy).
