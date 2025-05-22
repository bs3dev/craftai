# ADR-001: Use Event-Driven Architecture for Core Services

---

## 🆔 ADR Metadata

- **ID**: ADR-001  
- **Date**: 2025-05-22  
- **Author**: Leia Organa  
- **Status**: accepted

---

## 🎯 Context

As the Rebel Recruitment Portal must scale across multiple mission control centers and interact with external services like identity validation, pilot training, and fleet dispatch — we need an architecture that supports **loose coupling**, **real-time communication**, and **resilience to failure**.

A traditional monolithic or tightly coupled service layer would slow us down, reduce fault tolerance, and make onboarding new rebel base nodes harder.

---

## 🧠 Decision

We will adopt an **Event-Driven Architecture (EDA)** using **message queues** (Kafka, NATS, or RabbitMQ) for core services communication.

Each service will emit and listen to domain-specific events. Key decisions include:

- Events will follow a canonical structure with versioning.
- Critical flows like registration, validation, and assignment will be event-based.
- We’ll use an event store pattern to allow replaying or audit if needed.

---

## ⚖️ Alternatives Considered

### 1. REST-Only Microservices

- Simpler for initial implementation
- But requires tight coordination between services and leads to high coupling

### 2. Monolith with Internal Pub/Sub

- Centralized control and easier debugging
- But lacks scalability and resilience

---

## ✅ Consequences

### Positive

- High decoupling and extensibility
- Easier to onboard new services (e.g., Rebel Pilot Matcher)
- Enables asynchronous retries, audits, and testing

### Negative

- Increases architectural complexity
- Requires learning curve for message semantics and consistency handling
- Tooling and observability will need to be upgraded

---

## 📚 References

- [Martin Fowler – Event-Driven Architecture](https://martinfowler.com/articles/201701-event-driven.html)
- [Kafka Patterns for Microservices](https://www.confluent.io/blog/microservices-communication/)
- Internal document: `/tech/event-standards.md`

---

> *This ADR guides our future discussions around service communication patterns and supports long-term agility as our rebellion grows.*
