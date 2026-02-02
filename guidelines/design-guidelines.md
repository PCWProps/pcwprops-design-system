# PCWProps Design Guidelines

## Liquid Glass UI — Section 1 (Guidelines)

Guidelines are **non-negotiable rules** that constrain behavior. Style tokens execute these rules.

---

## 1. System Intent

- The UI must feel **cinematic, immersive, modern, and on the cutting edge**.
- Avoid conventional vertical scrolling. Pages should evolve through **scenes, transitions, and scroll-locked moments**.
- Visual complexity is encouraged **when it serves narrative flow**.
- Clarity is required at the level of hierarchy and intent, not simplicity of visuals.

---

## 2. Reuse & System Integrity (Hard Rules)

- Reuse existing components, tokens, and styles first.
- If new styles are required, they **must be added** to the shared variable/token system.
- No orphan styles, colors, animations, or effects are permitted.
- Every system extension must support **both Dark and Light modes**.

---

## 3. Dark ↔ Light Mode Rules

- **PCW Dark Mode** is canonical.
- **PCW Light Mode** is a true counterpart, never a direct inversion.
- Dark and Light modes must share **identical token names and structure**.
- Any new token must be defined for **both modes simultaneously**.

---

## 4. Motion & Narrative Rules

- Motion, depth, and hierarchy must choreograph a **cinematic page evolution**.
- Scroll-lock, layered transitions, and scene-based progression are encouraged.
- Motion must feel controlled, intentional, and premium — never playful.

---

## 5. Animation Governance

- All animations must be reusable system variants.
- Every animation requires:
  - A named animation token
  - A CSS flag
  - A defined z-index
- No inline or one-off animations are allowed.

---

## 6. Reject Output Checklist (Make QA)

Reject output if any of the following occur:

- One-off colors, gradients, or opacity values appear
- Animations exist without tokens, flags, or z-index
- Light mode diverges structurally from Dark mode
- Layout resolves into a simple vertical scroll
- Components are duplicated instead of extended

---

## 7. Design Primitives: Scroll Narrative

- **Scene:** A locked visual state
- **Act:** A sequence of scenes
- **Transition:** The motion between scenes

Pages should be composed as **Acts**, not sections.

---

## 8. Component Rules

- All components must be **variant-based** and **token-driven**.
- New components **extend** the system; they do **not fork** it.
- Allow **one primary CTA per scene**.

---

## 9. Dual-Mode Make Prompt Pattern

Use this pattern when running Make:

> Generate Dark and Light mode variants in one run.
> Use identical token names and component structure.
> Apply Dark mode as canonical; derive Light mode accordingly.

---

## 10. System Objective

This system must support:

- Full parity across Dark/Light, Web/App, Static/Animated
- Highly animated, immersive, modern interfaces
- Long-term reuse without drift
- Direct parity between design, Make output, and CSS implementation

---

**Next:** Review [Style Tokens](../styles/STYLE_TOKENS.md) to execute these rules.
