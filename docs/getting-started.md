# 🚀 Getting Started with CraftAI

Welcome to CraftAI — a human–AI framework for building software with hybrid teams.  
This guide walks you through how to set up, configure, and run your first CraftAI project.

---

## 📁 Project Structure

Your CraftAI project should follow this structure:

```
craftai/
├── templates/
│   └── default/
│       ├── agents/
│       └── branding/, tech/, product/, ...
├── projects/
│   └── your-project/
│       └── project.yaml
├── docs/
│   ├── getting-started.md
│   └── file-disciplines.md
```

---

## 1️⃣ Step 1 — Clone the Framework

```bash
git clone https://github.com/bs3dev/craftai.git
cd craftai
```

---

## 2️⃣ Step 2 — Explore Available Agents

Each agent is defined in `./templates/default/agents/` and includes:

- A persona definition (`persona_prompt`)
- Skills and behavior rules
- Files they rely on (`file_context`)
- Real-world examples of usage

📄 See [`agents/README.md`](../templates/default/agents/README.md) for an overview.

---

## 3️⃣ Step 3 — Define Your Project

Inside `./projects/your-project/`, create a `project.yaml`.  
This file declares:

- The project name, goals, and context
- Which agents are involved and enabled
- The files that agents should reference

📁 See `projects/your-project/project.yaml` for a working example.

---

## 4️⃣ Step 4 — Start Orchestrating

CraftAI doesn’t require a UI. You can use any LLM interface (e.g. ChatGPT, Claude) to act as the Orchestrator.

Just give a prompt like:

> “Forge, scaffold a Flutter app using Clean Architecture.”  
> “Quill, write a landing page headline aligned with our tone of voice.”  
> “Echo, suggest UX improvements for our onboarding screen.”

The agent uses its `.yaml` profile and relevant context files to execute the task.

---

## 🧠 Tips for Prompting Agents

- Address the agent by name (e.g. "Forge", "Nova")
- Be concise but specific about what you want
- Mention which project you're working on if applicable
- Ask for explanations or step-by-step output when needed

---

## 🛠 Want to Add a New Agent?

1. Copy any `.yaml` file in `/templates/default/agents/`
2. Customize `id`, `title`, `persona_prompt`, `skills`, and `rules`
3. Add the agent to your `project.yaml` under the `agents:` section

> Agents are fully modular — define the team you need per project.

---

## 🧪 Runtime (Coming Soon)

CraftAI will soon support a local execution engine via CLI.

```bash
npx craftai run projects/your-project
```

Until then, agent execution happens via manual prompt orchestration in any LLM.

---

## 🧭 Learn More

- 📚 See [`docs/file-disciplines.md`](./file-disciplines.md) for all supported file types and their purpose  
- 📄 Explore each agent in [`templates/default/agents/`](../templates/default/agents/)  
- 🧰 Use templates in `templates/default/` to build your context files

---

## 💬 Questions?

Open an issue or reach us at [bs3.dev](https://bs3.dev).  
We'd love to hear how you're crafting with AI.
