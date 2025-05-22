# 🧱 Architectural Decision Records (ADR)

> This document defines the purpose, format, and practices for maintaining ADRs (Architectural Decision Records) in this project.  
> ADRs ensure that key technical decisions are documented, understood, and traceable over time — by both humans and AI agents.

---

## 📘 What is an ADR?

An **Architectural Decision Record** captures a **single, significant technical decision** made in the life of the project, along with:

- The **context** that led to it
- The **decision** that was made
- The **alternatives** that were considered
- The **consequences** of that decision

ADRs answer the question:  
**"Why is the system the way it is?"**

---

## 🧱 Why Use ADRs?

- 🧠 Preserve architectural reasoning over time
- 🤖 Enable CraftAI agents to align with past decisions
- 🗂️ Provide traceability and justification for trade-offs
- 🧭 Guide onboarding, refactoring, and planning
- 📚 Support audits, compliance, and stakeholder clarity

---

## 📂 File Structure and Storage

All ADRs are stored in the following folder: ./tech/adr/
Each ADR should follow this naming pattern: ADR-<ID>-<short-title>.md


Examples:

- `ADR-001-event-driven-architecture.md`
- `ADR-002-auth-provider-switch.md`

---

## 🧩 Required Sections in Each ADR

| Section                      | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| 📌 **Status**                | `proposed`, `accepted`, `rejected`, `superseded`, or `deprecated`           |
| 🎯 **Context**               | Why this decision is needed                                                |
| 🧠 **Decision**              | What was decided and why                                                   |
| ⚖️ **Alternatives Considered** | Other paths explored and reasons for not choosing them                      |
| ✅ **Consequences**          | Trade-offs, side effects, future implications                              |
| 📚 **References** *(optional)* | Links to issues, specs, RFCs, or benchmarks                                |
| 🆔 **Metadata**              | ID, Date, Author, and optionally related ADRs or superseded decisions       |

---

## 📌 Valid Status Values

- `proposed`: not yet reviewed or approved
- `accepted`: the decision is active and in effect
- `rejected`: deliberately not chosen
- `superseded`: replaced by a newer ADR
- `deprecated`: no longer in use or discouraged

---

## 🧠 Example ADR Snippet

```markdown
# ADR-001: Use Event-Driven Architecture for Internal Services

📌 Status: accepted  
🆔 ID: 001  
📅 Date: 2025-05-18  
✍️ Author: Bruno Brandes  

---

🎯 Context  
Our platform needs real-time communication between microservices such as checkout, ledger, and notifications...

🧠 Decision  
We will adopt an event-driven architecture using Kafka to decouple internal service communication...

⚖️ Alternatives Considered  
- RESTful synchronous APIs  
- gRPC streams  
- AWS SQS for async queuing

✅ Consequences  
- Pro: Loose coupling, horizontal scalability  
- Con: Higher ops complexity, eventual consistency

📚 References  
- https://martinfowler.com/articles/201701-event-driven.html

🔁 Best Practices

* One ADR per decision. Keep it focused.
* Write ADRs even when rejecting an option (that’s equally valuable context).
* Use consistent formatting and filenames.
* Link ADRs from PRs, commits, and documentation.
* Supersede instead of editing existing ADRs — preserve history.

## ✅ Compliance Checklist

- [ ] Filename follows `ADR-<ID>-<short-title>.md` convention?
- [ ] All required sections are present and complete?
- [ ] Status is one of the predefined values (`accepted`, `proposed`, etc)?
- [ ] Context and decision are clearly written and specific?
- [ ] Alternatives are listed with rationale for rejection?
- [ ] Consequences include both benefits and drawbacks?
- [ ] References or links are included when relevant?
- [ ] Superseded ADRs are cross-referenced if applicable?




