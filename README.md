# Trading Simulation Platform

This project is a backend-only **Trading Simulation Platform** designed to demonstrate
backend architecture, microservices design and reactive programming using **Kotlin**.

The platform simulates the core components of a brokerage system:
accounts, orders and portfolios, focusing on **consistency, clean architecture
and scalability** rather than real market connectivity.

---

## 🎯 Goals

- Practice backend development using **Kotlin**
- Apply **microservices architecture**
- Use **reactive programming** with Spring WebFlux and coroutines
- Design a clean and explicit **domain model**
- Showcase architectural decisions suitable for **financial environments**

---

## 🧱 Architecture Overview

The platform is composed of independent microservices:

- **account-service**: user accounts and balances
- **order-service**: order lifecycle management
- **portfolio-service**: positions and portfolio calculation

Each service follows **Clean Architecture** principles:
- Domain
- Application
- Infrastructure
- API (controllers)

Services communicate via **REST APIs**.
Authentication is handled using **JWT**.

---

## 🛠️ Tech Stack

- Kotlin
- Spring Boot (WebFlux)
- Kotlin Coroutines
- PostgreSQL
- R2DBC
- Gradle
- Docker & Docker Compose
- JWT authentication

---

## 📦 Services

### Account Service
Responsible for:
- Account creation and management
- Balance management
- Account validation

### Order Service
Responsible for:
- Placing buy/sell orders
- Order validation
- Order state transitions

### Portfolio Service
Responsible for:
- Tracking positions
- Calculating holdings and P&L
- Aggregating trading activity

---

## 🔐 Security

- JWT-based authentication
- Stateless services
- Role-based access (future improvement)

---

## 🚀 Running the project

```bash
docker-compose up --build
```
---

Each service exposes its own REST API.

## 🔮 Future Improvements

- Event-driven communication between services

- Market data integration

- Risk management rules

- Idempotency handling

- Observability (metrics & tracing)

## 🧠 Design Philosophy

This project prioritizes:

- Explicit domain modeling

- Clear separation of concerns

- Readable and maintainable code

- Predictable behavior over feature completeness
