# 🎨 Design System Reference Guide

> This document is not a design system.  
> It guides agents and collaborators on how to find, interpret, and use the official design system of the product — ensuring consistency and adherence to the brand’s UI/UX foundations.

---

## 🎯 Purpose

To serve as a central guide for interacting with the design system — aligning all visual, structural, and interactive elements produced by agents or developers with the established brand design language.

---

## 🧠 Used by Agents

- **Nova**: to generate UI layouts, components, and screens
- **Echo**: to align tone and visuals in conversational UI
- **Forge**: to scaffold front-end structure using design tokens
- **Scroll**: to embed design rules in documentation or specs

---

## 📁 Design System Sources

> Use these references as the **single source of truth** for UI decisions.

| Resource              | Link / Location                          | Notes                        |
|------------------------|------------------------------------------|-------------------------------|
| Figma Library          | https://figma.com/file/XXXX              | Main component and token set |
| Storybook             | https://design.company.com/storybook     | Live preview of components   |
| Token Documentation   | https://zeroheight.com/p/brand-guidelines| Includes spacing, color, type |
| Design Git Repository | https://github.com/org/design-system     | For development usage        |

---

## 🧩 What the Design System Defines

| Layer               | Examples                                      |
|---------------------|-----------------------------------------------|
| Foundations         | Spacing, color palette, typography, radius    |
| Components          | Buttons, modals, inputs, forms, nav           |
| Patterns            | Onboarding, authentication, empty states      |
| Motion & Feedback   | Loading, transitions, system statuses         |
| Accessibility       | Contrast, keyboard nav, screen reader support |

---

## 🧠 How Agents Should Use It

- Always match component **names** and **semantics** from the source system (ex: `PrimaryButton`, not `BlueCTA`)
- Use **tokens**, not hardcoded values (ex: `$spacing-md`, `$color-primary`)
- Validate **contrast and hierarchy** for accessibility
- When in doubt, prefer **existing patterns** over new UI metaphors

---

## 🤖 API / Component Access

If generating code:

- Use imports from the design system library (e.g., `@company/ui`)
- Fallback to Storybook or design token references if uncertain
- Never invent UI logic outside of defined components unless explicitly instructed

---

## ✅ Compliance Checklist

- [ ] Are all components mapped to the source design system?
- [ ] Are tokens used instead of hardcoded values?
- [ ] Is the layout consistent with documented spacing and grids?
- [ ] Does the generated UI follow accessibility rules?
- [ ] Are component names and states aligned with Figma/Storybook?

---

## 📚 Reference Links

- [Google Material Design (M3)](https://m3.material.io/)
- [Design Systems Handbook by InVision](https://www.designbetter.co/design-systems-handbook)
- [Storybook Accessibility Addon](https://storybook.js.org/addons/@storybook/addon-a11y/)
- [Design Tokens W3C Draft](https://design-tokens.github.io/community-group/format/)

---

> *A strong design system is more than aesthetics — it’s the DNA of your product experience. Agents and humans must speak its language fluently.*
