# <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> John Basrai

**Senior/Staff Software Engineer**<br>
*Rust & C++ · Backend Systems · Distributed Architectures · CI/CD · High-Performance Applications*

## <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> About Me

Solution-oriented, results-driven software engineer with **15+ years of experience** in systems and backend development — currently specializing in **Rust** for authentication infrastructure, backend systems, and correctness-first applications. Recent focus on **OAuth2/OIDC/JWT** implementations with comprehensive automated testing. Skilled in Rust, Modern C++, and Python, with a strong focus on architectural clarity, modularity, and security-first design.

I'm currently developing [tokn](https://github.com/JohnBasrai/tokn), a production-ready OAuth2/OIDC authorization server and JWT token service in Rust, featuring comprehensive automated testing, RFC compliance, and security-first design patterns.

## 📌 Featured
👉 [📝 "Building Reliable Rust CI/CD: Lessons from Production Failures"](https://www.linkedin.com/pulse/building-reliable-rust-cicd-lessons-from-production-john-basrai--wclhc/)<br>
👉 [📝 "What the Cloudflare Outage Teaches Us About Production Rust"](https://www.linkedin.com/pulse/what-cloudflare-outage-teaches-us-production-rust-john-basrai--7yquc/)

Other recent projects include:

* [**axum-quickstart**](https://github.com/JohnBasrai/axum-quickstart) — RESTful Axum backend with async Redis, WebAuthn/Passkeys support, and CI-ready dev tooling
* [**argus-events**](https://github.com/JohnBasrai/argus-events) — Production event tracking service with Prometheus metrics, distributed tracing, and clean architecture patterns

---

* 🌍 Based in Yuba City, CA
* 🤝 Open to collaborating on backend systems, authentication infrastructure, or distributed systems in Rust

## **Project Spotlight**:  
### 🔐 tokn: OAuth2/OIDC & JWT Authentication Infrastructure

A production-ready authentication infrastructure demonstrating complete OAuth2/OIDC authorization server and JWT token service implementation in Rust. This project showcases security-first design, RFC compliance, and comprehensive automated testing.

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

### 🧩 More Rust Projects

Here are additional selected projects showcasing Rust across domains including authentication, AWS, databases, zero-knowledge proofs, and frontend/backend integration:

---

| Repo | Highlights |
| ---- | ---------- |
| **[tokn](https://github.com/JohnBasrai/tokn)** | OAuth2/OIDC authorization server (RFC 6749) and JWT token service (RFC 7519) with 5 REST endpoints, token lifecycle management, refresh rotation, AuthMiddleware, and 10 automated security tests |
| **[axum-quickstart](https://github.com/JohnBasrai/axum-quickstart)** | Production-ready Axum + Redis API featuring PostgreSQL-backed WebAuthn credential storage, Redis challenge management, Prometheus metrics, health monitoring, clean architecture patterns (EMBP), and comprehensive testing infrastructure |
| **cr8s** | Rocket + Postgres backend with JWT auth, role-based access, SQLx migrations, comprehensive integration test suite with database transactions and API endpoint validation. Part of a full-stack platform for crate metadata, release tracking, and user access |
| **[cr8s-fe](https://github.com/JohnBasrai/cr8s-fe)** | Yew/WASM frontend companion to the cr8s Rust backend, cross-platform Docker dev environment, Playwright E2E testing |
| **[zkp-cp](https://github.com/JohnBasrai/zkp-cp)** | Zero-knowledge proof implementation in Rust — gRPC client-server demo of Chaum–Pedersen ZK proofs using tonic |
| **[argus-events](https://github.com/JohnBasrai/argus-events)** | Production event tracking service with Prometheus metrics, distributed tracing, clean architecture (trait-based repository, EMBP), and container-per-test isolation strategy |
| **[mempool-vortex](https://github.com/JohnBasrai/mempool-vortex)** | MEV infrastructure simulation with real-time Ethereum mempool monitoring, WebSocket streaming, and latency measurement in Rust |
| **[sensorflow-data-pipeline](https://github.com/JohnBasrai/sensorflow-data-pipeline)** | Modular sensor data pipeline in Rust: fetch, transform, analyze, store, and expose via API with PostgreSQL indexing optimization and real-time anomaly detection |

📁 **[Complete Project Portfolio](https://u.pcloud.link/publink/show?code=XZzpRs5ZkaemojJyP7jaLpK6phpph8GNltRk)** — Full list of GitHub repositories with descriptions

### What I'm Looking For
Open to roles in **authentication infrastructure (OAuth2/OIDC/JWT)**, Rust-based backend/fullstack systems, distributed architectures, cryptographic protocols (ZKPs), or embedded platforms. **Strong emphasis on test-driven development and quality engineering practices.**

### Current Focus
Currently developing modern authentication infrastructure with **tokn** (OAuth2/OIDC/JWT) and integrating **WebAuthn/Passkeys** into axum-quickstart. Focus on production-ready security patterns, comprehensive automated testing (10 security test scenarios), and RFC-compliant implementations. Building on lessons learned from cr8s ecosystem to deliver cleaner CI/CD workflows and containerization strategies.

<p align="left">
<a href="https://docs.microsoft.com/en-us/cpp/?view=msvc-170" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/cplusplus-colored.svg" width="36" height="36" alt="C++" /></a>
<a href="https://www.rust-lang.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" width="36" height="36" alt="Rust" /></a>
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/git-colored.svg" width="36" height="36" alt="Git" /></a>
<a href="https://www.oracle.com/java/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/java-colored.svg" width="36" height="36" alt="Java" /></a>
<a href="https://www.python.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg" width="36" height="36" alt="Python" /></a>
</p>

### 🛠️ Skills Overview

**Areas of Expertise**  
- C++ and Rust-based Systems Programming  
- Distributed Systems  
- API Design  
- Real-Time Processing  
- Authentication & Authorization (OAuth2/OIDC/JWT)
- Cryptography  
- WebAssembly Frontend Development
- Real-Time Ethereum Mempool Processing
- Flashbots-style MEV Opportunity Detection & Simulation
- Modular Rust Pipeline Design (Searcher, Bundler, Mempool, Config)

**Languages & Libraries**  
- Rust (since 2022)  
- C / Modern C++ (STL, Boost)
- Python  
- Java  
- SQL  
- WebAssembly (WASM)  

**Async & Networking**  
- Tokio / Async / Futures  
- reqwest  
- WebSocket  
- TCP/IP / UDP  
- RTP (Real-time Transport Protocol)  
- Web-Sys
- Ethereum WebSocket Integration (mempool ingestion)
- Multi-Relay Submission (Flashbots, bloXroute, Eden — simulated)

**Cloud & Infrastructure**  
* **AWS Lambda** — [aws-lambda-action-filter](https://github.com/JohnBasrai/aws-lambda-action-filter): Rust Lambda function for filtering entity actions by time and priority, with tests and corrected logic
- AWS (Dev/Deploy)
- IronBank container hardening

**Databases & Caching**  
- PostgreSQL / Redis / SQLx / Diesel

**Testing Frameworks & Strategies**  
- **Rust Testing** - Unit and integration testing with cargo test framework
- **Integration Testing** - Database transactions, API validation, and service integration
- **Security Testing** - OAuth2/JWT token lifecycle, rotation, revocation, and middleware validation
- **API Testing** - RESTful endpoint validation and authentication flow testing
- **E2E Testing** - Playwright E2E browser automation and UI testing
- **MEV Simulation** Testing (non-submitting bundle pipeline with --simulate)

**DevOps & CI/CD**  
- Docker / Docker Compose (advanced container orchestration)
- GitLab CI/CD, GitHub Actions (performance optimization, cross-platform workflows)
- **Test Automation** - Automated test execution with Docker service orchestration
- Jenkins

**Web Framework Middleware**  
- Axum middleware (authentication, request validation)
- Trait-based middleware composition

**RPC & Message Brokers**  
- Apache Thrift
- gRPC/protobuf
- ZeroC Ice, IceRPC
- CORBA
- ActiveMQ

**Frameworks & APIs**  
- Axum / Rocket / Actix / Yew
- RESTful APIs  
- gRPC (Tonic)
- GraphQL
- Apache Thrift  
- Serde

**Embedded & OS Platforms**  
- Linux  
- MCOS  
- VxWorks  
- QNX  
- Mercury RTOS  
- DMA/RACEway Fabrics  

**Monitoring & Observability**  
- Prometheus  
- Loki  
- Grafana  

**Tools**  
- Git  
- Cargo  
- Docker  
- Docker Compose  

**🧠 Work Habits & Culture Fit**

- Test-Driven Quality / Automated Test Suites
- Remote-First / Asynchronous Communication
- Pair Programming & Code Review Culture

### 🔧 Recent Highlights

- **Authentication Infrastructure**: Built production-ready OAuth2/OIDC authorization server and JWT token service with **10 automated security tests** validating token lifecycle, refresh rotation, revocation, and protected route authentication
- **RFC Compliance**: Implemented OAuth2 (RFC 6749) and JWT (RFC 7519) specifications with HS256 signing, 15-minute access tokens, 7-day refresh tokens, and JTI-based revocation using Redis TTL blacklist
- **Security Testing Excellence**: Comprehensive test suite covering token generation, validation, rotation (prevents replay attacks), revocation, blacklisting, and middleware authorization with automated CI/CD integration
- **WebAuthn/Passkeys Integration**: Built WebAuthn credential storage (PostgreSQL), challenge management (Redis), and authentication flows in axum-quickstart with automated testing
- **Integration Testing Excellence**: Implemented comprehensive integration test suite for cr8s backend with database transaction testing, endpoint validation, and automated CI/CD integration
- **Performance Engineering**: Optimized CI/CD pipeline for cr8s-fe, achieving 25% performance improvement (5m → 4m build times)
- Refined **Docker-based local development** for rapid iteration and frontend/backend parity
- **Cross-Platform Compatibility**: Solved complex Docker user permission issues across development environments (local dev vs GitHub runners)  
- **DevOps Excellence**: Eliminated environment configuration drift by consolidating version management and improving container orchestration

### 🧪 Testing Philosophy & Practice

**Full-Stack Test Coverage**: Achieved comprehensive testing coverage across multiple projects:
- **Security Testing**: 10 automated OAuth2/JWT tests (token lifecycle, rotation, revocation, middleware)
- **Backend Integration Tests**: Database transaction testing, API endpoint validation, authentication flows
- **Frontend E2E Tests**: User journey automation with Playwright
- **CI/CD Integration**: Automated test execution with Docker service orchestration
- **Test Isolation**: Proper test database setup/teardown and transaction rollback patterns

### Socials

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnbasrai/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/JohnBasrai)
---

## 📋 Architecture & Patterns

**[Explicit Module Boundary Pattern (EMBP)](https://github.com/JohnBasrai/architecture-patterns/blob/main/rust/embp.md)** 

- A Rust architectural pattern I've documented that uses gateway files (`mod.rs`, `lib.rs`, `main.rs`) to create explicit module boundaries and controlled dependencies. EMBP enables complete internal refactoring freedom while maintaining clean public APIs and clear architectural layers.

---
## 🛠️ Featured Tools

**tokn Authentication Infrastructure**

[![tokn CI](https://github.com/JohnBasrai/tokn/actions/workflows/rust.yml/badge.svg)](https://github.com/JohnBasrai/tokn)

**Rust Dev Container CI**

[![rust-base-containers CI](https://github.com/JohnBasrai/rust-base-containers/actions/workflows/ci.yml/badge.svg)](https://github.com/JohnBasrai/rust-base-containers)

---

## 🏅 Badges

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![CI](https://img.shields.io/badge/GitHub%20Actions-CI-blue?logo=github-actions&logoColor=white&style=for-the-badge)

### 🧪 Testing & Quality Assurance
![Integration Testing](https://img.shields.io/badge/Integration%20Testing-Rust-orange?style=for-the-badge&logo=rust&logoColor=white)
![E2E Testing](https://img.shields.io/badge/E2E%20Testing-Playwright-45ba4b?style=for-the-badge&logo=playwright&logoColor=white)
![Security Testing](https://img.shields.io/badge/Security%20Testing-OAuth2%2FJWT-red?style=for-the-badge&logo=rust&logoColor=white)
![Test Automation](https://img.shields.io/badge/Test%20Automation-CI%2FCD-blue?style=for-the-badge&logo=github-actions&logoColor=white)

## 🤝 Let's Connect

If you're hiring for backend, distributed systems, authentication infrastructure, or Rust-focused roles, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/johnbasrai/).
