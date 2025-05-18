# CRAFTAI.md

## 🧬 Core Architecture of CraftAI

CraftAI is a human–AI framework that enables **multi-agent, multi-task collaboration** for building software.  
It merges agent-based software thinking with a creative and orchestration-first approach to development.

---

## 🔁 The Shift from Execution to Orchestration

In traditional software teams, humans write, review, test, and deploy code.  
In CraftAI, **humans orchestrate** — and **agents execute**.

A developer becomes a *conductor*, guiding a team of intelligent agents that perform tasks such as:

- 📦 Implementing features
- 🧹 Refactoring modules
- 🧪 Testing and validating code
- 📄 Writing documentation
- 🎨 Designing user interfaces
- 📊 Analyzing architecture
- 🧭 Refining product strategy
- 📣 Communicating product value
- 🔍 Researching competitors and trends
- 💡 Translating user needs into requirements

---

## 🧠 System Overview

```
           +----------------+
           |  Orchestrator  |
           |  (Human Lead)  |
           +--------+-------+
                    |
         +----------▼-----------+
         |     Orchestration    |     <- Task routing, monitoring, validation
         |       Engine         |
         +----------+-----------+
                    |
     +--------------+--------------+
     |              |              |
+----▼----+    +----▼----+    +----▼----+
| Agent A |    | Agent B |    | Agent C |
|  Tech   |    | Content |    |  Data   |
+---------+    +---------+    +---------+
     |              |              |
[ Feature ]   [ Doc PR ]     [ Analytics ]
```

---

## ⚙️ Components

### 1. **Orchestrator (Human Role)**
- Writes tasks in natural language
- Assigns agents
- Reviews and merges output

### 2. **Execution Engine (Planned)**
- Parses task definitions
- Dispatches them to the appropriate agents
- Collects results and presents summaries

### 3. **Agent Definitions**
Stored as `.md` or `.json`, each agent includes:

```yaml
name: tech-agent
description: Writes and refactors code.
skills:
  - build-feature
  - improve-code
  - write-tests
context:
  repos: ["frontend/", "backend/"]
  rules: ["Clean Architecture", "Test Coverage > 80%"]
```

### 4. **Playbooks**
Reusable task templates:

```yaml
task: build-feature
description: Create a new feature based on user story
input:
  - title
  - acceptance_criteria
steps:
  - generate spec
  - scaffold code
  - write tests
  - open PR
```

---

## 🧪 Agent Lifecycle

| Phase | Description |
|-------|-------------|
| **Load** | Agent is initialized with access to repo and config |
| **Understand** | Agent reads task prompt, gathers context |
| **Plan** | Agent proposes steps and structure |
| **Act** | Agent performs edits, opens PR |
| **Validate** | Agent runs tests and/or peer review |

---

## 🛰 Example: A Day in CraftAI

### Scenario:
You write the instruction:

> “Refactor the checkout component to follow Clean Architecture and improve testability.”

CraftAI:

1. Selects the `tech-agent`
2. Parses the prompt
3. Generates a plan
4. Edits the code in `frontend/checkout/`
5. Runs tests
6. Opens a PR
7. Posts the summary back to the orchestrator

All within minutes.

---

## 🌱 Future Directions

- Agent marketplace (plug third-party agents)
- Visual orchestrator UI
- Integration with GitHub Apps & Actions
- Support for voice-based instructions
- Real-time collaboration between human & agents

---

## 🧭 Final Note

CraftAI is not just a framework.  
It’s a reimagination of how software is created in the age of intelligent systems.

Join the craft.
