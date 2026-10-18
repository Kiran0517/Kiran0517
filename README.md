<div align="center">

# Hi, I'm Kiran Reddy

### Full-stack software engineer · Backend systems · Reliability

I build user-facing applications and the systems that keep them reliable.

[Portfolio](https://portfolio-kiranreddy.vercel.app/) · [LinkedIn](http://www.linkedin.com/in/bodhireddykiranreddy) · [Email](mailto:kiranreddy321ms@gmail.com)

Boston, MA · M.S. Information Systems, Northeastern University

</div>

---

## About me

My work spans React and TypeScript interfaces, Java/Spring Boot and Node.js services, real-time data pipelines, and cloud deployments. I enjoy following a problem across the stack: from a slow dashboard to its API calls, database queries, and infrastructure metrics.

At **Saayam For All**, I build user-facing workflows and backend services. Previously, I worked on **Swapt**, a B2B post-purchase SaaS platform, and supported distributed services at **Tata Consultancy Services**. My work has included reducing analytics p95 latency from **800 ms to 480 ms**, delivering dashboard updates in **under 3 seconds**, and improving deployment workflows.

## Projects worth exploring

### [Incident Lab](https://github.com/Kiran0517/incident-lab)
**Build it. Break it. Understand it. Prove the fix.**

A three-service order platform for investigating distributed-system failures through load testing, fault injection, and observability.

- **Build:** Java 21, Spring Boot, PostgreSQL, Maven, and Docker Compose, with concurrency-safe stock reservations and idempotent retries.
- **Observe:** OpenTelemetry traces, Prometheus metrics, Jaeger, Grafana, and structured logs.
- **Measure:** Approximately **1,200 orders/second** at **p95 below 50 ms** in k6 load tests with 20 virtual users and **3M+ historical records**.
- **Investigate:** A dropped index cut throughput **41×** while requests still returned without errors. Database analysis and connection-pool metrics exposed the bottleneck; rollback restored performance.
- **Fix:** Made uncertain payment outcomes explicit and built reconciliation. Repeating the payment-timeout experiment reduced silently stuck orders from **119 to 0**; reconciliation resolved **483 ambiguous orders** across experiments.

The lesson I keep coming back to: **a timeout doesn't prove an operation failed.**

### [Cosmo Plan](https://github.com/Kiran0517/My-Personal-Projects-/tree/main/CosmoPlan-DMDD-main)
**Multi-tenant application design, access control, and database performance.**

A space exploration management project built with React, Java, Spring Boot, PostgreSQL, and Redis.

- Designed multi-tenant services with indexed queries completing in **under 100 ms across 500K+ records**.
- Implemented role-based access control with OAuth 2.0 and JWT.
- Automated application testing with Jest and Cypress through GitHub Actions.

## Tools I work with

- **Languages & interfaces:** Java, TypeScript, JavaScript, Python, Go, SQL, React, Next.js.
- **Services & data:** Spring Boot, Node.js, REST, GraphQL, WebSockets, PostgreSQL, MySQL, MongoDB, Redis, Kafka.
- **Cloud & delivery:** AWS, Docker, Kubernetes, GitHub Actions, Jenkins, Maven.
- **Testing & observability:** Jest, Cypress, k6, Toxiproxy, OpenTelemetry, Prometheus, Jaeger, Grafana, Datadog.

## How I approach engineering

- **Follow the evidence.** Use traces, logs, metrics, and database records to test explanations for failures.
- **Close the loop.** Repeat the conditions that exposed a bug to verify the fix.
- **Listen, then iterate.** Translate stakeholder requirements and customer feedback into concrete application improvements.
- **Review what AI produces.** I use Claude Code, Cursor, and GitHub Copilot to draft tests and debug failures, and review the generated code.

---

Interested in full-stack development, backend performance, or reliability engineering? [Let's connect.](http://www.linkedin.com/in/bodhireddykiranreddy)
