# 🧠 CraftAI Core Agents

> This directory contains all the **CraftAI agents** available in the `default` template.  
> Each agent represents a highly specialized AI teammate — designed to operate autonomously, guided by natural instructions and project context.

---

## 📦 File Structure

Each agent is defined by:

- `agent-name.yaml`: machine-readable definition (prompt, file context, rules)
- `agent-name.md`: human-readable manual (mission, usage, examples, relationships)

---

## 🧩 Core Agents

| ID       | Title                    | Description                                                   |
|----------|--------------------------|---------------------------------------------------------------|
| [`Forge`](./forge.md)   | Master Builder            | Builds, connects, and maintains code architecture             |
| [`Nova`](./nova.md)     | Visual Architect          | Designs interfaces, layout, and component systems             |
| [`Quill`](./quill.md)   | Voice of the Mission      | Crafts persuasive, strategic copy and UX writing              |
| [`Echo`](./echo.md)     | Voice of the User         | Refines journeys and ensures usability and empathy            |
| [`Shield`](./shield.md) | Guardian of Quality       | Validates, tests, and ensures security and reliability        |
| [`Pulse`](./pulse.md)   | Strategic Navigator       | Aligns actions with product vision and business strategy      |
| [`Scope`](./scope.md)   | Intelligence Sentinel     | Analyzes competition and external trends                      |
| [`Scroll`](./scroll.md) | Keeper of Knowledge       | Documents features, decisions, and system flows               |

---

## 🌱 Optional / Future Agents (Suggested)

These agents are not yet implemented, but can be created by extending the current system:

| ID       | Title                  | Suggested Role                                               |
|----------|------------------------|--------------------------------------------------------------|
| `Flux`   | Delivery Engineer      | Automates CI/CD, infra setup, and deployment workflows       |
| `Ghost`  | Observability Analyst  | Tracks real-time performance and system anomalies            |
| `Oracle` | Predictive Analyst     | Surfaces insights using AI predictions and trends            |
| `Link`   | Integration Specialist | Manages API connectivity and service integration             |
| `Scout`  | Research Companion     | Supports user interviews and product discovery efforts       |

> You can add these or define your own — the system is fully extensible.

---

## 🧠 How Agents Work

- Defined in a `project.yaml` under `projects/your-project/`
- Activated by setting `enabled: true`
- Each reads its `file_context` to perform scoped, autonomous tasks
- Orchestrated by you — the human architect — using natural instructions

---

## 🛠 Example `project.yaml` Usage

```yaml
agents:
  - id: Forge
    path: ./templates/default/agents/forge.yaml
    role: "Builds and structures the core codebase"
    enabled: true

  - id: Quill
    path: ./templates/default/agents/quill.yaml
    role: "Crafts user-facing and internal communication"
    enabled: true
```

---

## 🧪 Adding New Agents

To create your own agent:

1. **Duplicate** an existing `.yaml` and `.md` file in this directory
2. **Define** the following fields:
   - `id`, `title`, `description`
   - `persona_prompt`, `skills`, `rules`, `examples`
   - `file_context` (e.g., input files like `product-vision.md`, `tone-of-voice.md`, etc.)
3. **Reference the agent** in your `project.yaml` under `agents`

> Agents are fully modular. Mix, match, and specialize them per mission.

---

## ⚙️ Execution (WIP)

In the current version, CraftAI agents are executed manually through LLMs like **ChatGPT**, **Claude**, or similar platforms.
A runtime executor is under development to allow for **automated orchestration**, context parsing, and agent chaining.