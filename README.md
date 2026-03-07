# <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> John Basrai

**Senior Software Engineer**
*Rust & C++ · Systems & Distributed Architectures · High-Performance Applications*

## About Me

Senior systems engineer with **15+ years of experience** building backend and distributed systems, currently focused on **Rust** for high-assurance services spanning networking protocols, edge coordination, and authentication infrastructure. I care deeply about architectural clarity, explicit boundaries, and automated testing.

* 🌍 Yuba City, CA
* 🤝 Open to Rust-focused backend and distributed systems work

### Current Focus

- **[quelay](https://github.com/JohnBasrai/quelay)** — QUIC-based stream relay daemon in Rust for satellite and high-latency link environments. Implements priority scheduling via Deficit Round Robin, wire-level bandwidth enforcement, and lossless stream recovery. Validates BBR congestion control as a 4–5× throughput improvement over NewReno on degraded BLOS links.
- **[mom-rpc](https://github.com/JohnBasrai/mom-rpc)** — published Rust crate providing RPC over message-oriented middleware (AMQP, DDS, MQTT). Decouples application logic from broker mechanics while preserving explicit control over reliability, routing, and feature composition.

## 📌 Writing & Talks

- [Building Reliable Rust CI/CD: Lessons from Production Failures](https://www.linkedin.com/pulse/building-reliable-rust-cicd-lessons-from-production-john-basrai--wclhc/)
- [What the Cloudflare Outage Teaches Us About Production Rust](https://www.linkedin.com/pulse/what-cloudflare-outage-teaches-us-production-rust-john-basrai--7yquc/)

---

## 🛰️ Project Spotlight — quelay

QUIC-based stream relay daemon written in Rust, designed for satellite and high-latency link environments.

**Highlights**
- Priority scheduling via Deficit Round Robin with wire-level bandwidth enforcement
- Lossless stream recovery across link outages using a three-pointer spool buffer
- Retransmit accounting for accurate bandwidth allocation under degraded conditions
- Validates BBR as a 4–5× throughput improvement over NewReno (750 ms RTT, 5% packet loss)
- Maintains configured bandwidth allocation within ±3% under impairment
- Docker-based link simulation harness using `tc netem` for reproducible satellite testing

**Stack**: Rust, QUIC, Docker, `tc netem`

---

## 🧩 Selected Projects

| Repo | Focus |
| ---- | ----- |
| **[rust-edge-agent](https://github.com/JohnBasrai/rust-edge-agent)** | Embedded Linux edge agent: ARM64 cross-compilation, MQTT coordination via mom-rpc, reproducible CI |
| **[tokn](https://github.com/JohnBasrai/tokn)** | OAuth2/OIDC/JWT authorization server — RFC 6749/7519, token rotation, PostgreSQL, 10 security tests |
| **[axum-quickstart](https://github.com/JohnBasrai/axum-quickstart)** | Async REST APIs in Rust with WebAuthn/Passkeys, PostgreSQL, Redis, Prometheus |
| **[zkp-cp](https://github.com/JohnBasrai/zkp-cp)** | Chaum–Pedersen zero-knowledge proofs in Rust (gRPC, tonic) |
| **[cr8s](https://github.com/JohnBasrai/cr8s)** | Rocket backend with JWT auth, role-based access, SQLx migrations, full integration testing |
| **[mempool-vortex](https://github.com/JohnBasrai/mempool-vortex)** | Ethereum mempool monitoring and latency analysis in Rust |

---

## 🛠️ Technical Focus

**Systems & Architecture**
- High-latency and satellite link protocols (QUIC, BBR, RTP)
- Secure sandboxed execution (Linux namespaces, cgroups v2)
- Message-oriented middleware and edge coordination (MQTT, AMQP, DDS)
- Explicit control/data-plane separation

**Languages & Runtime**
- Rust (async, networking, systems)
- C / Modern C++
- Python, SQL, WebAssembly

**Infrastructure & Observability**
- PostgreSQL, Redis, Docker
- Prometheus, Grafana, Loki

**Testing & CI**
- Integration-heavy testing strategies
- Security-focused test coverage
- GitHub Actions & GitLab CI

---

## 📋 Architecture Patterns

**[Explicit Module Boundary Pattern (EMBP)](https://github.com/JohnBasrai/architecture-patterns/blob/main/rust/embp.md)**

A documented Rust pattern for enforcing architectural boundaries while preserving refactor freedom.

---

## 🤝 Let's Connect

If you're hiring for backend, distributed systems, or Rust-focused roles, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/johnbasrai/) or here on GitHub.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnbasrai/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/JohnBasrai)
