# <img src="https://www.rust-lang.org/logos/rust-logo-32x32.png" alt="Rust" width="24" valign="middle" /> John Basrai

**Senior Rust Software Engineer**  
*Backend · Distributed Systems · WASM · CI/CD · E2E Testing*

## <img src="https://www.rust-lang.org/logos/rust-logo-32x32.png" alt="Rust" width="24" valign="middle" /> About Me

Solution-oriented and results-driven software engineer with 15+ years of experience in systems and backend development, currently specializing in **Rust**. Proven expertise in designing high-performance, scalable, and reliable software using **Rust**, **Modern C++**, and **Python**. Adept at applying engineering principles, object-oriented design, and advanced problem-solving techniques to deliver robust enterprise solutions.

I’m currently building a full-stack Rust app across two coordinated repos: cr8s (backend with Rocket + Postgres) and cr8s-fe (Yew/WebAssembly SPA). The frontend manages its own Docker-first orchestration and integrates with CI-verified Playwright E2E tests. I emphasize async execution, observability, and system resilience—especially in distributed or embedded domains. I’m also open to systems programming in Rust, including Linux CLI tools, where performance and safety are critical. Known for debugging complex issues and delivering production-grade solutions across the stack.

- 🌍 I'm based in Yuba City, CA
- 🧠 Currently building a Rocket + Postgres REST backend with a Yew/WebAssembly SPA front-end … See the **[cr8s](https://github.com/JohnBasrai/cr8s)** + **[cr8s-fe](https://github.com/JohnBasrai/cr8s-fe)** stack
- 🧠 Also worked on a RESTful backend using **Rust**, Axum, and Redis in my [axum-quickstart](https://github.com/JohnBasrai/axum-quickstart) project  
- 🤝 I'm open to collaborating on projects — especially in Rust, backend systems, or CLI tool development

<br> **Project Spotlight**:  
| Repo                                                                 | Highlights                                                       |
| -------------------------------------------------------------------- | ---------------------------------------------------------------- |
| **[cr8s](https://github.com/JohnBasrai/cr8s)**                       | Rocket + Postgres backend  •  Docker-first dev env & CI          |
| **[cr8s-fe](https://github.com/JohnBasrai/cr8s-fe)**                 | Yew/WebAssembly SPA  •  Live-reload, Playwright e2e tests        |
| **[axum-quickstart](https://github.com/JohnBasrai/axum-quickstart)** | Alternative Axum/Tokio REST template with full integration tests |
| **[zkp-cp](https://github.com/JohnBasrai/zkp-cp)**   | gRPC client-server demo of Chaum–Pedersen ZK proofs using **tonic**  |

### What I'm Looking For
Open to roles in Rust-based backend/fullstack systems, distributed architectures, cryptographic protocols (ZKPs), or embedded platforms.

### Current Focus
Currently hardening a Rocket + Yew micro-SaaS, integrating gRPC with Tonic, and expanding Playwright-based E2E coverage.

💼 Open to full-time Rust backend roles or select consulting engagements.<br>
The best way to contact me is via [LinkedIn](https://www.linkedin.com/in/johnbasrai).

Currently focused on Rust-based backend and distributed system development.

<p align="left">
<a href="https://docs.microsoft.com/en-us/cpp/?view=msvc-170" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/cplusplus-colored.svg" width="36" height="36" alt="C++" /></a>
<a href="https://www.rust-lang.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/rust-colored.svg" width="36" height="36" alt="Rust" /></a>
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/git-colored.svg" width="36" height="36" alt="Git" /></a>
<a href="https://www.oracle.com/java/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/java-colored.svg" width="36" height="36" alt="Java" /></a>
<a href="https://www.python.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/python-colored.svg" width="36" height="36" alt="Python" /></a>
</p>

### 🛠️ Skills Overview

**Areas of Expertise**  
- Rust-based Systems Programming  
- Distributed Systems  
- API Design  
- Real-Time Processing  
- Cryptography  
- WebAssembly Frontend Development  

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

**Cloud & Infrastructure**  
- AWS (Dev/Deploy)
- IronBank container hardening

**Databases & Caching**  
- PostgreSQL / Redis / SQLx / Diesel

**End-to-End Testing**  
 - Playwright - E2E browser automation and UI testing 

**DevOps & CI/CD**  
- Docker / Docker Compose
- GitLab CI/CD, GitHub Actions
- Jenkins  

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

- Agile / Scrum / Kanban
- Test-Driven Development (TDD)
- Pair Programming & Remote Collaboration
- Asynchronous Communication (remote-first / remote-only)

### 🔧 Recent Highlights

- Added **Playwright-powered manual E2E test suite** for a fullstack Rust/WASM application
- Enhanced **GitHub Actions workflows** with `workflow_dispatch`, conditional steps, and Docker service orchestration
- Refined **Docker-based local development** for rapid iteration and frontend/backend parity


### Socials

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/johnbasrai/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/JohnBasrai)
---

## 📋 Architecture & Patterns

**[Explicit Module Boundary Pattern (EMBP)](https://github.com/JohnBasrai/architecture-patterns/blob/main/rust/embp.md)** 

- A Rust architectural pattern I've documented that uses gateway files (`mod.rs`, `lib.rs`, `main.rs`) to create explicit module boundaries and controlled dependencies. EMBP enables complete internal refactoring freedom while maintaining clean public APIs and clear architectural layers.

---
## 🛠️ Featured Tools

**Rust Dev Container CI**

[![rust-base-containers CI](https://github.com/JohnBasrai/rust-base-containers/actions/workflows/ci.yml/badge.svg)](https://github.com/JohnBasrai/rust-base-containers)

---

## 🏅 Badges

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![CI](https://img.shields.io/badge/GitHub%20Actions-CI-blue?logo=github-actions&logoColor=white&style=for-the-badge)

## 🤝 Let's Connect

If you're hiring for backend, distributed systems, or Rust-focused roles, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/johnbasrai/).
