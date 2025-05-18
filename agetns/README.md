# 🧠 CraftAI Agents Directory

This folder contains all the agents available in the CraftAI ecosystem.

Each agent represents a highly specialized AI teammate with a defined purpose, skillset, and execution style — designed to operate autonomously, guided by natural language instructions and project context.

---

## 🧩 Core Agents (Defined)

| ID       | Name (Title)               | Role Description                                                  |
|----------|----------------------------|-------------------------------------------------------------------|
| **Forge**   | Master Builder              | Builds, connects, and maintains code architecture and structure  |
| **Nova**    | Visual Architect            | Designs interfaces, layout, and component systems                |
| **Quill**   | Voice of the Mission        | Crafts persuasive, strategic copy and UX writing                 |
| **Echo**    | Voice of the User           | Refines journeys, ensures usability and empathy                  |
| **Shield**  | Guardian of Quality         | Validates, tests, and ensures security and reliability           |
| **Pulse**   | Strategic Navigator         | Aligns all actions with product vision and business strategy     |
| **Scope**   | Intelligence Sentinel       | Analyzes competition and external trends                         |
| **Scroll**  | Keeper of Knowledge         | Documents all technical and strategic decisions                  |

---

## 🌱 Optional / Future Agents (Suggested)

These agents are not defined yet, but can be added to the system as needed.

| ID       | Name (Title)           | Role Description                                                   |
|----------|------------------------|--------------------------------------------------------------------|
| **Flux**     | Delivery Engineer       | Automates CI/CD, environment config, deployment pipelines          |
| **Ghost**    | Observability Analyst   | Monitors product usage and performance in real time               |
| **Oracle**   | Predictive Analyst      | Surfaces data-driven insights, churn risks, and behavioral trends |
| **Link**     | Integration Specialist  | Handles API communication, system bridges, external services      |
| **Scout**    | Research Companion      | Supports user interviews, product discovery and field insights    |

---

## 📂 Agent Files

Each agent is defined in its own `.yaml` file, containing:

- A short identity and mission
- A `persona_prompt` for roleplay-based reasoning
- Skills, examples, and contextual file bindings
- Rules that govern behavior and quality

> See examples like `Forge.yaml`, `Quill.yaml`, etc. to get started creating your own.

---

## ✨ Want to add your own agent?

1. Copy one of the existing `.yaml` files as a template.
2. Define a new `id`, `title`, and `persona_prompt`.
3. Specify the skills, file_context, rules, and examples.
4. Reference your agent in a project by adding it to `project.yaml`.

