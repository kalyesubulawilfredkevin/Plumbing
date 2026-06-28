---
name: Hydro-Aesthetic Premium
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#42474f'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#727780'
  outline-variant: '#c2c7d1'
  surface-tint: '#2d6197'
  primary: '#00355f'
  on-primary: '#ffffff'
  primary-container: '#0f4c81'
  on-primary-container: '#8ebdf9'
  inverse-primary: '#a0c9ff'
  secondary: '#00677d'
  on-secondary: '#ffffff'
  secondary-container: '#50d9fe'
  on-secondary-container: '#005c70'
  tertiary: '#572500'
  on-tertiary: '#ffffff'
  tertiary-container: '#7a3700'
  on-tertiary-container: '#ffa46c'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d2e4ff'
  primary-fixed-dim: '#a0c9ff'
  on-primary-fixed: '#001c37'
  on-primary-fixed-variant: '#07497d'
  secondary-fixed: '#b3ebff'
  secondary-fixed-dim: '#4cd6fb'
  on-secondary-fixed: '#001f27'
  on-secondary-fixed-variant: '#004e5f'
  tertiary-fixed: '#ffdbc8'
  tertiary-fixed-dim: '#ffb68b'
  on-tertiary-fixed: '#321200'
  on-tertiary-fixed-variant: '#753400'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  display-lg:
    fontFamily: Poppins
    fontSize: 56px
    fontWeight: '700'
    lineHeight: 64px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Poppins
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Poppins
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Poppins
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
  margin-mobile: 16px
  margin-desktop: 48px
  section-gap: 120px
---

## Brand & Style
The brand personality is authoritative yet approachable, merging the reliability of master craftsmanship with the sophistication of modern smart-home technology. This design system targets high-net-worth homeowners and luxury estate managers who value precision, cleanliness, and rapid, high-tech solutions.

The visual style is **Premium Glassmorphism**. It utilizes multi-layered depth, frosted translucency, and vibrant background blurs to evoke a sense of water, clarity, and flow. The aesthetic is "High-Tech Professional," utilizing soft lighting effects and floating elements to differentiate from traditional, "gritty" industrial service providers. The emotional response should be one of immediate relief and trust—conveying that the infrastructure of the home is in expert hands.

## Colors
The palette is rooted in deep aquatic tones, contrasted by high-energy accents.

- **Primary Deep Blue (#0F4C81):** Represents depth, stability, and professional water management. Used for primary branding and grounding elements.
- **Secondary Cyan (#00B4D8):** Represents clarity and movement. Used for glass highlights, gradients, and interactive states.
- **Accent Orange (#FF7A00):** Used sparingly for urgent Call-to-Actions (CTAs) and critical alerts, providing high-contrast visibility against blue backgrounds.
- **Surface Strategy:** The design system employs a light background (#F8FAFC) for standard information and deep dark sections (#0F172A) to signal premium service tiers or technical specifications. Glass panels should use a semi-transparent white (60-80% opacity) with a 16px-32px backdrop blur.

## Typography
The typographic hierarchy balances the geometric friendliness of **Poppins** for headings with the systematic legibility of **Inter** for functional text. 

Headlines should be set with tight letter-spacing to feel modern and "contained." Display sizes are reserved for hero sections and impact statements, while labels use slightly increased letter-spacing and a semi-bold weight to maintain professional clarity even at small sizes. Use the Primary Deep Blue for most headings to maintain authority, transitioning to white on dark or glass surfaces.

## Layout & Spacing
The layout follows a fluid 12-column grid system with generous vertical "breathing room" to maintain a premium feel. 

- **Desktop:** 12-column grid, 48px side margins, 24px gutters.
- **Mobile:** 4-column grid, 16px side margins.
- **Rhythm:** Elements are spaced in multiples of 8px. Large sections are separated by 120px of whitespace to ensure information is never crowded. 

Floating elements and glass panels should often overlap section boundaries slightly to create a sense of three-dimensional space and layered depth.

## Elevation & Depth
This design system relies heavily on **Glassmorphism** and **Ambient Shadows** to create a high-tech, tactile feel.

- **Level 1 (Base):** Flat surfaces or subtle 1px inner borders to define boundaries.
- **Level 2 (Cards):** 20% opacity white fill with 20px backdrop-blur, a 1px semi-transparent white border, and a soft shadow (0px 10px 30px rgba(15, 76, 129, 0.08)).
- **Level 3 (Floating):** Increased blur (40px) and a more pronounced shadow to indicate elements that are "closer" to the user, such as sticky navbars or active modals.

**3D Tilt Effect:** Service cards should implement a subtle CSS perspective tilt (max 5 degrees) on hover, following the cursor to emphasize the "high-tech" nature of the service.

## Shapes
A consistent **24px radius** (rounded-xl) is the standard for all primary UI components, including cards, input fields, and large buttons. This extreme roundedness removes "sharp edges" from the plumbing experience, suggesting safety and a premium, modern touch. 

- **Containers/Cards:** 24px.
- **Buttons/Inputs:** 16px (to maintain structural integrity at smaller heights).
- **Icons:** Should feature soft, rounded terminals and thick strokes (2px minimum) to match the UI weight.

## Components

### Sticky Glass Navbar
The navigation bar is a floating element with a `backdrop-filter: blur(20px)` and a background of `rgba(255, 255, 255, 0.7)`. It features a 1px bottom border in a light cyan tint.

### Premium Service Cards
Cards utilize the 3D tilt effect and glassmorphic styling. Icons within cards are housed in circular "water-drop" containers with a gradient from Secondary Cyan to Primary Blue.

### Modern Form Inputs
Inputs are defined by a light background (#F1F5F9) that transitions to white on focus. The focus state is marked by a 2px Secondary Cyan glow and a subtle elevation lift. Labels sit above the input in `label-md` styling.

### Buttons
- **Primary:** Solid Primary Deep Blue with a 10% Cyan glow on hover.
- **Secondary:** Transparent with a 2px Primary Deep Blue border.
- **Emergency CTA:** Accent Orange (#FF7A00) with a subtle "pulse" animation to draw immediate attention.

### 3D Floating Elements
Decorative 3D spheres or "water droplets" with frosted textures should be placed behind glass panels in the background to enhance the depth effect without distracting from the content.