---
name: Artisanal Forge & Groom
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#d2c4b5'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#9b8f81'
  outline-variant: '#4e4539'
  surface-tint: '#ebc07e'
  primary: '#ebc07e'
  on-primary: '#432c00'
  primary-container: '#c59d5f'
  on-primary-container: '#4f3400'
  inverse-primary: '#795921'
  secondary: '#c4c6d0'
  on-secondary: '#2d3038'
  secondary-container: '#464951'
  on-secondary-container: '#b6b8c1'
  tertiary: '#e5c187'
  on-tertiary: '#422c01'
  tertiary-container: '#c09f68'
  on-tertiary-container: '#4d3608'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffddae'
  primary-fixed-dim: '#ebc07e'
  on-primary-fixed: '#281800'
  on-primary-fixed-variant: '#5e410b'
  secondary-fixed: '#e0e2ec'
  secondary-fixed-dim: '#c4c6d0'
  on-secondary-fixed: '#191c22'
  on-secondary-fixed-variant: '#44474e'
  tertiary-fixed: '#ffdeaa'
  tertiary-fixed-dim: '#e5c187'
  on-tertiary-fixed: '#271900'
  on-tertiary-fixed-variant: '#5b4314'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Playfair Display
    fontSize: 34px
    fontWeight: '600'
    lineHeight: 42px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 36px
    fontWeight: '600'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  headline-sm:
    fontFamily: Playfair Display
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 28px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.06em
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.08em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 10px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-mobile: 1rem
  margin: 3rem
  margin-mobile: 1.25rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system establishes a refined masculine atmosphere combining old-world craftsmanship with industrial precision. Designed for an artisanal grooming parlor in Kota Batu, it blends dark luxury with mechanical authenticity. The experience balances warmth and authority: the raw confidence of blackened steel and slate offset by the radiant glow of burnished bronze.

The aesthetic philosophy draws heavily from modern industrial minimalism intersected with tactile luxury. Surfaces feel dense, weighted, and engineered. Interfaces use deep, unpolluted dark tones to create an intimate studio-floor ambience, accented with fine hair-thin metallic lines and controlled frosted-glass surfaces that mimic backlit amber glass bottles and brushed brass hardware.

## Colors

The color palette captures the raw materiality of an upscale grooming workshop:

- **Primary Accent (`#C59D5F`):** A warm, radiant metallic bronze/gold used for key interactive moments, booking highlights, active selections, and focal iconography.
- **Secondary Surface (`#1C1F26`):** Dark slate infused with a cool cast iron undertone, serving as cards, elevated sheets, and drawer backdrops.
- **Tertiary Accent (`#8A6D3B`):** Deep burnished bronze for hover states, subtle golden borders, inactive step counters, and atmospheric gradients.
- **Base Canvas (`#121212`):** Deep charcoal black providing a heavy, light-absorbing ground plane that allows typography and bronze finishes to stand forward.

Text hierarchy relies strictly on pure white (`#FFFFFF`) for primary titles, monetary values, and active actions, paired with muted graphite gray (`#A0AAB2`) for timestamps, secondary descriptions, metadata, and service descriptions.

## Typography

The pairing creates intentional friction between the editorial grandeur of `Playfair Display` and the architectural clarity of `Plus Jakarta Sans`.

- **Headlines (`Playfair Display`):** Evoke vintage apothecary labels, luxury grooming journals, and heritage craftsmanship. Display titles must maintain tight line heights and negative letter-tracking to appear anchored and deliberate.
- **Body & Numerical Information (`Plus Jakarta Sans`):** Ensures flawless legibility for booking calendars, barber schedules, and pricing matrices. 
- **Labels & Micro-copy:** Rendered with elevated letter-spacing (`0.06em` to `0.1em`) and set in uppercase when designating statuses, barber specialties, or service category headers.

## Layout & Spacing

The layout operates on a disciplined 12-column grid system for desktop and tablet views, reflowing to a 4-column system for mobile viewports. Generous negative space balances the density of the deep charcoal background, allowing each service module and imagery panel to command focus.

