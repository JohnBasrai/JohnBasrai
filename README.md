# <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" alt="Rust" width="24" valign="middle" /> John Basrai

**Senior Software Engineer**
*Rust & C++ · Systems & Distributed Architectures · High-Performance Applications*

## About Me

Senior systems engineer with **15+ years of experience** building backend and distributed systems, currently focused on **Rust** for authentication infrastructure and secure, high-assurance services. I care deeply about architectural clarity, explicit boundaries, and automated testing.

* 🌍 Yuba City, CA
* 🤝 Open to Rust-focused backend and distributed systems work

### Current Focus

- **[tokn](https://github.com/JohnBasrai/tokn)** — OAuth2/OIDC/JWT authorization server in Rust, implementing RFC 6749/7636 with automated protocol testing (PKCE, token rotation, scope enforcement).
- **[rtp-opus-streamer](https://github.com/JohnBasrai/rtp-opus-streamer)** — real-time audio streaming system in Rust using RTP (RFC 3550) and Opus (RFC 6716), exploring resilience, observability, and behavior under network constraints.

## 📌 Writing & Talks

- [Building Reliable Rust CI/CD: Lessons from Production Failures](https://www.linkedin.com/pulse/building-reliable-rust-cicd-lessons-from-production-john-basrai--wclhc/)
- [What the Cloudflare Outage Teaches Us About Production Rust](https://www.linkedin.com/pulse/what-cloudflare-outage-teaches-us-production-rust-john-basrai--7yquc/)

---

## 🔐 Project Spotlight — tokn

OAuth2/OIDC authorization server in Rust with PKCE, refresh token rotation, and automated security testing.

**Highlights**
- RFC-compliant OAuth2 server with PostgreSQL persistence
- JWT lifecycle management (RFC 7519)
- Redis-backed token revocation and replay protection
- 10 automated integration tests covering security edge cases
- Clean architecture using EMBP and trait-based abstractions

**Stack**: Axum, PostgreSQL (SQLx), Redis, Argon2id, Docker Compose

---

## 🧩 Selected Projects

| Repo | Focus |
| ---- | ----- |
| **axum-quickstart** | Async REST APIs in Rust with WebAuthn/Passkeys, PostgreSQL, Redis, Prometheus |
| **cr8s** | Rocket backend with JWT auth, role-based access, SQLx migrations, full integration testing |
| **zkp-cp** | Chaum–Pedersen zero-knowledge proofs in Rust (gRPC, tonic) |
| **mempool-vortex** | Ethereum mempool monitoring and latency analysis in Rust |

---

## 🛠️ Technical Focus

**Systems & Architecture**
- Secure sandboxed execution (Linux namespaces, cgroups v2)
- User-facing ingress, scheduling, and backpressure
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

## 🤝 Let’s Connect

If you’re hiring for backend, distributed systems, or Rust-focused roles, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/johnbasrai/) or here on GitHub.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnbasrai/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/JohnBasrai)
