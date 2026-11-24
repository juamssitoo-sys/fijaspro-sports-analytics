---
name: "FijasPro — Kinetic Telemetry"
description: "High-contrast dark graphite sports analytics and smart prediction design system blending stadium passion with quantitative precision."
---

## Overview

FijasPro is an intelligent sports analytics, live statistics, and model-driven prediction platform covering **Fútbol**, **NBA**, and **Esports (VALORANT & CS2)**. The visual identity fuses the adrenaline of championship broadcast graphics with the clarity of a quantitative telemetry terminal.

- **Brand Personality:** Intense, analytical, transparent, and athletic.
- **Target Audience:** Data-minded sports fans, analysts, and competitive followers who demand verified statistics separated clearly from predictive model estimates.
- **Design Style:** **High-Contrast Kinetic Dark** — deep graphite surfaces (`#111318` to `#282A2F`) paired with razor-sharp hairline dividers, intense competition accents (Blaze Coral, Tactical Emerald, Cyber Cyan), bold geometric headlines, and tabular monospace telemetry. Never resembles a betting house or a generic spreadsheet.

## Colors

The palette is anchored in deep graphite neutrals rather than pure `#000000` to prevent light-text halation. Intense accents signal live action, model confidence, and discipline identity while strictly respecting WCAG AA contrast.

- **Primary (`#FFB4A1` / Container `#FF5628`):** Blaze Coral — channels stadium energy, primary CTAs, and active navigation states.
- **Secondary (`#43FFBB`):** Tactical Emerald — signals live matches, verified historical data, and high-confidence model alignment.
- **Tertiary (`#7BD0FF`):** Cyber Cyan — highlights Esports telemetry (VALORANT / CS2), analytical breakdowns, and comparative charts.
- **Surfaces:** Layered graphite tiers (`surface-container-lowest` `#0C0E13` through `surface-container-highest` `#33353A`) establish depth without heavy drop shadows.

```yaml
colors:
  primary: "#FFB4A1"
  on-primary: "#611300"
  primary-container: "#FF5628"
  on-primary-container: "#540F00"
  secondary: "#43FFBB"
  on-secondary: "#003825"
  secondary-container: "#00E2A0"
  on-secondary-container: "#005F41"
  tertiary: "#7BD0FF"
  on-tertiary: "#00354A"
  tertiary-container: "#009BD1"
  on-tertiary-container: "#002D40"
  success: "#43FFBB"
  on-success: "#003825"
  warning: "#FBBF24"
  on-warning: "#3B2600"
  error: "#FFB4AB"
  on-error: "#690005"
  error-container: "#93000A"
  on-error-container: "#FFDAD6"
  background: "#111318"
  on-background: "#E2E2E9"
  surface: "#111318"
  surface-dim: "#111318"
  surface-bright: "#37393F"
  surface-container-lowest: "#0C0E13"
  surface-container-low: "#1A1B21"
  surface-container: "#1E2025"
  surface-container-high: "#282A2F"
  surface-container-highest: "#33353A"
  on-surface: "#E2E2E9"
  on-surface-variant: "#AAABB2"
  outline: "#5D5E64"
  outline-variant: "#2E3036"
  inverse-surface: "#E2E2E9"
  inverse-on-surface: "#2E3036"
  inverse-primary: "#B22B00"
  shadow: "#000000"
  scrim: "#000000"
```

## Typography

A three-role typographic system engineered for broadcast impact and rapid numerical scanning:

- **Headline (`Mulish`):** Bold geometric sans with tight tracking (`-0.5px`) for scoreboard-grade titles and hero statements.
- **Body (`Instrument Sans`):** Crisp neo-grotesque with open counters for effortless reading of match previews, analytical notes, and navigation.
- **Mono (`Spline Sans Mono`):** Tabular monospace for percentages, projections, uncertainty intervals, timestamps, and comparative stats.

Every numeric metric, score, and projection must apply `tabular-nums`.

