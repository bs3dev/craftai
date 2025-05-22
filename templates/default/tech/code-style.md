# ✨ Code Style & Clean Coding Guidelines

> This document defines the coding standards and clean code principles that ensure our codebase remains readable, maintainable, and scalable.  
> It serves as a shared contract for all contributors and agents.

---

## 🎯 Purpose

To promote a consistent and human-readable codebase by applying clean code principles, reducing technical debt, and facilitating collaboration across teams and agents.

---

## 🧠 Used by Agents

- **Forge**: for generating and scaffolding code
- **Shield**: for enforcing static analysis, linting, and test coverage
- **Scroll**: for generating documentation and code annotations

---

## 🧬 Core Principles

Inspired by *Clean Code* and *Refactoring*:

- **Readability First**: Code should be easy to read and understand.
- **Single Responsibility**: Each function or class should have one purpose.
- **DRY (Don't Repeat Yourself)**: Avoid code duplication.
- **KISS (Keep It Simple, Stupid)**: Simplicity over complexity.
- **YAGNI (You Aren't Gonna Need It)**: Implement only what's necessary.
- **Refactor Often**: Continuously improve the code structure without altering its behavior.

---

## 🧾 Naming Conventions

- Use descriptive and meaningful names for variables, functions, and classes.
- Follow consistent casing:
  - `camelCase` for variables and functions.
  - `PascalCase` for classes and components.
  - `UPPER_SNAKE_CASE` for constants.
- Avoid abbreviations and single-letter names, except for loop indices.

---

## 🧩 Functions and Methods

- Keep functions short and focused; ideally, no more than 20 lines.
- Each function should perform a single task.
- Use descriptive names that convey the function's purpose.
- Limit the number of parameters; prefer objects or parameter objects for multiple related parameters.

---

## 🧱 Classes and Modules

- Adhere to the Single Responsibility Principle.
- Keep classes small and focused.
- Organize code into modules that encapsulate related functionality.
- Use interfaces or abstract classes to define contracts when appropriate.

---

## 🧹 Comments and Documentation

- Write self-explanatory code that minimizes the need for comments.
- Use comments to explain the "why" behind complex logic, not the "what".
- Maintain up-to-date documentation for public APIs and modules.
- Utilize tools like JSDoc or TypeDoc for automated documentation generation.

---

## 🧪 Testing and Quality Assurance

- Write unit tests for all critical functions and components.
- Aim for high test coverage, but prioritize meaningful tests over coverage percentage.
- Use test-driven development (TDD) where applicable.
- Employ linting tools (e.g., ESLint) and formatters (e.g., Prettier) to enforce code style.

---

## 📁 Project Structure

- Organize files and directories by feature or domain.
- Use consistent naming for files and folders.
- Separate concerns: keep business logic, data access, and UI components in distinct layers.

---

## 🔧 Tooling and Automation

- Integrate linters, formatters, and static analysis tools into the development workflow.
- Set up pre-commit hooks to enforce code quality checks.
- Use continuous integration (CI) pipelines to automate testing and deployment processes.

---

## ✅ Consistency Checklist

- [ ] Are naming conventions consistently applied?
- [ ] Do functions and classes adhere to the Single Responsibility Principle?
- [ ] Is the code free of unnecessary comments and dead code?
- [ ] Are tests present and meaningful for critical functionality?
- [ ] Is the codebase free of duplication and follows DRY principles?
- [ ] Are code formatting and linting rules enforced automatically?

---

## 📚 Reference Links

- [Clean Code: A Handbook of Agile Software Craftsmanship](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)
- [Refactoring: Improving the Design of Existing Code](https://martinfowler.com/books/refactoring.html)
- [Martin Fowler’s Clean Code Articles](https://martinfowler.com/tags/clean%20code.html)
- [freeCodeCamp: How to Write Clean Code](https://www.freecodecamp.org/news/how-to-write-clean-code/)
- [Codacy: What Is Clean Code?](https://blog.codacy.com/what-is-clean-code)

---

> *"Any fool can write code that a computer can understand. Good programmers write code that humans can understand."*  
> — Martin Fowler
