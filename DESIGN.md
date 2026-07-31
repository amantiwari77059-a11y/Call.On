---
name: Reliable Communication System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#0051d5'
  on-secondary: '#ffffff'
  secondary-container: '#316bf3'
  on-secondary-container: '#fefcff'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#002113'
  on-tertiary-container: '#009668'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#dbe1ff'
  secondary-fixed-dim: '#b4c5ff'
  on-secondary-fixed: '#00174b'
  on-secondary-fixed-variant: '#003ea8'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
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
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  call-number:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  container-max: 1200px
  gutter: 16px
---

## Brand & Style

This design system is engineered for a professional VoIP environment where clarity, reliability, and speed are paramount. The aesthetic follows a **Corporate / Modern** approach, prioritizing functional minimalism to reduce cognitive load during high-stakes communication.

The target audience consists of business professionals and remote teams who require an interface that feels stable and "always-on." The emotional response should be one of calm confidence—achieved through generous whitespace, a structured layout, and a palette that evokes trust and technical precision. The UI avoids unnecessary ornamentation, focusing instead on high-quality typography and clear interactive states.

## Colors

The palette is anchored by a deep Navy Primary (`#0F172A`), providing a sense of authority and groundedness. A vibrant Blue Secondary (`#2563EB`) is used for primary actions, signifying connectivity and digital intelligence. Emerald Green (`#10B981`) serves as the functional tertiary color, specifically reserved for "Call" actions, "Online" status indicators, and successful connection states.

The background uses a Crisp White (`#FFFFFF`) with subtle Slate Gray (`#F8FAFC`) surface washes to differentiate sections. This high-contrast pairing ensures that text remains legible under various lighting conditions, critical for mobile professional use.

## Typography

The typography strategy employs a dual-sans approach to balance character with utility. **Manrope** is used for headlines and numeric displays (dial pads, active call timers) due to its modern, balanced proportions and excellent digit legibility. **Inter** is utilized for all body copy and contact lists, providing a systematic, neutral feel that excels in data-dense environments.

For technical metadata, such as IP addresses or call quality metrics, **JetBrains Mono** provides a precise, monospaced alternative that suggests technical reliability. Scale is handled strictly: large display sizes are used for active call screens, while compact, high-legibility labels are used for call history and contact directories.

## Layout & Spacing

The design system utilizes a **8px soft grid** to maintain mathematical harmony across all components. Layouts should be fluid but contained within a maximum width of 1200px for desktop environments to prevent line lengths from becoming unreadable.

- **Mobile:** Uses a 4-column fluid grid with 16px side margins and 16px gutters.
- **Desktop:** Transition to a 12-column grid. Side margins expand to 40px or auto-center.
- **Vertical Rhythm:** Spacing between contact list items is fixed at 8px to maintain a high information density while remaining touch-friendly.

## Elevation & Depth

This system uses **Tonal Layers** and **Ambient Shadows** to define hierarchy. Depth is not used for decoration, but to indicate "modality"—such as an incoming call overlay or a dropdown menu.

- **Level 0 (Base):** White or light gray background.
- **Level 1 (Cards):** Subtle 1px border in `#E2E8F0` with no shadow. Used for list grouping.
- **Level 2 (Active Elements):** Soft, diffused shadow (0px 4px 12px rgba(15, 23, 42, 0.08)). Used for the dialer pad and floating action buttons.
- **Level 3 (Modals/Overlays):** Deep, wide shadow (0px 12px 32px rgba(15, 23, 42, 0.12)) to pull the active call screen to the front of the user's focus.

## Shapes

The shape language is consistently **Rounded**, using an 8px (`0.5rem`) base radius. This creates a contemporary, approachable feel without appearing overly playful or "bubbly."

- Standard buttons and input fields use `rounded` (8px).
- Avatars and high-level containers use `rounded-lg` (16px).
- Connectivity indicators and status badges use `rounded-full` (pill-shaped) to distinguish them from interactive buttons.

## Components

### Buttons
- **Primary:** Solid `#2563EB` with white text. Used for "Start Call" or "Save."
- **Success:** Solid `#10B981`. Used exclusively for "Accept Call."
- **Destructive:** Solid `#EF4444`. Used for "End Call" or "Decline."
- **Ghost:** Transparent background with `#64748B` text. Used for secondary settings.

### Input Fields
Inputs should have a 1px border in `#CBD5E1`. On focus, the border shifts to the primary blue with a 2px outer "glow" (shadow) of the same color at 10% opacity.

### Call Cards
Contact cards in the history view should feature a clear trailing icon indicating call direction (inbound/outbound/missed) using the system's semantic colors (Green for inbound, Red for missed).

### Dialer Pad
The dialer pad uses circular buttons with a light gray hover state. Large, centered numerals in Manrope are paired with smaller alphabetical sub-text to mimic traditional telephony for user familiarity.

### Status Indicators
Small, pill-shaped chips used to indicate "HD Audio," "VPN Connected," or "Recording." These should use low-saturation background tints of the primary colors to remain informative but non-distracting.