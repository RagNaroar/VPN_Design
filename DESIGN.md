---
name: Cyber-Minimalist Design System
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#39393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1c1b1e'
  surface-container: '#201f22'
  surface-container-high: '#2a2a2d'
  surface-container-highest: '#353438'
  on-surface: '#e5e1e5'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e1e5'
  inverse-on-surface: '#313033'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ffb2b8'
  on-secondary: '#67001d'
  secondary-container: '#ff506e'
  on-secondary-container: '#5b0018'
  tertiary: '#faf3ff'
  on-tertiary: '#3c0090'
  tertiary-container: '#e1d2ff'
  on-tertiary-container: '#7213ff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#ffdadb'
  secondary-fixed-dim: '#ffb2b8'
  on-secondary-fixed: '#40000f'
  on-secondary-fixed-variant: '#91002d'
  tertiary-fixed: '#e9ddff'
  tertiary-fixed-dim: '#d1bcff'
  on-tertiary-fixed: '#23005b'
  on-tertiary-fixed-variant: '#5700c9'
  background: '#131316'
  on-background: '#e5e1e5'
  surface-variant: '#353438'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 40px
  container-max-width: 1200px
---

## Brand & Style

This design system embodies a "Cyber-Minimalist" aesthetic, merging the raw, functional power of terminal-based hacking tools with the refined sophistication of modern premium software. It is designed for high-performance privacy tools where security must feel both impenetrable and instantaneous.

The visual narrative is built on the contrast between the "Deepest Black" void of the background and the hyper-vibrant neon signals of the interface. It utilizes **Glassmorphism** to create a sense of multi-layered intelligence, suggesting a UI that floats over a complex stream of data. The emotional response is one of total control, advanced technical capability, and uncompromising digital safety.

## Colors

The palette is strictly dark-mode, designed to reduce ocular strain while emphasizing critical status indicators.

*   **Primary (Neon Cyan):** Used for "Active" states, secure connection status, and successful data flow. It represents safety and speed.
*   **Secondary (Electric Pink):** Reserved for "Breach" alerts, disconnect warnings, and high-priority system interruptions.
*   **Tertiary (Deep Purple):** Used for background accents, encryption process visualizations, and secondary navigation elements to provide depth without distracting from primary actions.
*   **Neutral (Deepest Black):** The foundation of the UI. All surfaces use this hex as a base, typically with varying levels of opacity to facilitate glass effects.

## Typography

This design system utilizes a dual-font strategy to balance legibility with a high-tech atmosphere.

*   **Inter** is used for primary UI headlines and navigation. Its clean, geometric sans-serif nature provides a modern, professional anchor to the design.
*   **JetBrains Mono** is used for all body text, status logs, and data readouts. The monospaced nature reinforces the "hacker" aesthetic and ensures that numerical data (like IP addresses and transfer speeds) remains perfectly aligned and legible.
*   **Case Usage:** Labels and technical metadata should frequently use all-caps with increased letter spacing to mimic machine-readable headers.

## Layout & Spacing

The layout follows a strict 12-column fluid grid system with technical, tight gutters. 

*   **Grid Model:** Content is housed in modular "Panels" that snap to the grid. 
*   **Spacing Rhythm:** All spacing must be a multiple of the 4px base unit. This ensures a mathematical precision consistent with the technical nature of the product.
*   **Responsiveness:** On mobile, the 12-column grid collapses to a single-column stack. Side margins increase on desktop to maintain a focused, "command center" feel in the middle of the screen. 
*   **Visual Density:** High-density information displays (like logs) should use 8px internal padding, while primary interaction areas (like the "Connect" button) should use generous 32px or 48px padding to stand out.

## Elevation & Depth

Depth in the design system is achieved through light and transparency rather than physical shadows.

1.  **Backdrop Blur:** All floating panels must use a 24px background blur. The surface color is a 40% to 60% opacity version of the Deepest Black.
2.  **Glowing Borders:** Instead of shadows, elevation is indicated by 1px solid borders. For active or elevated elements, these borders should have a subtle outer glow (box-shadow) using the Primary or Tertiary color with a 10px-20px spread and low opacity (20%).
3.  **Tonal Stacking:** Higher-level elements (like modals) should have a slightly lighter background opacity than the base panels to indicate they are closer to the user.

## Shapes

The shape language is "Soft-Precision." By using a minimal 4px radius (Level 1), the UI maintains a sharp, technical edge while avoiding the dated look of absolute 0px corners.

*   **Standard Elements:** Buttons, input fields, and panels use the base 4px radius.
*   **Interactive Controls:** Small toggles or checkboxes may use the base radius to maintain consistency.
*   **Exceptions:** Terminal windows or log streams should remain sharp (0px) to distinguish them as "raw" system outputs.

## Components

*   **Buttons:** Primary buttons use a solid Neon Cyan fill with black monospaced text. Secondary buttons use a ghost style with a 1px Cyan border and a subtle glow on hover.
*   **Live Terminal Logs:** A dedicated component for real-time status updates. It uses a black background (80% opacity), no border-radius, and JetBrains Mono green-tinted or cyan-tinted text.
*   **Scanning Effects:** When connecting, panels should display a horizontal "scan-line" animation—a 1px high Primary color gradient that moves vertically across the glass surface.
*   **Input Fields:** Inputs are styled as simple 1px bottom-borders (underline style) or fully outlined glass boxes. The cursor should be a solid, blinking block to mimic a terminal.
*   **Status Chips:** Small, capsules used for "Encrypted," "Protected," or "Kill-switch Active." These use a 1px border of the associated status color (Cyan/Pink) with a 10% opacity fill of that same color.
*   **Connection Toggle:** A large, prominent central component. It should feature a heavy glow effect when "ON," acting as the primary light source for the entire screen.