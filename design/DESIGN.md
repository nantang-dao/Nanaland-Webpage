---
name: Neo-Natural Tech
colors:
  surface: '#fcf8ff'
  surface-dim: '#dad7f3'
  surface-bright: '#fcf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f2ff'
  surface-container: '#efecff'
  surface-container-high: '#e8e5ff'
  surface-container-highest: '#e2e0fc'
  on-surface: '#1a1a2e'
  on-surface-variant: '#594139'
  inverse-surface: '#2f2e43'
  inverse-on-surface: '#f2efff'
  outline: '#8d7168'
  outline-variant: '#e1bfb5'
  surface-tint: '#ab3500'
  primary: '#ab3500'
  on-primary: '#ffffff'
  primary-container: '#ff6b35'
  on-primary-container: '#5f1900'
  inverse-primary: '#ffb59d'
  secondary: '#006b5c'
  on-secondary: '#ffffff'
  secondary-container: '#65fade'
  on-secondary-container: '#007262'
  tertiary: '#00677e'
  on-tertiary: '#ffffff'
  tertiary-container: '#00a7cb'
  on-tertiary-container: '#003744'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbd0'
  primary-fixed-dim: '#ffb59d'
  on-primary-fixed: '#390c00'
  on-primary-fixed-variant: '#832600'
  secondary-fixed: '#65fade'
  secondary-fixed-dim: '#41ddc2'
  on-secondary-fixed: '#00201b'
  on-secondary-fixed-variant: '#005045'
  tertiary-fixed: '#b5ebff'
  tertiary-fixed-dim: '#59d5fb'
  on-tertiary-fixed: '#001f28'
  on-tertiary-fixed-variant: '#004e60'
  background: '#fcf8ff'
  on-background: '#1a1a2e'
  surface-variant: '#e2e0fc'
  bg-soft-orange: '#FFF3EF'
  bg-soft-green: '#E6FAF5'
  text-muted: '#5B5B6C'
  accent-gradient-start: '#FF6B35'
  accent-gradient-end: '#FF8C69'
typography:
  headline-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: '700'
    lineHeight: '1.3'
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
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
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  headline-xl-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  section-gap: 120px
  unit: 4px
---

## Brand & Style

This design system embodies the "Bright Neo-Natural Tech" aesthetic, specifically tailored for the **nanaland developer community**. It balances the organic warmth of community-driven rural construction with the precision of blockchain technology. The UI is designed to evoke a sense of optimism, clarity, and fluid digital collaboration.

The style is a hybrid of **Glassmorphism** and **Minimalism**, prioritizing airy layouts and depth through translucent layers rather than rigid borders. It avoids "card stacking" in favor of spacious, flowing arrangements that highlight the ecosystem's integration.

**Key visual principles:**
- **Fluidity:** Use of non-linear transitions and asymmetrical layouts to move away from traditional corporate grids.
- **Transparency:** Extensive use of backdrop blurs to suggest a "window" into the digital landscape.
- **Vibrancy:** High-energy accents against soft, organic background gradients.

## Colors

The palette is anchored by "Vitality Orange" (Primary) and "Trust Green" (Secondary), representing the energy of the community and the reliability of the technology, respectively. 

The background is a **dynamic linear gradient** flowing from Top-Left (`#FFF3EF`) to Bottom-Right (`#E6FAF5`), creating a "natural light" effect. Surfaces should primarily be pure white or semi-transparent glass.

**Usage Guidelines:**
- **Vitality Orange:** Reserved for primary CTAs, active status indicators in SEMI, and the "warm" side of UI animations.
- **Trust Green:** Used for success states, "bai" system primary actions, and secondary identifiers.
- **Deep Navy (#1A1A2E):** The primary text color, ensuring high legibility against the light background.
- **Glass Surfaces:** `rgba(255, 255, 255, 0.7)` with a `blur(20px)` for panels and navigation.

## Typography

The system uses **Plus Jakarta Sans** for headlines to provide a modern, friendly, and geometric feel. **Inter** is used for all functional body and label text to maintain a systematic, neutral clarity, especially for complex task-based information in the "bai" system.

**Implementation Rules:**
- **Bilingual Strategy:** The design system must maintain identical visual weighting for Chinese and English. Use `HarmonyOS Sans` or `PingFang SC` for Chinese text to match the optical weight of Inter.
- **Leading:** Generous line heights (1.6 for body) are mandatory to support the "spacious" brand personality.
- **Hierarchy:** Use font weight rather than color alone to distinguish between primary headers and secondary descriptions.

## Layout & Spacing

The layout is built on a **12-column fluid grid** for the main site, but transitions into a **Fluid Non-Grid** model for product detail pages.

**Form Factor Rules:**
- **Desktop:** Features an asymmetrical layout where content blocks overlap or drift slightly off-center to create a sense of motion.
- **Horizontal Sequence:** Main pages (Home, Overview, About, Join) are arranged as a continuous horizontal strip. Transitions are triggered via `translateX`.
- **Mobile:** Elements reflow to a vertical stack. The "Product Detail" phone mockups scale down but remain the focal point, with interaction buttons moving to a bottom-docked carousel or grid.

**Breakpoints:**
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## Elevation & Depth

This system uses **Diffuse Color Shadows** to create a light, energetic feel that avoids the "heavy" look of traditional drop shadows.

- **Standard Elevation:** No shadow, only 1px semi-transparent borders (`rgba(255,255,255,0.3)`).
- **Floating Panels/Cards:** `0 8px 24px rgba(255,107,53,0.12)`. The shadow color should match the context (Orange for SEMI, Green for bai).
- **Active/Hover State:** The shadow expands to `0 12px 32px rgba(255,107,53,0.18)` and the element scales slightly (1.02x).
- **Backdrop Blur:** Navigation and overlays must use `backdrop-filter: blur(20px)` with a light tint of the background color to maintain context.

## Shapes

The shape language is defined by **High Circularity**. Rounded corners are used to soften the "tech" aspect and emphasize the "natural" aspect of the community.

- **Primary Cards:** 24px corner radius.
- **Main CTAs / Buttons:** 12px (rounded-lg) for a modern, tactile feel.
- **Outer Containers:** 32px (rounded-xl) to create distinct "zones" of content.
- **Mobile Frames:** The mockups should use a 40px radius to mimic flagship smartphone industrial design.

## Components

### Buttons
- **Primary:** Gradient fill (`#FF6B35` to `#FF8C69`), 12px rounded corners. White text. `cubic-bezier(0.2, 0.8, 0.2, 1)` for all states.
- **Secondary:** Transparent background with a 1.5px gradient border. 
- **Floating Interaction (Product Detail):** Circular or capsule-shaped buttons. When active, they scale to 1.5x and fill with their respective theme color.

### Cards
- **Glass Card:** 24px radius, `rgba(255, 255, 255, 0.8)` background, backdrop blur. Avoid heavy borders; use subtle shadows for definition.

### Navigation Bar
- **Dynamic State:** Starts transparent. At `scroll > 80px`, it transitions to `rgba(255,255,255,0.85)` with a blur. 
- **Language Toggle:** A simple "中/EN" switch in the top-right. Transitioning language must trigger a global state refresh without page reload.

### Simulation Mockups (Mobile)
- Used in product details. These are not static images but "living" UI containers. 
- Skins must be derived from provided SEMI/bai screenshots but use "NANA" placeholder data.
- Animation must be synchronized with the external "Function Buttons" using the defined easing.

### Inputs & Forms
- **Soft Inputs:** 12px rounded corners, light gray background (`#F9F9FC`). On focus, the border transitions to Primary Orange with a soft glow.