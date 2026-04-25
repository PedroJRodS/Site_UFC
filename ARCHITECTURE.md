# ARCHITECTURE

## Stack Decision
- Runtime: static HTML document served via browser.
- Styling: Tailwind via CDN (`https://cdn.tailwindcss.com`) with inline `tailwind.config`.
- Fonts/Icons: Google Fonts + Material Symbols.
- JavaScript: vanilla JS for small interactions and form validation only.

## Project Structure
- `code.html`: composed page used for preview and delivery.
- `sections/`: section-level partials used as source modules.
  - `Header.html`
  - `Hero.html`
  - `Stats.html`
  - `Footer.html`
- `assets/images/`: local image assets used by hero and content sections.
- `DESIGN.md`: original visual guidance.
- `DESIGN_SYSTEM.md`: implementation-facing token and usage guide.
- `USABILITY.md`: UX heuristics and acceptance criteria.

## Composition Model
- Source of truth for major sections is `sections/`.
- `code.html` is the assembled output for deployment/testing.
- Update flow:
  1. Edit section partial in `sections/`.
  2. Replicate final markup into the equivalent block in `code.html`.
  3. Validate interactions and responsiveness.

## Naming Conventions
- Files: kebab-case (`hero-ufc-ai.jpg`, `researchers-team.jpg`).
- CSS variables: `--brand-*`.
- Utility helpers: semantic naming (`.neon-glow-hover`, `.btn-primary-neon`).

## Asset Policy
- Avoid fragile placeholder URLs in production sections.
- Prefer local optimized assets in `assets/images/`.
- Always set meaningful `alt` text and preserve visual fallback backgrounds.

## Quality Gates
- Visual consistency with dark + neon identity.
- No broken image links.
- Keyboard-focus visibility on interactive controls.
- Mobile-first rendering verified at 360px, 768px, and 1280px.
