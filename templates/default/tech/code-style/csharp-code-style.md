# ✨ C# Code Style & Clean Coding Guidelines

> This document defines the coding conventions and clean code principles for C# projects.  
> It serves as a shared guide to ensure readability, consistency, and maintainability.

---

## 🎯 Purpose

To promote a consistent, human-readable codebase by applying clean code principles, reducing technical debt, and improving collaboration across teams and AI agents.

---

## 🧠 Used by Agents

- **Forge**: for code generation and scaffolding
- **Shield**: for static analysis, linting, and test enforcement
- **Scroll**: for documentation and code annotation

---

## 🧬 Naming Conventions

- **PascalCase**: for classes, interfaces, methods, and public properties.  
  Example: `CustomerService`, `CalculateTotal()`
- **camelCase**: for local variables, method parameters, and private fields.  
  Example: `orderTotal`, `customerName`
- **Field prefixes**:
  - Private fields: `_` (e.g., `_orderRepository`)
  - Static fields: `s_` (e.g., `s_instance`)
  - Thread-static: `t_` (e.g., `t_localData`)

> Reference: [C# Identifier Naming Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names)

---

## 🧩 Formatting & Structure

- Indentation: Use 4 spaces; do not use tabs.
- Braces: Always use braces `{}` — even for single-line blocks.
- Line spacing: Use blank lines to group logical sections.
- One declaration per line.

---

## 🧱 Clean Code Principles

Based on Clean Code and Refactoring fundamentals:

- **Readability first**: Code should be easy to scan and understand.
- **Single Responsibility**: Functions and classes should do one thing.
- **DRY**: Avoid duplication at all costs.
- **KISS**: Keep it simple — avoid unnecessary complexity.
- **YAGNI**: Don’t build what you don’t need (yet).
- **Refactor often**: Improve structure continuously without changing behavior.

---

## 🧹 Comments & Documentation

- **Self-explanatory code > comments**
- Comment only when the *why* is unclear from the *what*
- Use XML documentation (`///`) for public APIs and classes
- Keep comments accurate and updated

---

## 🧪 Testing & Quality Assurance

- **Unit tests**: Required for all business logic and critical paths
- **Test coverage**: Aim for > 80% meaningful coverage
- **TDD**: Consider for new modules and high-risk areas
- **Tools**: xUnit, NUnit, MSTest; static analysis via SonarQube or Resharper

---

## 📁 Project Structure

- Structure code by feature or layer (e.g., `Controllers`, `Services`, `Repositories`)
- Use clear and consistent folder and file naming
- Maintain clear separation of concerns

---

## 🔧 Tooling & Automation

- Linters: StyleCop, Roslyn Analyzers
- Formatters: Visual Studio Code Format, Resharper
- CI Integration: Enforce style and tests in pull requests

---

## ✅ Consistency Checklist

- [ ] Are naming conventions consistently applied?
- [ ] Are functions and classes focused and small?
- [ ] Is the code formatted and linted?
- [ ] Are comments used sparingly and meaningfully?
- [ ] Are unit and integration tests present?
- [ ] Are Clean Code principles visibly followed?

---

## 📚 Reference Links

- [Microsoft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)
- [Identifier Naming Rules](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names)
- [Clean Code by Robert C. Martin](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)
- [Refactoring by Martin Fowler](https://martinfowler.com/books/refactoring.html)
- [Martin Fowler on Clean Code](https://martinfowler.com/tags/clean%20code.html)

---

> *“Any fool can write code that a computer can understand. Good programmers write code that humans can understand.”*  
> — Martin Fowler
