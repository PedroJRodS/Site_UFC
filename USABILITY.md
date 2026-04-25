# USABILITY

## Heuristics Adopted
- **Visibility of system status**: newsletter form shows immediate success/error feedback.
- **Consistency and standards**: shared hover/focus behavior across cards, buttons, and links.
- **Error prevention**: email validation before submit.
- **Recognition over recall**: CTA labels are explicit and action-oriented.
- **Aesthetic and minimalist design**: neon effects are controlled and only emphasized on hover/focus.

## Interaction States
- Buttons and cards:
  - Base: dark surface + soft border.
  - Hover: `duration-300` with neon glow and slight lift.
  - Active: subtle scale-down to communicate click.
  - Focus-visible: ring/outline with high contrast.
- Links:
  - Hover color change + optional slight translate only when not harming readability.

## Responsive Rules
- Breakpoints:
  - Mobile: `<768px`
  - Tablet: `>=768px`
  - Desktop: `>=1024px`
- Metrics grid:
  - Mobile: 2 columns.
  - Tablet/Desktop: 2 columns with increased spacing.
- Research cards:
  - Mobile: single-column stack.
  - Tablet: 2 columns.
  - Desktop: 4 columns.
- Hero typography:
  - Mobile: compact line breaks and reduced display size.
  - Desktop: large display scale.

## Newsletter UX
- Invalid email:
  - Red border, explicit helper text.
- Valid email submit:
  - Green confirmation message and non-blocking reset.
- Input must preserve focus visibility for keyboard users.

## QA Checklist
- Keyboard navigation visits nav links, CTAs, and form controls in logical order.
- Hover/focus states are visible on dark backgrounds.
- No horizontal scroll on mobile.
- Hero + metrics + research tracks remain readable at 360px width.
