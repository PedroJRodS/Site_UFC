---
name: UFC AI Design System
colors:
  surface: '#121316'
  surface-dim: '#121316'
  surface-bright: '#38393c'
  surface-container-lowest: '#0d0e11'
  surface-container-low: '#1a1c1e'
  surface-container: '#1f2022'
  surface-container-high: '#292a2c'
  surface-container-highest: '#343537'
  on-surface: '#e3e2e5'
  on-surface-variant: '#c4c6cf'
  inverse-surface: '#e3e2e5'
  inverse-on-surface: '#2f3033'
  outline: '#8e9198'
  outline-variant: '#43474e'
  surface-tint: '#afc8f0'
  primary: '#afc8f0'
  on-primary: '#163152'
  primary-container: '#001f3f'
  on-primary-container: '#6f88ad'
  inverse-primary: '#476083'
  secondary: '#a7c8ff'
  on-secondary: '#003060'
  secondary-container: '#0174d9'
  on-secondary-container: '#fefcff'
  tertiary: '#fdb69a'
  on-tertiary: '#4f2411'
  tertiary-container: '#391303'
  on-tertiary-container: '#b5785f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d4e3ff'
  primary-fixed-dim: '#afc8f0'
  on-primary-fixed: '#001c3a'
  on-primary-fixed-variant: '#2f486a'
  secondary-fixed: '#d5e3ff'
  secondary-fixed-dim: '#a7c8ff'
  on-secondary-fixed: '#001b3b'
  on-secondary-fixed-variant: '#004788'
  tertiary-fixed: '#ffdbce'
  tertiary-fixed-dim: '#fdb69a'
  on-tertiary-fixed: '#351002'
  on-tertiary-fixed-variant: '#6b3a25'
  background: '#121316'
  on-background: '#e3e2e5'
  surface-variant: '#343537'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1440px
  gutter: 24px
  margin: 40px
---

## Brand & Style

This design system establishes a visual language that bridges the storied institutional prestige of the Universidade Federal do Ceará with the cutting-edge frontier of Artificial Intelligence. The brand personality is **Authoritative**, **Visionary**, and **Precise**. It aims to evoke a sense of "Techno-Academic Excellence"—the feeling of being in a world-class laboratory where heritage meets the future.

The aesthetic leans heavily into **Sophisticated Minimalism** combined with **Glassmorphism**. By using translucent layers and high-fidelity textures, the UI creates a sense of depth and data transparency. The inclusion of subtle data visualization patterns (such as node-link structures or abstract wave-forms) as background elements reinforces the AI and technological focus without cluttering the interface.

## Colors

The palette is anchored by **Deep Navy (#001F3F)**, providing the institutional "gravity" and serving as the primary surface color in this dark-themed system. **Tech Blue (#0074D9)** acts as the secondary driver, used for primary actions and structural highlights.

**Electric Cyan** is reserved for high-energy AI states, data highlights, and "active" technology indicators. **Gold** is used sparingly as a prestigious accent to denote academic excellence, official certifications, or high-level milestones. The background utilizes a near-black **Neutral Base (#0B1218)** to provide maximum contrast for glass effects and vibrant cyan glow states.

## Typography

This design system utilizes **Space Grotesk** for headlines to inject a technical, geometric edge that suggests innovation and scientific inquiry. For body copy and functional labels, **Inter** is used for its exceptional readability and neutral, professional character.

The typographic hierarchy is generous, with large display sizes for key metrics and AI insights. Letter spacing is slightly tightened on headlines for a more "designed" look and widened on small labels to ensure legibility on dark, translucent backgrounds.

## Layout & Spacing

The layout follows a **12-column fixed grid** within a centralized container for desktop views, ensuring that academic content remains focused and readable. A strict **8px spacing scale** governs all margins and padding to maintain mathematical harmony.

Information is organized into "Modules." These modules use expansive whitespace (margins of 40px+) to separate high-level concepts, while internal component spacing is kept tight to imply precision. Layouts should prioritize a "Dashboard" feel, where data visualizations and text live in balanced proximity.

## Elevation & Depth

Depth is achieved through **Glassmorphism** rather than traditional shadows. Surfaces are defined by:
1.  **Backdrop Blur:** A 12px to 20px Gaussian blur on background layers.
2.  **Translucency:** 60-80% opacity on Deep Navy surfaces.
3.  **Inner Strokes:** 1px "Light Leak" borders (white or cyan at 10-15% opacity) on the top and left edges of components to simulate light hitting glass.
4.  **Outer Glows:** Instead of drop shadows, "Active" elements emit a subtle Electric Cyan outer glow (blur: 15px, opacity: 20%) to indicate AI-driven interactivity.

## Shapes

The shape language is **Soft (0.25rem / 4px base)**. This slight rounding removes the harshness of brutalism while maintaining the rigid, structural integrity required for an academic institution. 

Larger containers (Cards) may use `rounded-lg` (8px), but buttons and input fields stay sharp at 4px. This "Micro-rounding" communicates technical precision—like machined hardware—rather than the "bubbly" friendliness of consumer apps.

## Components

### Buttons
Primary buttons use a **Solid Tech Blue** fill with white text. Secondary buttons are "Ghost" style with a 1px Electric Cyan border and a backdrop blur. The "AI Insight" button variant uses a subtle Gold gradient border.

### Cards
Cards are the primary container for academic data. They must feature a frosted glass effect (Backdrop Filter) and a 1px border. Header areas within cards should be separated by a subtle 1px divider.

### Input Fields
Inputs are dark-themed with a Deep Navy background and a Tech Blue bottom-border. On focus, the border transitions to Electric Cyan with a soft glow effect.

### Data Visualization Patterns
Subtle background patterns—such as a faint dot grid or light-weight vector lines connecting "nodes"—should be used within the background of cards to denote sections where AI analysis is occurring.

### Chips & Tags
Used for research categories or AI confidence scores. These are small, pill-shaped elements with low-opacity fills (10% Cyan or 10% Gold) and high-contrast text.

### Additional Components
- **AI Progress Stepper:** A linear indicator using a cyan pulse animation.
- **Academic Breadcrumbs:** Minimalist text links using Gold for the current page to maintain institutional hierarchy.