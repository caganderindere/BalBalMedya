---
name: Cinematic Prestige
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#d1c5b4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#9a8f80'
  outline-variant: '#4e4639'
  surface-tint: '#e9c179'
  primary: '#e9c179'
  on-primary: '#412d00'
  primary-container: '#b99552'
  on-primary-container: '#442f00'
  inverse-primary: '#77591c'
  secondary: '#e3c288'
  on-secondary: '#412d01'
  secondary-container: '#5c4517'
  on-secondary-container: '#d4b47b'
  tertiary: '#b0c7f6'
  on-tertiary: '#173057'
  tertiary-container: '#849bc8'
  on-tertiary-container: '#193259'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdea6'
  primary-fixed-dim: '#e9c179'
  on-primary-fixed: '#271900'
  on-primary-fixed-variant: '#5d4204'
  secondary-fixed: '#ffdea5'
  secondary-fixed-dim: '#e3c288'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5a4315'
  tertiary-fixed: '#d7e3ff'
  tertiary-fixed-dim: '#b0c7f6'
  on-tertiary-fixed: '#001b3f'
  on-tertiary-fixed-variant: '#2f476f'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
  warm-ivory: '#F1EBDD'
  obsidian-light: '#121212'
typography:
  display-lg:
    fontFamily: EB Garamond
    fontSize: 72px
    fontWeight: '500'
    lineHeight: 80px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: EB Garamond
    fontSize: 48px
    fontWeight: '500'
    lineHeight: 56px
  headline-lg-mobile:
    fontFamily: EB Garamond
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  headline-md:
    fontFamily: EB Garamond
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
    letterSpacing: 0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.1em
spacing:
  unit: 8px
  gutter: 24px
  margin-desktop: 80px
  margin-mobile: 20px
  max-width: 1440px
---

## Brand & Style
The design system is rooted in the intersection of historical prestige and future-facing strategy. The brand personality is authoritative yet understated, evoking the feeling of a high-end film production house or a cultural heritage institution. 

The aesthetic follows a **Minimalist-Cinematic** movement. It prioritizes extreme negative space to allow content to breathe, high-contrast color relationships to establish hierarchy, and thin, precision-engineered gold accents to signify luxury. A subtle film grain texture should be applied to large "Obsidian" surfaces to avoid digital flatness and add a tactile, celluloid quality to the interface.

## Colors
The palette is dominated by **Obsidian Black (#050505)**, serving as the canvas for all experiences to create a "theatrical" environment. 

**Luxury Gold (#B99552)** is used sparingly for interactive primary elements and significant highlights. **Muted Gold (#8E7340)** serves as a secondary accent for borders and less critical metadata. **Warm Ivory (#F1EBDD)** is reserved exclusively for high-readability body text and "Paper" style surfaces where dark text is required. Avoid using pure white; the ivory maintains the organic, archival feel of the brand.

## Typography
Typography is the primary vehicle for the brand’s "Heritage meets Future" narrative. 

- **Headlines (EB Garamond):** Used for all major titles. The serif structure provides a classic, literary feel. Use tight letter-spacing for large display sizes to maintain a sophisticated, editorial look.
- **Body & Labels (Inter):** Used for all functional text, navigation, and long-form reading. Inter’s clinical precision contrasts against the serif headings, representing the brand's strategic and technological edge.
- **Label-Caps:** This style is essential for "Overlines" and small metadata, providing a structured, modern architectural feel.

## Layout & Spacing
The layout utilizes a **Fixed Grid** model on desktop to maintain "Theatrical Framing." Content is centered within a 1440px container with generous 80px margins. 

The spacing rhythm is intentional and sparse. Use vertical spacing (margins between sections) that is 1.5x larger than typical SaaS products to emphasize the "Luxury" and "Cinematic" nature of the content. On mobile, transition to a 4-column fluid grid, but maintain 20px safe-area margins to ensure text does not feel cramped.

## Elevation & Depth
Depth is created through **Tonal Layering** rather than traditional drop shadows. 

1. **Base:** Obsidian Black (#050505) with a 2% opacity film grain overlay.
2. **Surface:** Obsidian Light (#121212) used for cards and containers to create a subtle lift.
3. **Accents:** Depth is further articulated through **1px Muted Gold (#8E7340) outlines**. These "Ghost Borders" should have a low-opacity (approx 30%) to appear as fine-lined architectural details.
4. **Active State:** Use a 1px solid Luxury Gold (#B99552) border for focused or active elements, creating a "glow" effect without using actual blurs.

## Shapes
This design system utilizes **Sharp (0px)** corners for all primary UI elements, including buttons, cards, and input fields. Sharp edges evoke a sense of precision, professional discipline, and architectural permanence. 

Roundness should only be used for elements that represent human interaction or fluidity, such as circular play buttons or specific icon containers, but structural components must remain strictly rectangular.

## Components
- **Buttons:** Primary buttons use a solid Luxury Gold (#B99552) background with Black text. Secondary buttons are "Ghost" style: 1px Muted Gold border with Warm Ivory text. Transitions should be slow (300ms) to feel cinematic.
- **Input Fields:** Obsidian Light (#121212) backgrounds with a bottom-only 1px Muted Gold border. Labels should use the `label-caps` typography style.
- **Cards:** Cards should have no background fill (transparent) or a very subtle Obsidian Light fill. They are defined by their 1px Muted Gold borders.
- **Film Grain Overlay:** A global fixed-position `div` with a noise texture at 3% opacity should sit above all background colors but below text content.
- **Navigation:** Minimalist top-bar navigation. Use high letter-spacing on `label-caps` for nav links. No background blur; use solid Obsidian Black to maintain a heavy, grounded feel.