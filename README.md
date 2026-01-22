# <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> John Basrai

**Senior Software Engineer**<br>
*Rust & C++ · Backend Systems · Distributed Architectures · CI/CD · High-Performance Applications*

## <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> About Me

Solution-oriented, results-driven software engineer with **15+ years of experience** in systems and backend development — currently specializing in **Rust** for authentication infrastructure, backend systems, and high-assurance applications. Skilled in Rust, Modern C++, and Python, with strong focus on architectural clarity, modularity, and automated testing.

* 🌍 Based in Yuba City, CA
* 🤝 Open to collaborating on backend systems, authentication infrastructure, or distributed systems in Rust

### Current Focus

Currently developing **[tokn](https://github.com/JohnBasrai/tokn)** (OAuth2/OIDC/JWT authorization server) and integrating **WebAuthn/Passkeys** into axum-quickstart. Implementing RFC 6749/7636 compliance with automated protocol testing (10 security test scenarios covering PKCE, token rotation, scope enforcement). Applying cr8s CI/CD patterns to containerized authentication services.

Designing a real-time audio streaming system in Rust — **[rtp-opus-streamer](https://github.com/JohnBasrai/rtp-opus-streamer)**
 — using RTP (RFC 3550) and Opus (RFC 6716). This work explores end-to-end systems behavior from audio capture through network transport to playback, with emphasis on production concerns such as network resilience, observability, and adaptive behavior under constrained conditions.

## 📌 Featured
👉 [📝 "Building Reliable Rust CI/CD: Lessons from Production Failures"](https://www.linkedin.com/pulse/building-reliable-rust-cicd-lessons-from-production-john-basrai--wclhc/)<br>
👉 [📝 "What the Cloudflare Outage Teaches Us About Production Rust"](https://www.linkedin.com/pulse/what-cloudflare-outage-teaches-us-production-rust-john-basrai--7yquc/)

---

## **Project Spotlight**:  
### 🔐 tokn: OAuth2/OIDC & JWT Authentication Infrastructure

OAuth2/OIDC authorization server in Rust with RFC 6749/7636 compliance, PKCE flow, refresh token rotation, and automated protocol testing.

🔧 **Highlights**:
- Complete OAuth2 authorization server (RFC 6749) with PostgreSQL persistence
- JWT token service (RFC 7519) with HS256 signing and lifecycle management
- **5 REST API endpoints** for complete token flows (generation, validation, refresh, revocation)
- **AuthMiddleware** for Bearer token validation on protected routes
- **10 automated integration tests** validating all authentication flows and security scenarios
- Token rotation and JTI-based revocation using Redis TTL blacklist
- Clean Architecture with EMBP pattern and trait-based abstractions
- Comprehensive rustdoc with RFC references

🧪 **Testing & Quality**:
```bash
./scripts/test-jwt-service.sh
```
✅ Token generation & validation (HS256 signing, expiration)  
✅ Refresh token rotation (prevents replay attacks)  
✅ Token revocation & blacklisting (Redis-backed)  
✅ Protected route authentication (JWT middleware)  
✅ Security edge cases (missing tokens, revoked tokens)

**Technical Stack**: Axum, PostgreSQL (SQLx), Redis, Argon2id, jsonwebtoken, Docker Compose

---

### 🧩 More Rust Projects

| Repo | Highlights |
| ---- | ---------- |
| **[axum-quickstart](https://github.com/JohnBasrai/axum-quickstart)** | Async REST API in Rust using Axum, Redis, and Tokio. Demonstrates WebAuthn/Passkeys authentication with PostgreSQL credential storage, Redis challenge management, session-based auth, Prometheus metrics, and comprehensive integration testing |
| **[cr8s](https://github.com/JohnBasrai/cr8s)** | Rocket + Postgres backend with JWT auth, role-based access, SQLx migrations, comprehensive integration test suite with database transactions and API endpoint validation. Part of a full-stack platform for crate metadata, release tracking, and user access |
| **[cr8s-fe](https://github.com/JohnBasrai/cr8s-fe)** | Yew/WASM frontend companion to the cr8s Rust backend, cross-platform Docker dev environment, Playwright E2E testing |
| **[zkp-cp](https://github.com/JohnBasrai/zkp-cp)** | Zero-knowledge proof implementation in Rust — gRPC client-server demo of Chaum–Pedersen ZK proofs using tonic |
| **[argus-events](https://github.com/JohnBasrai/argus-events)** | Event tracking service in Rust + Axum with query filtering, Prometheus metrics, Docker containerization, 21 integration tests, and CI/CD pipeline |
| **[mempool-vortex](https://github.com/JohnBasrai/mempool-vortex)** | MEV infrastructure simulation with real-time Ethereum mempool monitoring, WebSocket streaming, and latency measurement in Rust |
| **[sensorflow-data-pipeline](https://github.com/JohnBasrai/sensorflow-data-pipeline)** | Modular sensor data pipeline in Rust: fetch, transform, analyze, store, and expose via API with PostgreSQL indexing optimization and real-time anomaly detection |

📁 **[Complete Repository List](https://u.pcloud.link/publink/show?code=XZzpRs5ZkaemojJyP7jaLpK6phpph8GNltRk)** — All GitHub repositories with descriptions

---

## 🛠️ Skills Overview

**Core Expertise**  
- Rust & C++ Systems Programming  
- Backend & Distributed Systems  
- Authentication & Authorization (OAuth2/OIDC/JWT/WebAuthn)
- API Design (REST, gRPC, GraphQL)
- Cryptography & Zero-Knowledge Proofs

**Languages**  
- Rust (since 2022; async, networking, systems)
- C / Modern C++ (STL, Boost)
- Python, SQL
- WebAssembly (WASM)  

**Async & Networking**  
- Tokio, Async/Futures, reqwest
- WebSocket, TCP/IP, UDP, RTP
- Real-time streaming, packetized media transport
- Ethereum WebSocket Integration

**Architecture**
- Secure sandboxed execution (namespaces, cgroups v2)
- Ingress, scheduling, and backpressure in distributed systems

**Databases & Infrastructure**  
- PostgreSQL, Redis, SQLx, Diesel
- Docker / Docker Compose
- IronBank container hardening

**Testing Strategies**  
- Unit & Integration Testing (Rust cargo test)
- Security Testing (OAuth2/JWT token lifecycle, rotation, revocation)
- E2E Testing (Playwright browser automation)
- API Testing (RESTful endpoint validation)
- CI/CD Integration (Docker service orchestration)

**DevOps & CI/CD**  
- GitLab CI/CD, GitHub Actions (performance optimization, cross-platform workflows)
- Automated test execution with Docker orchestration

**Web Frameworks & Middleware**  
- Axum / Rocket / Actix / Yew
- Axum middleware (authentication, request validation)
- Trait-based middleware composition

**Monitoring & Observability**  
- Prometheus, Loki, Grafana  
- Latency, throughput, and runtime metrics

---

## 🧪 Testing Philosophy & Practice

Testing across multiple layers with emphasis on automation and isolation:
- **Security Testing**: 10 automated OAuth2/JWT tests (token lifecycle, rotation, revocation, middleware)
- **Backend Integration**: Database transaction testing, API endpoint validation, authentication flows
- **Frontend E2E**: User journey automation with Playwright
- **CI/CD Integration**: Automated test execution with Docker service orchestration
- **Test Isolation**: Proper database setup/teardown and transaction rollback patterns

---

## 📋 Architecture & Patterns

**[Explicit Module Boundary Pattern (EMBP)](https://github.com/JohnBasrai/architecture-patterns/blob/main/rust/embp.md)** 

A Rust architectural pattern I've documented that uses gateway files (`mod.rs`, `lib.rs`, `main.rs`) to create explicit module boundaries and controlled dependencies. EMBP enables complete internal refactoring freedom while maintaining clean public APIs and clear architectural layers.

---

## 🤝 Let's Connect

If you're hiring for backend, distributed systems, authentication infrastructure, or Rust-focused roles, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/johnbasrai/).

### Socials

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnbasrai/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/JohnBasrai)
