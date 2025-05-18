# 🚀 Getting Started with CraftAI

Welcome to CraftAI — a human–AI framework for building software with hybrid teams.  
This guide will walk you through how to set up, configure, and run your first CraftAI project.

---

## 📁 Project Structure

Your CraftAI project should follow this base structure:

```
craftai/
├── agents/                # Agent definitions (.yaml)
│   ├── Forge.yaml
│   └── ...
├── projects/
│   └── your-project/
│       └── project.yaml
├── branding/, tech/, ...  # Context folders referenced in project.yaml
└── docs/                  # Documentation like this guide
```

---

## 1️⃣ Step 1 — Clone the Framework

```bash
git clone https://github.com/bs3dev/craftai.git
cd craftai
```

---

## 2️⃣ Step 2 — Explore Available Agents

Each agent is defined in `./agents/` and includes:

- A persona definition (`persona_prompt`)
- Skills and examples
- Files they rely on (`file_context`)
- Rules they follow strictly

📄 Check [`./agents/README.md`](../agents/README.md) for a full list.

---

## 3️⃣ Step 3 — Define Your Project

Inside `./projects/your-project/`, create a `project.yaml`.  
This file declares:

- The project goals and description
- Which agents are involved
- What context files are available (branding, vision, code style, etc.)

> 📁 See `project.en.yaml` in the root folder for an example.

---

## 4️⃣ Step 4 — Start Orchestrating

CraftAI doesn’t require a UI to start. You can use ChatGPT or any LLM interface to orchestrate the agents by giving prompts like:

> “Forge, create a Flutter app scaffold based on Clean Architecture.”  
> “Quill, write a recruitment headline aligned with our tone of voice.”  
> “Echo, suggest UX improvements for the onboarding form.”

The agent uses its `.yaml` profile and relevant context to execute the task.

---

## 🧠 Tips for Prompting Agents

- Address the agent by name (e.g. "Forge", "Quill")
- Be specific but concise in what you want
- Let the agent know which project and context it's working with

---

## 🧪 Want to Add a New Agent?

1. Duplicate any `.yaml` file in `/agents/`
2. Customize the `id`, `title`, `persona_prompt`, and skillset
3. Reference it in your `project.yaml` to activate

---

## 💬 Questions?

Open an issue or ping us at [bs3.dev](https://bs3.dev).  
We'd love to hear how you're crafting with AI.

