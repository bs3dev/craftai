# 📚 CraftAI File Disciplines (Expanded)

This document defines all major file types used in CraftAI projects.  
Each file represents a key discipline — engineering, design, product, data, or operations — and is referenced by specific agents as part of their context.

---

## 📐 Architecture & Engineering

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `stack.md`                | Technologies, platforms, environments                     | Forge, Shield, Scroll  |
| `code-style.md`           | Naming, formatting, and coding conventions                | Forge, Shield          |
| `adrs/*.md`               | Architecture Decision Records                             | Scroll, Forge, Pulse   |
| `tech-debt.md`            | Known limitations and tech debt backlog                   | Forge, Pulse, Shield   |

---

## 🎨 Design & Experience

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `branding-guidelines.md`  | Visual identity: logo, color, spacing, usage              | Nova, Quill            |
| `tone-of-voice.md`        | Linguistic tone, personality, writing style               | Quill, Echo, Scroll    |
| `ui-patterns.md`          | Approved interface components and design tokens           | Nova, Echo             |
| `accessibility.md`        | Guidelines for inclusive and accessible experiences        | Echo, Shield           |

---

## 📦 Product & Strategy

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `product-vision.md`       | Mission, audience, goals, value proposition               | Pulse, Scope, Forge    |
| `feature-priorities.md`   | Roadmap items, prioritization rationale                   | Pulse, Scope           |
| `personas.md`             | User archetypes and segments                              | Echo, Pulse            |
| `market-positioning.md`   | Competitive value, messaging pillars                      | Pulse, Scope, Quill    |

---

## 📊 Data & Metrics

| File Name                  | Description                                               | Used By Agents         |
|---------------------------|-----------------------------------------------------------|------------------------|
| `metrics-guide.md`        | KPIs, OKRs, conversion goals                              | Pulse, Scope, Echo     |
| `analytics-specs.md`      | Events tracked, schema, tool usage (e.g. GA, Mixpanel)    | Echo, Shield           |
| `retention-cohorts.md`    | Behavior analysis of user segments                        | Pulse, Scope           |

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

- Use clear formatting: headlines, bullet points, and structured sections
- Each file should be created using the [template.md](../templates/template.md)
- Reference these files in your `project.yaml` under `context.files`
- Agents will load only the relevant documents from this list

