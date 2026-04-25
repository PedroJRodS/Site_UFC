# DESIGN_SYSTEM

## Purpose
Implementation reference for the UFC AI landing page visual system, derived from `DESIGN.md` and adapted to the current dark & neon direction.

## Brand Core Palette
- `--brand-bg-deep`: `#0B1218`
- `--brand-surface`: `#121316`
- `--brand-neon-blue`: `#0074D9`
- `--brand-neon-blue-soft`: `#AFc8F0`
- `--brand-accent-orange`: `#FF7A1A`
- `--brand-text-high`: `#E3E2E5`
- `--brand-text-muted`: `#C4C6CF`

## Token Mapping (Tailwind Inline Config)
- `primary` -> `var(--brand-neon-blue)`
- `secondary-container` -> `var(--brand-neon-blue)`
- `tertiary` -> `var(--brand-accent-orange)`
- `surface` / `background` -> `var(--brand-surface)`
- `on-surface` -> `var(--brand-text-high)`
- `on-surface-variant` -> `var(--brand-text-muted)`

## Reserved Tokens
Tokens from the generated dense palette that are not currently used in visible UI stay reserved for future states:
- `*-fixed`, `*-fixed-dim`, and `on-*-fixed-*`
- `inverse-*`
- full error container pair (`error-container`, `on-error-container`) beyond form feedback

## Neon Interaction Rules
- Hover glow must remain subtle and readable.
- Recommended glow for primary actions:
  - Outer glow: `0 0 0 1px rgba(0, 116, 217, 0.35), 0 0 22px rgba(0, 116, 217, 0.28)`
- Recommended glow for accent actions:
  - Outer glow: `0 0 0 1px rgba(255, 122, 26, 0.35), 0 0 22px rgba(255, 122, 26, 0.24)`
- Default transition timing: `duration-300`.

## Typography
- Headings: Space Grotesk.
- Body and labels: Inter.
- Keep uppercase labels for navigation and CTA identifiers only.

## Contrast & Accessibility
- All CTA text must remain AA readable over dark backgrounds.
- Focus style must be visible in keyboard navigation without relying on color alone (outline or ring + color).
