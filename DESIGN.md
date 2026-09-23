---
version: alpha
name: Design Tokens
description: Shared color, type, radius, and spacing for sites that use this package. Component specs stay in each product repo.
colors:
  primary: "{colors.ink}"
  secondary: "{colors.ink-muted}"
  tertiary: "{colors.accent}"
  neutral: "{colors.canvas}"
  canvas: "#0A0A0A"
  canvas-elevated: "#171717"
  canvas-subtle: "#0A0A0ACC"
  ink: "#F5F5F5"
  ink-muted: "#A3A3A3"
  ink-subtle: "#737373"
  line: "#262626"
  line-strong: "#404040"
  line-soft: "#262626CC"
  accent: "#6EE7B7"
  accent-muted: "#34D399CC"
  cta: "#F5F5F5"
  cta-fg: "#0A0A0A"
typography:
  display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: -0.025em
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.625
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.625
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.625
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
  label-caps:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.14em
  mono-meta:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
rounded:
  control: 0.5rem
  card: 1rem
  pill: 9999px
spacing:
  grid: 1rem
  section-sm: 4rem
  section-md: 5rem
  section-lg: 6rem
  content-max: 72rem
  media: 18rem
  media-lg: 20rem
---

# Design tokens

This repository is the only place to edit shared color, type, radius, and spacing. `tokens.css` is what the sites compile. This file is the same values in Google's DESIGN.md schema, for agents and exporters.

Product repos keep their own component specs and page rules. They install this package and import `design-tokens/tokens.css`. They do not copy these values into a second `tokens.css`.

## Colors

Near-black neutrals with one phosphor accent.

- **Canvas (`#0A0A0A`):** Page background.
- **Canvas elevated (`#171717`):** Cards and raised panels.
- **Ink (`#F5F5F5`):** Primary text.
- **Ink muted (`#A3A3A3`):** Body copy.
- **Ink subtle (`#737373`):** Meta and eyebrows.
- **Line (`#262626`, strong `#404040`):** Default and hover borders.
- **Accent (`#6EE7B7`):** Code and system signals. Never a primary button fill.
- **CTA (`#F5F5F5` on `#0A0A0A`):** Inverse primary actions.

## Typography

**Inter** for UI text. **JetBrains Mono** for meta and code.

## Shapes

- **Control (`0.5rem`):** Small controls and code chips.
- **Card (`1rem`):** Surfaces and media frames.
- **Pill (`9999px`):** Primary buttons and tags.

## Rules

- Change a value here, then install the updated package in each site.
- Do not add a new hex value in a product repo. Add the token here first.
- Accent is for code and system signals.
- Primary actions use the inverse CTA pair.