- **Desktop (>= 1024px):** 12 columns, 48px canvas margin, 24px gutters. Master layouts emphasize asymmetrical sidebars for appointments and broad columns for portfolio visual curation.
- **Tablet (768px - 1023px):** 8 columns, 32px canvas margin, 20px gutters. Dual-pane scheduling transitions into collapsible stack views.
- **Mobile (< 768px):** 4 columns, 20px canvas margin, 16px gutters. Structural dividers become razor-thin horizontal rules (`1px solid rgba(197, 157, 95, 0.15)`).

## Elevation & Depth

Depth does not rely on heavy drop shadows; rather, it uses metallic edge light, subtle tonal shifts, and optical glass overlays to build industrial sophistication.

- **Base Layer:** Pure background (`#121212`).
- **Surface Elevation 1 (Card & Module Tier):** `#1C1F26` with a micro-border of `1px solid rgba(197, 157, 95, 0.18)`.
- **Surface Elevation 2 (Floating Modals, Time Pickers, Sheets):** Semi-opaque dark slate (`rgba(28, 31, 38, 0.85)`) layered over a `16px` backdrop-filter blur. Borders shift to a refined dual tone: `1px solid rgba(197, 157, 95, 0.35)` on top and left, grounding the component with industrial beveling.
- **Active / Elevated Hover:** A localized radial glow of warm bronze (`rgba(197, 157, 95, 0.12)`) emitting from behind the card or trigger, eliminating the need for conventional diffuse drop shadows.

## Shapes

To mirror tailored tailoring and machined steel tools, the interface employs tight, restrained radii (`roundedness: 1`). 

- Default interactive elements (buttons, inputs, cards) use an architectural `4px` (`0.25rem`) radius.
- Larger sheet containers and featured booking modules utilize `8px` (`0.5rem`).
- Strict pill shapes are reserved solely for live service statuses (e.g., "Available Today" or "In Chair").
- Dividers between sections mimic industrial cold-rolled steel: 1px continuous lines with subtle metallic stops.

## Components

### Buttons
- **Primary Action (Book Appointment, Confirm):** Filled with solid Warm Bronze (`#C59D5F`), charcoal text (`#121212`) set in `Plus Jakarta Sans` semi-bold, uppercase with subtle letter-spacing. On hover, background shifts to `#D6AF72` with a subtle `0 0 16px rgba(197, 157, 95, 0.25)` ambient glow.
- **Secondary Action (View Portfolio, Details):** Transparent fill with a `1px solid #C59D5F` boundary and white text. Hover transitions to `background: rgba(197, 157, 95, 0.1)`.
- **Ghost/Tertiary:** Pure text button in `#A0AAB2` transitioning to `#FFFFFF` on hover, paired with an inline bronze arrow icon.

### Cards & Service Tiles
- Structured using `#1C1F26` with a `1px` border of `rgba(197, 157, 95, 0.15)`.
- Padding scales at `space-lg` (`1.5rem`).
- Service pricing displays in `Playfair Display` in Warm Bronze, paired with muted duration metadata in `Plus Jakarta Sans`.

### Chips & Barber Badges
- Compact rectangular profiles with `4px` corner radii.
- Inactive chips feature dark charcoal surfaces with muted gray text (`#A0AAB2`).
- Active chips receive an inward glow via `1px solid #C59D5F` border and subtle gold-tinted fill (`rgba(197, 157, 95, 0.08)`).

### Form Inputs & Date/Time Pickers
- Input fields use an inset industrial styling: background `#15181E`, bordered by `1px solid rgba(160, 170, 178, 0.2)`.
- Active focus state: border immediately sharpens to `#C59D5F`, accompanied by a delicate outer halo of `rgba(197, 157, 95, 0.15)`.
- Placeholder text in `#A0AAB2` at 50% opacity.

### Checkboxes & Selection Controls
- Precision square boxes (`18px × 18px`) with `2px` corner radii.
- Unchecked: bordered in `rgba(160, 170, 178, 0.4)` over a dark foundation.
- Checked: filled with solid Warm Bronze (`#C59D5F`) bearing an engraved dark checkmark icon.

### Dividers & Section Anchors
- 1px industrial rules with gradient fades: `linear-gradient(90deg, transparent, rgba(197, 157, 95, 0.3) 50%, transparent)`.