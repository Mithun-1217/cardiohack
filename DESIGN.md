---
name: Clinical Precision
colors:
  surface: '#faf8ff'
  surface-dim: '#d9d9e2'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3fc'
  surface-container: '#ededf6'
  surface-container-high: '#e7e7f1'
  surface-container-highest: '#e1e2eb'
  on-surface: '#191b22'
  on-surface-variant: '#434653'
  inverse-surface: '#2e3037'
  inverse-on-surface: '#f0f0f9'
  outline: '#737784'
  outline-variant: '#c3c6d5'
  surface-tint: '#1d59c1'
  primary: '#003c90'
  on-primary: '#ffffff'
  primary-container: '#0f52ba'
  on-primary-container: '#bcceff'
  inverse-primary: '#b0c6ff'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#732900'
  on-tertiary: '#ffffff'
  tertiary-container: '#993900'
  on-tertiary-container: '#ffc0a7'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d9e2ff'
  primary-fixed-dim: '#b0c6ff'
  on-primary-fixed: '#001945'
  on-primary-fixed-variant: '#00419c'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdbcd'
  tertiary-fixed-dim: '#ffb596'
  on-tertiary-fixed: '#360f00'
  on-tertiary-fixed-variant: '#7d2d00'
  background: '#faf8ff'
  on-background: '#191b22'
  surface-variant: '#e1e2eb'
typography:
  headline-lg:
    fontFamily: Manrope
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 38px
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: -0.01em
  label-caps:
    fontFamily: Public Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base-unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 20px
  container-max: 1440px
---

## Brand & Style
The design system is engineered for high-stakes healthcare environments where clarity, speed of cognition, and trust are paramount. The brand personality is clinical, authoritative, and calm, designed to reduce cognitive load for practitioners managing complex patient data. 

The aesthetic follows a **Corporate / Modern** style with a focus on functional minimalism. It prioritizes information density without sacrificing legibility. Every visual element serves a functional purpose, utilizing whitespace not just for aesthetics, but as a critical separator for distinct data points. The interface evokes a sense of organized stability, ensuring users feel in control of the information presented.

## Colors
The palette is rooted in "Deep Clinical Blue" to establish immediate professional trust. The background uses a "Cool White" to reduce eye strain during long shifts. 

The status indicators—Stable (Green), Caution (Amber), and Alert (Red)—are calibrated for high accessibility and immediate recognition. These semantic colors are reserved exclusively for patient status and system health to prevent "alert fatigue." Neutrals are utilized for structural elements like borders and secondary text, ensuring the primary data remains the focal point.

## Typography
This design system utilizes a multi-font strategy to balance character with utility. **Manrope** is used for headlines to provide a modern, refined tone. **Inter** serves as the primary workhorse for body text and data grids due to its exceptional legibility at small sizes and tall x-height. **Public Sans** is employed for labels and metadata, providing an institutional, government-grade clarity.

For data-heavy views, tabular lining figures must be used to ensure columns of numbers align perfectly for quick scanning.

## Layout & Spacing
The system employs a **Fixed Grid** layout for desktop dashboards to ensure data visualization components remain in predictable locations, while transitioning to a fluid model for tablet viewing. A 12-column grid is the standard, with a 20px gutter to provide clear visual separation between data modules.

Spacing follows a strict 4px baseline shift. Internal card padding should be generous (24px) to prevent data clusters from feeling overwhelming, while list items utilize a tighter 8px vertical rhythm to maximize visible records.

## Elevation & Depth
The design system uses **Tonal Layers** and **Low-contrast Outlines** rather than heavy shadows to maintain a clean, clinical feel. Depth is communicated through subtle shifts in background saturation:
1.  **Level 0 (Base):** The main application background (#F8FAFC).
2.  **Level 1 (Cards):** Pure white surfaces with a 1px border (#E2E8F0).
3.  **Level 2 (Modals/Popovers):** Pure white with a soft, diffused 15% opacity blue-tinted shadow to indicate temporary interaction.

This approach ensures that the hierarchy is felt rather than seen, keeping the interface flat and efficient.

## Shapes
The shape language is **Soft**, utilizing a 4px (0.25rem) corner radius for most functional elements like buttons and input fields. Large containers and patient cards utilize an 8px (0.5rem) radius. 

This subtle rounding strikes a balance between the precision of "Sharp" edges and the friendliness of "Rounded" shapes, maintaining a professional medical instrument aesthetic without appearing cold or industrial.

## Components
- **Buttons:** High-contrast primary buttons in Deep Clinical Blue. Ghost buttons with 1px borders for secondary actions.
- **Patient Cards:** Structured with a dedicated header for vital signs. Uses a 1px interior divider to separate bio-data from clinical notes.
- **Data Displays:** Use "Sparklines" for historical trends within tables. Vital signs that are out of range should use the semantic status colors as a background "pill" for the value.
- **Navigation:** A persistent left-hand sidebar with icons and text labels. The active state is indicated by a 4px vertical bar in the primary color.
- **Input Fields:** Clear labels placed above the field. Error states must include both a red border and a descriptive icon for accessibility.
- **Chips/Badges:** Small, high-legibility badges for categorization (e.g., "In-Patient," "Post-Op"). Use subtle tinted backgrounds with darker text for maximum readability.