---
name: High-Signal Precision
colors:
  surface: '#101416'
  surface-dim: '#101416'
  surface-bright: '#363a3c'
  surface-container-lowest: '#0b0f10'
  surface-container-low: '#181c1e'
  surface-container: '#1c2022'
  surface-container-high: '#272b2c'
  surface-container-highest: '#313537'
  on-surface: '#e0e3e5'
  on-surface-variant: '#bbcac5'
  inverse-surface: '#e0e3e5'
  inverse-on-surface: '#2d3133'
  outline: '#869490'
  outline-variant: '#3c4946'
  surface-tint: '#57dbc8'
  primary: '#57dbc8'
  on-primary: '#003731'
  primary-container: '#26b8a6'
  on-primary-container: '#00433b'
  inverse-primary: '#006b5f'
  secondary: '#c4c7c9'
  on-secondary: '#2d3133'
  secondary-container: '#43474a'
  on-secondary-container: '#b2b5b8'
  tertiary: '#c4c7c9'
  on-tertiary: '#2d3133'
  tertiary-container: '#a2a5a7'
  on-tertiary-container: '#373b3d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#77f8e4'
  primary-fixed-dim: '#57dbc8'
  on-primary-fixed: '#00201c'
  on-primary-fixed-variant: '#005047'
  secondary-fixed: '#e0e3e5'
  secondary-fixed-dim: '#c4c7c9'
  on-secondary-fixed: '#181c1e'
  on-secondary-fixed-variant: '#43474a'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#181c1e'
  on-tertiary-fixed-variant: '#434749'
  background: '#101416'
  on-background: '#e0e3e5'
  surface-variant: '#313537'
typography:
  display:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  h1:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  h2:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0.01em
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.08em
  mono-data:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: -0.01em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin: 32px
---

## Brand & Style

This design system is engineered for high-stakes environments where information density and clarity are paramount. The brand personality is authoritative, technical, and stoic. It targets professional users in sectors like systems engineering, data science, and quantitative finance—environments where "noise" is a liability.

The aesthetic follows a **Minimalist-Systems** movement. It eschews decorative flourishes in favor of structural integrity and functional precision. The visual language is defined by strict alignment, monochromatic foundations with surgical use of color, and a "high-signal" approach to data visualization. Every element exists to serve a specific utility, evoking an emotional response of focused calm and absolute reliability.

## Colors

The palette is anchored in a deeply desaturated charcoal base to minimize eye strain during long-duration technical work. The primary accent, a desaturated teal, is used exclusively for primary actions, active states, and critical data points. 

Secondary surfaces are built through incremental tonal shifts rather than shadows, maintaining a flat, architectural feel. The border color (`#2A2E30`) is utilized for structural definition, ensuring that even in a dark environment, the hierarchy of containers remains distinct without relying on high-contrast dividers.

## Typography

Typography is used as a navigational tool. **Space Grotesk** provides a technical, geometric edge to headlines, reinforcing the systems-oriented nature of the design system. **Inter** is utilized for all functional and body text to ensure maximum legibility at small scales.

Weight is used sparingly; lean toward "Medium" for emphasis rather than "Bold" to maintain the refined, professional character. For data-heavy tables and status labels, use the `label-caps` or `mono-data` styles to distinguish system-generated metadata from user-generated content.

## Layout & Spacing

This design system utilizes a rigid 4px baseline grid to ensure mathematical precision across all layouts. Information should be organized into a 12-column fluid grid for dashboard-style interfaces, or a fixed-width 1200px container for documentation and settings views.

Spacing is tight to accommodate high information density. Internal component padding should default to `sm` (8px) or `md` (16px) to keep elements compact. Use `xl` (40px) only to separate major logical sections of an application. Alignment must be pixel-perfect; "optical" alignment should be secondary to structural grid adherence.

## Elevation & Depth

Depth is conveyed through **Tonal Layers** rather than shadows. In this dark-mode environment, "elevation" is simulated by lightening the background hex code.

1.  **Level 0 (Base):** `#101416` – The main application canvas.
2.  **Level 1 (Surface):** `#161B1D` – Cards, sidebars, and navigation rails.
3.  **Level 2 (Overlay):** `#1C2124` – Modals, dropdowns, and tooltips.

Use low-contrast outlines (`#2A2E30`) to define the boundaries of these surfaces. Avoid drop shadows entirely; if an overlay requires further separation from the background, use a 1px solid border in a slightly lighter charcoal (`#3A3F42`).

## Shapes

The shape language is "Soft-Mechanical." A 0.25rem (4px) corner radius is applied to buttons, inputs, and cards. This slight rounding prevents the UI from feeling aggressive while remaining significantly more professional and serious than "pill-shaped" or highly rounded consumer designs.

Icons should follow a 2px stroke weight with square caps and joins to match the precise, geometric nature of the Space Grotesk typeface.

## Components

### Buttons
- **Primary:** Background `#26B8A6`, Text `#101416` (High contrast). No border.
- **Secondary:** Transparent background, 1px Border `#2A2E30`, Text `#E0E3E5`.
- **Ghost:** Transparent background, Text `#E0E3E5`, subtle hover state using surface `#1C2124`.

### Input Fields
Inputs must use the `#0C0F10` background (darker than the base) to create an "etched" look. Use a 1px border of `#2A2E30`. The active state is signaled by a 1px border of `#26B8A6` and a subtle inner glow.

### Chips & Tags
Small, 20px height, using the `label-caps` typography. Backgrounds should be desaturated: use a 10% opacity teal for "Active" and `#2A2E30` for "Neutral."

### Data Lists
Lists are the core of this design system. Use 1px bottom borders (`#2A2E30`) to separate rows. Hover states should trigger a background shift to `#161B1D`. Ensure text alignment in tables follows technical standards: numbers are right-aligned, text is left-aligned.

### Cards
Cards are defined by their background (`#161B1D`) and a subtle border. No shadows. Use cards to group related data parameters, keeping the header of the card in the `h3` or `label-caps` style for clear sectioning.