```yaml
typography:
  display-lg:
    fontFamily: "Mulish"
    fontSize: 48px
    fontWeight: 800
    lineHeight: 52px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Mulish"
    fontSize: 32px
    fontWeight: 800
    lineHeight: 36px
    letterSpacing: -0.25px
  display-md:
    fontFamily: "Mulish"
    fontSize: 36px
    fontWeight: 800
    lineHeight: 42px
    letterSpacing: -0.5px
  display-md-mobile:
    fontFamily: "Mulish"
    fontSize: 28px
    fontWeight: 800
    lineHeight: 32px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: "Mulish"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 34px
    letterSpacing: -0.25px
  headline-md:
    fontFamily: "Mulish"
    fontSize: 22px
    fontWeight: 700
    lineHeight: 28px
    letterSpacing: -0.15px
  title-lg:
    fontFamily: "Instrument Sans"
    fontSize: 18px
    fontWeight: 700
    lineHeight: 24px
    letterSpacing: 0px
  title-md:
    fontFamily: "Instrument Sans"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 22px
    letterSpacing: 0px
  body-lg:
    fontFamily: "Instrument Sans"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
    letterSpacing: 0px
  body-md:
    fontFamily: "Instrument Sans"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
    letterSpacing: 0px
  label-lg:
    fontFamily: "Instrument Sans"
    fontSize: 13px
    fontWeight: 600
    lineHeight: 18px
    letterSpacing: 0.25px
  label-sm:
    fontFamily: "Instrument Sans"
    fontSize: 11px
    fontWeight: 600
    lineHeight: 16px
    letterSpacing: 0.5px
  mono-md:
    fontFamily: "Spline Sans Mono"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 18px
    letterSpacing: 0px
  mono-sm:
    fontFamily: "Spline Sans Mono"
    fontSize: 11px
    fontWeight: 500
    lineHeight: 14px
    letterSpacing: 0.25px
```

## Layout & Spacing

Desktop uses an asymmetric **12-column analytical shell** with a persistent `240px` left navigation rail and fluid main canvas (`max-w-[1440px]`), allowing wide match-comparison panels and bento-style featured cards. Mobile (`390px`) collapses into a single-column stream with a sticky top discipline bar and fixed bottom navigation dock.

A strict **4px / 8px spacing scale** governs all padding, grid gaps, and section rhythms. Siblings use `gap-*` rather than margins.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 48px
  page-margin: 24px
```

## Elevation & Depth

Hierarchy relies on **tonal surface layering** and **crisp 1px `outline-variant` (`#2E3036`) borders** rather than drop shadows. Photography heroes use directional dark scrims (`from-surface-container-lowest/95 via-surface-container-lowest/70 to-transparent`) so overlaid broadcast typography remains effortlessly legible.

## Shapes

Sharp, engineered corners with deliberate hierarchy: `rounded-md` (`12px`) for primary match and analytics cards, `rounded` (`8px`) for buttons and inputs, `rounded-sm` (`4px`) for data bars and telemetry tags, and `rounded-full` for live status pills and team/player avatars.

```yaml
rounded:
  sm: 4px
  DEFAULT: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Motion is crisp, mechanical, and purposeful. Hover states and tab switches respond in `120ms` (`ease-out`), while analytical panels enter over `240ms` with smooth deceleration. Only `transform`, `opacity`, and `color` animate.

```yaml
motion:
  state-change:
    duration: 120ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 240ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

- **Tone of Voice:** Direct, passionate yet rigorous, transparent. Speaks like a lead sports data journalist ("Proyección del modelo: 61.4% · Muestra: 18 partidos").
- **Capitalisation:** Sentence case for headings and body; uppercase reserved strictly for compact discipline/live micro-badges (`EN DIRECTO`, `NBA`, `VALORANT`).
- **Terminology:** Always use *Pronóstico*, *Proyección del modelo*, *Datos reales*, *Nivel de incertidumbre*. Never use betting-house terms (*cuotas*, *apuesta*, *stake*, *bankroll*).
- **Do's and Don'ts:**
  - **Do** separate verified historical stats from model projections with distinct visual badges and monospace telemetry.
  - **Don't** invent probabilities or present pending predictions as won/lost.
  - **Don't** use generic `bg-blue-*` or arbitrary hex values; use semantic tokens exclusively.

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Badge** → `@components/badge.html`: `badge-numeric`, `badge-dot`
- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Tabs** → `@components/tabs.html`: `tabs-horizontal`, `tabs-with-icon`
- **Typography** → `@components/typography.html`: `typography-display`, `typography-body`, `typography-label`
