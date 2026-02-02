# PCWProps Style Tokens

## Liquid Glass UI — Section 2 (Style)

Style defines tokens, systems, and primitives that execute the Guidelines.

---

## 7. Token Architecture & Naming Conventions

**Token Naming**

- Colors: `color.{mode}.{group}.{role}`
- Alpha: `alpha.{value}`
- Gradients: `gradient.{context}.{type}`
- Glass: `glass.{variant}.{property}`
- Motion: `motion.{purpose}.{property}`

**Examples**

- `color.dark.surface.primary`
- `gradient.glass.primary`
- `motion.glass.reveal.duration`

---

## 8. Color System (Future-Proof)

### Modes

- PCW Dark Mode (Primary)
- PCW Light Mode (Secondary)

### Base Colors

- Deep Navy: #0B1020
- Midnight Blue: #162447
- Royal Blue: #1F3C88
- Antique Gold: #B9A14A
- Soft Gold: #F2D675
- White: #FFFFFF
- Charcoal Black: #0A0A0A

### Transparency Tokens

```
alpha.90 → 0.9
alpha.80 → 0.8
alpha.70 → 0.7
alpha.60 → 0.6
alpha.50 → 0.5
alpha.40 → 0.4
alpha.30 → 0.3
alpha.20 → 0.2
alpha.10 → 0.1
```

Transparency is applied **only via tokens**.

---

## 9. Gradient System

### Supported Types

- Linear
- Radial
- Conic
- Mesh (layered)

### Required Gradient Tokens

- `gradient.glass.primary`
- `gradient.glass.secondary`
- `gradient.background.depth`
- `gradient.accent.gold`
- `gradient.interactive.hover`

Gradients must enhance depth and cinematic flow.

---

## 10. PCW Liquid Glass Material System

### Core Rules

- Glass is layered, translucent, and depth-aware.
- Glass containers should be flex-based primitives.
- Glass must actively participate in motion and narrative flow.

### Glass Variants

**Primary**

- z-index: 10
- CSS flag: `--pcw-glass-primary`

**Secondary**

- z-index: 8
- CSS flag: `--pcw-glass-secondary`

**Tertiary**

- z-index: 5
- CSS flag: `--pcw-glass-tertiary`

**Active**

- z-index: +10
- CSS flag: `--pcw-glass-active`

Light-mode glass must reduce blur and increase contrast to preserve readability.

---

## 11. Motion & Animation Token System

### Timing Tokens

- `motion.duration.fast`
- `motion.duration.medium`
- `motion.duration.slow`

### Easing Tokens

- `motion.ease.in`
- `motion.ease.out`
- `motion.ease.inOut`

### Scroll Tokens

- `motion.scroll.lock`
- `motion.scroll.release`

All motion must reference these tokens.

---

## 12. Scroll Narrative Primitives

- **Scene**: A locked visual state
- **Act**: A sequence of scenes
- **Transition**: The motion between scenes

Pages should be composed as **Acts**, not sections.

---

## 13. Component Rules

- All components must be variant-based and token-driven.
- New components extend the system; they do not fork it.
- One primary CTA per scene.

---

## 14. Dual-Mode Make Prompt Pattern

Use this pattern when running Make:

> Generate Dark and Light mode variants in one run.
> Use identical token names and component structure.
> Apply Dark mode as canonical; derive Light mode accordingly.

---

## 15. System Objective

This system must support:

- Full parity across Dark/Light, Web/App, Static/Animated
- Highly animated, immersive, modern interfaces
- Long-term reuse without drift
- Direct parity between design, Make output, and CSS implementation

---

**Reference:** See [Color System](COLOR_SYSTEM.md) for palette details and [Guidelines](../guidelines/DESIGN_GUIDELINES.md) for constraints.
