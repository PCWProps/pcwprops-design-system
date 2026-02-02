# PCWProps Color System

**Brand Palette:** Deep Navy, Gold, White  
**System:** Liquid Glass UI (Dark Mode Canonical)

---

## Color Palette

### Primary Colors

| Color         | Hex     | RGB         | HSLA           | Usage                              |
| ------------- | ------- | ----------- | -------------- | ---------------------------------- |
| Deep Navy     | #0B1020 | 11, 16, 32  | 217°, 49%, 8%  | Primary backgrounds, dominant      |
| Midnight Blue | #162447 | 22, 36, 71  | 217°, 52%, 18% | Secondary containers, secondary bg |
| Royal Blue    | #1F3C88 | 31, 60, 136 | 217°, 62%, 33% | Interactive states, tertiary       |

### Accent Colors

| Color        | Hex     | RGB           | HSLA          | Usage                              |
| ------------ | ------- | ------------- | ------------- | ---------------------------------- |
| Antique Gold | #B9A14A | 185, 161, 74  | 44°, 43%, 51% | Accents, highlights, tertiary text |
| Soft Gold    | #F2D675 | 242, 214, 117 | 44°, 81%, 70% | Primary accents, interactive, text |

### Neutral & System

| Color          | Hex     | RGB           | HSLA         | Usage                            |
| -------------- | ------- | ------------- | ------------ | -------------------------------- |
| White          | #FFFFFF | 255, 255, 255 | 0°, 0%, 100% | Text, high contrast, light mode  |
| Charcoal Black | #0A0A0A | 10, 10, 10    | 0°, 0%, 4%   | Maximum contrast, dark mode text |

### Semantic Colors (State)

| State   | Color | Hex     | Usage                      |
| ------- | ----- | ------- | -------------------------- |
| Success | Green | #4CAF50 | Approval, success feedback |
| Warning | Amber | #FFC107 | Caution, warning messages  |
| Error   | Red   | #F44336 | Errors, critical feedback  |
| Info    | Blue  | #2196F3 | Informational messages     |

---

## Color Modes

### Dark Mode (Canonical)

Deep navy as foundation; gold as accent; white for contrast.

```
Backgrounds:    #0B1020 → #162447 → #1F3C88
Text:          #FFFFFF (primary), #F2D675 (secondary)
Interactive:   #F2D675, #B9A14A
Borders:       rgba(255, 255, 255, 0.1)
Disabled:      rgba(255, 255, 255, 0.25 - 0.5)
```

### Light Mode (Structural Counterpart)

White as foundation; blue interactive; inverted gold for contrast.

```
Backgrounds:    #FFFFFF → #F5F5F5 → #EEEEEE
Text:          #0A0A0A (primary), #8B7A1F (secondary)
Interactive:   #1F3C88, #2E5FA0
Borders:       rgba(10, 10, 10, 0.1)
Disabled:      rgba(10, 10, 10, 0.12 - 0.38)
```

---

## Glass Opacity Layers

Glass elements use color + opacity for depth.

### Dark Glass Layers

```
glass.primary       rgba(22, 36, 71, 0.7)    + blur(12px)
glass.secondary     rgba(31, 60, 136, 0.6)   + blur(8px)
glass.tertiary      rgba(22, 36, 71, 0.4)    + blur(4px)
glass.active        rgba(31, 60, 136, 0.85)  + blur(16px)
```

### Light Glass Layers

```
glass.primary       rgba(245, 245, 245, 0.9) + blur(12px)
glass.secondary     rgba(238, 238, 238, 0.8) + blur(8px)
glass.tertiary      rgba(245, 245, 245, 0.5) + blur(4px)
glass.active        rgba(238, 238, 238, 0.95)+ blur(16px)
```

---

## Contrast Ratios

All color combinations meet WCAG AA accessibility standards:

| Foreground      | Background          | Contrast | WCAG |
| --------------- | ------------------- | -------- | ---- |
| #FFFFFF (White) | #0B1020 (Deep Navy) | 15.4:1   | AAA  |

# PCWProps Color System

**Brand Palette:** Deep Navy, Gold, White  
**System:** Liquid Glass UI (Dark Mode Canonical)

---

## Base Colors

| Color          | Hex     | RGB           | Usage                            |
| -------------- | ------- | ------------- | -------------------------------- |
| Deep Navy      | #0B1020 | 11, 16, 32    | Primary backgrounds              |
| Midnight Blue  | #162447 | 22, 36, 71    | Secondary containers             |
| Royal Blue     | #1F3C88 | 31, 60, 136   | Interactive states               |
| Antique Gold   | #B9A14A | 185, 161, 74  | Accents, highlights              |
| Soft Gold      | #F2D675 | 242, 214, 117 | Primary accents, text highlights |
| White          | #FFFFFF | 255, 255, 255 | Text, light mode surfaces        |
| Charcoal Black | #0A0A0A | 10, 10, 10    | Maximum contrast                 |

## Transparency Tokens

Applied **only via tokens**:

```
alpha.90 = 0.9
alpha.80 = 0.8
alpha.70 = 0.7
alpha.60 = 0.6
alpha.50 = 0.5
alpha.40 = 0.4
alpha.30 = 0.3
alpha.20 = 0.2
alpha.10 = 0.1
```

## Modes

### Dark Mode (Canonical)

```
Backgrounds:    #0B1020 → #162447 → #1F3C88
Text:           #FFFFFF (primary), #F2D675 (secondary)
Interactive:    #F2D675, #B9A14A
Borders:        rgba(255, 255, 255, 0.1)
Disabled:       rgba(255, 255, 255, 0.25–0.5)
```

### Light Mode (Structural Counterpart)

```
Backgrounds:    #FFFFFF → #F5F5F5 → #EEEEEE
Text:           #0A0A0A (primary), #8B7A1F (secondary)
Interactive:    #1F3C88, #2E5FA0
Borders:        rgba(10, 10, 10, 0.1)
Disabled:       rgba(10, 10, 10, 0.12–0.38)
```

## Glass Layers

### Dark Glass

```
glass.primary     rgba(22, 36, 71, 0.7)   + blur(12px) + z:10
glass.secondary   rgba(31, 60, 136, 0.6)  + blur(8px)  + z:8
glass.tertiary    rgba(22, 36, 71, 0.4)   + blur(4px)  + z:5
glass.active      rgba(31, 60, 136, 0.85) + blur(16px) + z:+10
```

### Light Glass

```
glass.primary     rgba(245, 245, 245, 0.9)  + blur(12px)
glass.secondary   rgba(238, 238, 238, 0.8)  + blur(8px)
glass.tertiary    rgba(245, 245, 245, 0.5)  + blur(4px)
glass.active      rgba(238, 238, 238, 0.95) + blur(16px)
```

## Required Gradient Tokens

- `gradient.glass.primary`
- `gradient.glass.secondary`
- `gradient.background.depth`
- `gradient.accent.gold`
- `gradient.interactive.hover`

## Usage & Accessibility

- Dark Mode is canonical; Light Mode is a structural counterpart with identical token names.
- No one-off hex values; all opacity applied via `alpha.*` tokens.
- Maintain WCAG AA contrast (4.5:1+) for text/background pairs.

---

**Part of:** [Style Tokens](STYLE_TOKENS.md) system  
**Reference:** [Design Guidelines](../guidelines/DESIGN_GUIDELINES.md)
