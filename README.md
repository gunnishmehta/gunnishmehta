<h1 align="center">Hi 👋, I'm Gunnish Mehta</h1>
<h3 align="center">Backend & Cloud Systems Engineer | Distributed Systems | Infrastructure Automation</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/gunnishmehta/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:work.gunnishmehta@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white"/></a>
</p>

---

### About Me

- 🎓 B.E. in Computer Engineering, Thapar Institute of Engineering and Technology
- 🏗️ I like designing systems that stay reliable under failure — retries, dead-letter queues, circuit breakers, and observability are recurring themes in my projects
- 🤝 Contributing to open source at [DSA-Meet-Design-Pilot](https://github.com/jkaus324/DSA-Meet-Design-Pilot) — a machine-coding/low-level-design interview-prep resource
- 🌱 Currently exploring **AWS Lambda** and **DynamoDB**
- 📫 Reach me at **work.gunnishmehta@gmail.com**

---

### 🚀 Featured Projects

**[Distributed Rate Limiter](https://github.com/gunnishmehta/Distributed-Rate-Limiter)** — `Node.js` `Express` `Redis` `Lua`
Redis-backed rate limiter implementing fixed window, sliding window log, and token bucket algorithms. Deliberately reproduced a real race condition in a naive check-then-act counter, proved it with a concurrency test (50/50 requests bypassed the limit), then fixed it atomically with a Lua/EVAL script (capped correctly at the limit). Also ships as a standalone, npm-installable Express middleware, verified by installing the packed `.tgz` into a separate project.

**[URL Shortener + Analytics](https://github.com/gunnishmehta/URL-Shortener-Analytics)** — `Node.js` `Express` `PostgreSQL` `Redis`
URL shortener with base62/random short-code strategies and a Redis cache-aside layer (~43% lower latency, ~57% higher throughput under load testing). Async click-analytics pipeline uses Redis Streams consumer groups for crash-safe delivery, with `XAUTOCLAIM` recovery on worker restart. Consumes the Distributed Rate Limiter above as a real npm dependency rather than reimplementing it.

**[Distributed Job Scheduler](https://github.com/gunnishmehta/job-scheduler)** — `Node.js` `Kafka` `Redis` `Docker`
Distributed job processing system using Kafka consumer groups for horizontal scaling with zero duplicate execution. Implements exponential backoff, dead-letter queues, and idempotent job submission via Redis-backed keys. Benchmarked throughput scaling ~1.87x by adding a worker.

**[API Gateway](https://github.com/gunnishmehta/api-gateway)** — `Node.js` `Express` `JWT` `Redis` `OpenTelemetry`
Reverse-proxy gateway centralizing authentication, rate limiting, and routing across backend services. Implements the circuit breaker pattern (closed/open/half-open) for fast failure during outages, with distributed tracing via OpenTelemetry and Jaeger.

---

### 🛠️ Other Projects

**[Observability Platform](https://github.com/gunnishmehta/observability-platform)** — `Node.js` `Kafka` `Prometheus` `Grafana`
Kafka-based log and metrics ingestion pipeline decoupling event capture from processing. Aggregates service metrics into Grafana dashboards via Prometheus, with threshold-based alerting to reduce mean time to detection.

**[Sketchy Squad](https://github.com/gunnishmehta/Sketchy-Squad-client)** ([server](https://github.com/gunnishmehta/Sketchy-Squad-server)) — `Node.js` `Express` `Socket.io`
Real-time multiplayer drawing-and-guessing game built with WebSockets for collaborative, low-latency gameplay.

**[campus_ride](https://github.com/gunnishmehta/campus_ride)** — `EJS` `Node.js`
E-cycle booking system for campus use, integrated with Google Sign-In and Razorpay for payments.

*Also worked freelance on **Estate Flow**, a full-stack real estate platform (React Native, Node.js, AWS Aurora, Docker) — client project, not publicly hosted.*

---

### 🧰 Tech Stack

**Languages:** C, C++, JavaScript, Python
**Backend & Frameworks:** Node.js, Express.js, React.js, React Native
**Cloud & Infra:** AWS, AWS Aurora, Docker, Kubernetes, CI/CD (GitHub Actions), Infrastructure as Code
**Data:** SQL, PostgreSQL, NoSQL, MongoDB, Redis
**Concepts:** Distributed Systems, REST APIs, Authentication & Authorization, Scalable Systems, Telemetry, Concurrency & Race Conditions, Lua (Redis scripting)
**Tools:** Git, Postman, JIRA, Linux

---

<p align="center"><i>Currently interested in Systems/Solutions Engineering roles at the intersection of distributed systems, cloud infrastructure, and automation.</i></p>
