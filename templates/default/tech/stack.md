# 🧱 Technical Stack Overview

> This document defines the technologies, frameworks, and infrastructure components used to build, deploy, test, and maintain this product.
> It guides engineers and agents in understanding and evolving the system over time.

---

## ⚙️ Frontend Framework

Describe the main technologies used in the client-side application.

- Framework: Flutter 3.x
- Architecture: Clean Architecture with Riverpod
- Component Library: Custom, Figma-linked tokens
- Target Platforms: Android, iOS, Web (progressive fallback)

> Nova and Forge use this section to generate UI, connect data flows, and adhere to standards.

---

## 🔧 Backend Framework

Outline the server-side stack and architectural patterns.

- Language: TypeScript
- Runtime: Node.js 20+
- Framework: Fastify
- API Style: REST + Webhooks + Event-driven endpoints
- Auth: JWT + OAuth2 via Auth0

> Forge and Shield use this to scaffold endpoints and enforce contract discipline.

---

## 🧮 Database

Specify database engines, query methods, and key constraints.

- Primary DB: PostgreSQL 15
- Access: Prisma ORM
- Migrations: Declarative with versioned scripts
- Indexing: Logical + full-text search on select tables

> Shield can validate data structure, performance, and migration consistency.

---

## 🛂 Authentication

Describe the identity and session management strategy.

- Provider: Auth0
- Token Strategy: Access/Refresh + JWT Scopes
- Permissions: Role-based (RBAC)
- Session Expiry: Sliding (30 min active)

---

## ☁️ Hosting & Deployment

Define where and how the application is hosted.

- Infra Provider: AWS
- Frontend: CloudFront + S3 static
- Backend: Lambda + API Gateway
- IaC: Pulumi + GitHub Actions
- DNS: Route 53

---

## 🔁 CI/CD Pipeline

- Version Control: GitHub
- Build: GitHub Actions
- Test: Vitest (unit), Playwright (E2E)
- Deploy: Preview via branches + Production via tags
- Secrets: GitHub Encrypted + AWS SSM fallback

> Agents should follow this flow or suggest improvements via pull requests.

---

## 🔍 Monitoring & Logging

- Logs: CloudWatch + Sentry
- Metrics: Datadog + AWS X-Ray
- Alerts: Slack + PagerDuty
- Dashboards: Datadog and Grafana (AWS-managed)

> Shield uses this data to triage and report root causes.

---

## 🧪 Testing Strategy

Describe how quality is enforced across the stack.

- Unit Tests: All logic modules must have > 90% coverage
- Integration Tests: For all external API interactions
- End-to-End: Run daily across critical flows (login, payment, error recovery)
- Linting: ESLint + Stylelint
- Static Analysis: SonarQube

---

## 📚 Reference Links

- [AWS Modern App Strategy](https://docs.aws.amazon.com/decision-guides/latest/modern-apps-strategy-on-aws-how-to-choose/modern-apps-strategy-on-aws-how-to-choose.html)
- [Amplify Fullstack Guide](https://aws.amazon.com/blogs/mobile/the-ctos-guide-to-building-fullstack-applications-with-aws-amplify/)
- [Azure Databricks CI/CD](https://learn.microsoft.com/azure/databricks/dev-tools/ci-cd/best-practices)
- [GCP Modern Tech Stack](https://cloud.google.com/resources/modernizing-data-tech-stack-ebook)
- [IBM Fullstack Dev](https://developer.ibm.com/learningpaths/get-started-mobile-dev-android/full-stack-mobile-dev)

---

> *This document helps CraftAI agents build faster, smarter, and in alignment with architectural excellence.*
