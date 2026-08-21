---
name: Cyber Catalog System
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#c0c1ff'
  on-secondary: '#1000a9'
  secondary-container: '#3131c0'
  on-secondary-container: '#b0b2ff'
  tertiary: '#ffb786'
  on-tertiary: '#502400'
  tertiary-container: '#df7412'
  on-tertiary-container: '#461f00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffdcc6'
  tertiary-fixed-dim: '#ffb786'
  on-tertiary-fixed: '#311400'
  on-tertiary-fixed-variant: '#723600'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
  surface-charcoal: '#1e293b'
  surface-slate: '#334155'
  electric-cyan: '#06b6d4'
  error-red: '#ef4444'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.03em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
---

## Brand & Style

This design system is engineered for a premium electronic catalog experience, prioritizing high-tech sophistication and visual clarity. The aesthetic merges **Modern Minimalism** with **Glassmorphism**, creating a futuristic environment where hardware feels tactile and digital interfaces feel atmospheric.

The experience is centered around a "Dark Mode First" philosophy. It avoids the clutter of traditional retail by utilizing expansive whitespace (or "darkspace"), precise geometric alignments, and subtle motion. The goal is to evoke a sense of high-end engineering and reliability, moving away from the loud, discount-driven visuals of standard electronics stores toward an editorial, boutique tech experience.

## Colors

The palette is anchored in a deep "Midnight" foundation (`#0f172a`), providing a high-contrast backdrop that allows product photography to pop. 

- **Primary Accent:** Electric Blue (`#3b82f6`) is used exclusively for interactive states, primary actions, and critical indicators.
- **Surface Strategy:** We use a hierarchy of grays to define depth. The base is `#0f172a`, while cards and containers utilize `#1e293b`. 
- **Glassmorphism:** Overlays and navigation bars use semi-transparent variants of the surface colors with background blurs to maintain a sense of environmental depth.
- **Accents:** Use the secondary Indigo and Cyan sparingly for categorization or technical specifications to reinforce the "high-tech" narrative.

## Typography

This design system utilizes **Inter** for its entire scale to ensure maximum legibility and a systematic, technical feel. 

- **Weight Usage:** Use "Extra Bold" (800) for display titles to create a strong visual anchor. "Semi Bold" (600) is reserved for product titles and primary UI labels.
- **Technical Styling:** For technical specifications and data points, use `label-md` with uppercase styling and increased letter spacing to emulate the look of precision instruments.
- **Scale:** On mobile devices, display and large headlines should scale down by 15-20% to maintain comfortable reading densities while preserving the hierarchy.

## Layout & Spacing

The system employs a **Fluid Grid** model built on an 8px base unit. 

- **Grid:** A 12-column grid is used for desktop layouts. Product galleries should use a flexible 3 or 4-column span depending on the product's visual complexity.
- **Margins:** High-impact "generous" margins are used on desktop (`64px`) to reinforce the premium minimalist feel. On mobile, this tightens to `20px` to maximize screen real estate for product imagery.
- **Navigation:** The navigation bar is fixed to the top, utilizing a `backdrop-filter: blur(12px)` to allow content to scroll underneath it, maintaining the glassmorphic aesthetic.

## Elevation & Depth

Depth is communicated through **Tonal Layers** and **Glassmorphism** rather than traditional heavy drop shadows.

- **Level 0 (Background):** The deepest layer, `#0f172a`.
- **Level 1 (Cards/Surface):** Elevated surfaces use `#1e293b` with a subtle 1px border of `rgba(255, 255, 255, 0.1)` to define edges without adding visual weight.
- **Level 2 (Active/Hover):** When an element is interacted with, use a subtle "Electric Blue" outer glow (`box-shadow: 0 0 20px rgba(59, 130, 246, 0.2)`) and increase the border opacity.
- **Overlays:** Modals and tooltips utilize a frosted glass effect (60% opacity surface with 16px blur) to maintain the user's context of the catalog behind the element.

## Shapes

The shape language is "Refined Geometric." We use a consistent `0.5rem` (8px) radius for most UI components (cards, buttons, inputs) to strike a balance between friendly modernism and technical precision.

- **Standard Elements:** `rounded` (8px) for primary containers.
- **Small Elements:** `rounded-sm` (4px) for tags and small indicators.
- **Interactive Triggers:** Full "Pill" shapes are reserved for specific floating action buttons or status indicators (e.g., "In Stock").

## Components

### Buttons
- **Primary:** Solid Electric Blue (`#3b82f6`) with white text. Hover state includes a subtle brightness increase and a soft blue glow.
- **Secondary:** Ghost style with a 1px slate border and transparent background. Fill on hover.

### Product Cards
- **Sleek Aesthetic:** No visible borders by default; use the Level 1 surface color. On hover, the card should scale slightly (1.02x) and reveal a thin Electric Blue bottom border.
- **Imagery:** Product images must have background removal to blend seamlessly into the dark UI or sit on a very subtle radial gradient.

### Input Fields
- Dark backgrounds (`#0f172a`) with a slate border. The border transitions to Electric Blue on focus. Labels should use the `label-sm` technical style.

### Glass Navigation
- A fixed header with `background: rgba(15, 23, 42, 0.8)` and `backdrop-filter: blur(10px)`. Include a single-pixel bottom divider in a slightly lighter slate.

### Chips & Tags
- Used for categories (e.g., "5G", "OLED"). Use low-saturation backgrounds (slate) with high-contrast text to keep them secondary to the main CTA.