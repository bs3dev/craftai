# 📚 CraftAI File Disciplines (Expanded)

This document defines all major file types used in CraftAI projects.  
Each file represents a key discipline — engineering, design, product, data, or operations — and is referenced by specific agents as part of their context.

---

## 📐 Architecture & Engineering

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `stack.md`                | Technologies, platforms, environments                     | Forge, Shield, Scroll  |
| `code-style/*`            | Coding conventions by language                            | Forge, Shield          |
| `adr/*.md`                | Architecture Decision Records                             | Scroll, Forge, Pulse   |
| `tech-debt.md`            | Known limitations and tech debt backlog                   | Forge, Pulse, Shield   |

---

## 🎨 Design & Experience

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `branding-guidelines.md`  | Visual identity: logo, color, spacing, usage              | Nova, Quill, Pulse     |
| `tone-of-voice.md`        | Linguistic tone, personality, writing style               | Quill, Echo, Scroll    |
| `design-system.md`        | Visual principles and reference links to external DS      | Nova, Echo             |
| `user-experience.md`      | Experience goals and emotional intent                     | Echo, Shield           |

---

## 📦 Product & Strategy

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `product-vision.md`       | Mission, audience, goals, value proposition               | Pulse, Scope, Forge    |
| `user-personas.yaml`      | Core user types and motivations                           | Echo, Pulse, Quill     |
| `go-to-market.md`         | Strategic launch and positioning plan                     | Pulse, Scope           |
| `market-positioning.md`   | Competitive narrative and messaging strategy              | Pulse, Scope, Quill    |

---

## 📊 Data & Metrics

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `analytics-metrics.md`    | KPIs, OKRs, user behavior, funnel events                  | Pulse, Scope, Echo     |
| `data-modeling.md`        | Entity structure, relationships, core datasets            | Forge, Shield, Scroll  |
| `retention-cohorts.md`    | Segment behavior analysis and lifecycle mapping           | Pulse, Scope           |

---

## 🧠 Knowledge & Documentation

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `adr/*.md`                | Technical or product decisions (duplicated intentionally) | Scroll, Forge, Pulse   |
| `onboarding-guide.md`     | Dev onboarding, processes, how-tos                        | Scroll, Pulse          |
| `internal-wiki.md`        | Miscellaneous team knowledge and tribal history           | Scroll                 |

---

## 🔌 Integrations & Operations

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `integration-apis.md`     | External APIs and service touchpoints                     | Forge, Link            |
| `deployment-flow.md`      | CI/CD pipeline, infra and environment overview            | Flux, Shield           |
| `observability.md`        | Logs, metrics, alerting setup                             | Ghost, Shield          |
| `security-policies.md`    | Authentication, authorization, data protection guidelines | Shield, Forge          |

---

## 🧭 How to Use

- Format all files using headlines, bullet points, and structured sections
- Use templates from `templates/default/{discipline}/`
- Reference the relevant files in `project.yaml` under `context.files`
- Agents will only consume the files listed in that context

---

> This file serves as a shared contract between creators and agents.  
> A well-mapped project structure = a well-orchestrated AI team.
