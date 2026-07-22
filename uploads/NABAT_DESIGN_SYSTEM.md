# Nabat AI — Design System & Brand Guidelines

**Version:** 2026  
**Last Updated:** April 23, 2026  
**Organization:** Nabat AI · The Operating System for Nature  
**Status:** Comprehensive — Extracted from Brand Guidelines & Executive Brief

---

## Quick Links

- **Fonts:** [Font Families](#font-families) | [Complete Font Stack](#complete-font-stack)
- **Colors:** [Core Palette](#core-palette---comprehensive) | [All Color Values](#all-color-values)
- **Spacing:** [Scale](#core-spacing-scale)
- **Components:** [Patterns](#components--patterns)

---

## Table of Contents

1. [Font Families](#font-families)
2. [Color System](#color-system)
3. [Typography](#typography)
4. [Spacing & Layout](#spacing--layout)
5. [Components & Patterns](#components--patterns)
6. [Visual Hierarchy](#visual-hierarchy)
7. [Accessibility](#accessibility)

---

## Font Families

### Complete Font Stack

| Font | Style | Weights | Usage | Import |
|------|-------|---------|-------|--------|
| **Cormorant Garamond** | Serif | 300, 400, 500, 600, 700 | Headlines, display text, editorial | `family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500` |
| **Inter Tight** | Sans-serif | 300, 400, 500, 600 | UI text, body, labels | `family=Inter+Tight:wght@300;400;500;600` |
| **JetBrains Mono** | Monospace | 300, 400, 500 | Code, technical labels, data | `family=JetBrains+Mono:wght@300;400;500` |

### Load Fonts (Google Fonts)

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500&family=Inter+Tight:wght@300;400;500;600&family=JetBrains+Mono:wght@300;400;500&display=swap" rel="stylesheet">
```

### Font Characteristics

**Cormorant Garamond**
- Elegant, high contrast serif
- Strong italic style for emphasis
- Best for: Display headings, manifesto statements, editorial voice
- Weights: 300 (light), 400 (regular), 500+ (bold)

**Inter Tight**
- Modern, geometric sans-serif
- Tightly spaced for efficiency
- Best for: UI elements, body text, labels, buttons
- Weights: 300 (light), 400 (regular), 500 (medium), 600 (bold)

**JetBrains Mono**
- Technical, fixed-width monospace
- Perfect readability for code and data
- Best for: Code snippets, technical labels, analytics
- Weights: 300 (light), 400 (regular), 500 (medium)

---

## Color System

## Color System

### All Color Values

#### CSS Variables (Semantic Names)

```css
:root {
  /* Text Colors */
  --ink: #0A1410;              /* Primary text */
  --ink-soft: #1C2A23;         /* Soft text, secondary content */
  --ink-muted: #4A5A50;        /* Muted text, captions */
  
  /* Background Colors */
  --paper: #F4EFE4;            /* Primary light background */
  --paper-warm: #EDE5D2;       /* Warm paper shade */
  --paper-deep: #E6DCC2;       /* Deep paper shade */
  

}
```

### Core Palette - Comprehensive

#### Primary Brand Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| **Brand Primary** | `#246C5F` | rgb(36, 108, 95) | Primary brand color, key interactive elements |
| **Primary Green Dark** | `#0D482E` | rgb(13, 72, 46) | Supporting green, secondary accents |
| **Nature Green** | `#00754A` | rgb(0, 117, 74) | Alternative primary, accent highlighting |
| **Button Green (Bright)** | `#63D487` | rgb(99, 212, 135) | Call-to-action, success states, buttons |

#### Neutral & Background Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| **Light Background** | `#FAFAF5` | rgb(250, 250, 245) | Primary page background |
| **Alt Background** | `#ECEBEA` | rgb(236, 235, 234) | Secondary background, hover states |
| **Pale Accent** | `#F7F9F3` | rgb(247, 249, 243) | Very light background support |
| **Accent Light** | `#E7F4EE` | rgb(231, 244, 238) | Light green background |
| **Dark Background** | `#111512` | rgb(17, 21, 18) | Dark mode page background |
| **Dark Forest** | `#0B1F17` | rgb(11, 31, 23) | Dark mode primary |
| **Forest 2** | `#0F2A1F` | rgb(15, 42, 31) | Dark shade alternative |
| **Forest 3** | `#15362A` | rgb(21, 54, 42) | Dark shade deep |

#### Text Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| **Text Primary** | `#0A1410` | rgb(10, 20, 16) | Main body text, primary content |
| **Text Soft** | `#1C2A23` | rgb(28, 42, 35) | Secondary text, slightly emphasized |
| **Text Muted** | `#4A5A50` | rgb(74, 90, 80) | Tertiary text, captions, metadata |
| **Text Soft Alt** | `#393B3A` | rgb(57, 59, 58) | Alternative muted text |

#### Gold & Accent Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| **Gold (Standard)** | `#B89968` | rgb(184, 153, 104) | Default accent, borders, dividers |
| **Gold Bright** | `#D4B577` | rgb(212, 181, 119) | Bright accent, emphasis, highlights |
| **Gold Deep** | `#8C6F3F` | rgb(140, 111, 63) | Deep accent, supporting gold |
| **Rule Color** | `#2A3A30` | rgb(42, 58, 48) | Borders, dividing lines |
| **Rule Paper** | `#B8A87E` | rgb(184, 168, 126) | Rules on paper backgrounds |

#### Dividers & Supporting Colors
| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| **Divider** | `#D8D4DA` | rgb(216, 212, 218) | Subtle borders, dividers |
| **Text Muted (Green)** | `#51765C` | rgb(81, 118, 92) | Muted green text, secondary content |

### Green Palette Ramps

The following colors represent the complete green palette system:

**Brand Primary Ramp** (Base: #246C5F)
- 50: #F0F7F5
- 100: #DCF1ED
- 200: #BDE3DC
- 300: #9FD5CB
- 400: #7AC4B5
- 500: #5BB3A0
- 600: #3C9F85
- 700: #246C5F (base)
- 800: #1A5247
- 900: #0F3830

**Nature Green Ramp** (Base: #0D482E)
- 50: #EEF5F2
- 100: #D6E8E2
- 200: #B1D9CC
- 300: #84C9B0
- 400: #5DB795
- 500: #3D9B76
- 600: #1E8656
- 700: #0D482E (base)
- 800: #093620
- 900: #051F14

**Button Green Ramp** (Base: #63D487)
- 50: #F2FCF7
- 100: #D9F5E6
- 200: #B3E8C7
- 300: #84DFC6
- 400: #6FD892
- 500: #5FD4B2
- 600: #41B396
- 700: #2A9478
- 800: #1A735E
- 900: #009D4B (bright)

**Support Green Ramp**
- Includes: #51765C, #2C514D, and complementary shades

### Color Usage Rules

- **Primary Green (#246C5F)** — Brand identity, main CTAs, key interactive elements
- **Button Green (#63D487)** — Buttons, success states, positive actions
- **Dark Forest** — Dark mode backgrounds, high contrast text
- **Gold (#B89968)** — Borders, dividers, luxury accents, emphasis
- **Neutral tones** — Support layout, maintain readability, create breathing room
- **High contrast** — All combinations meet WCAG AA minimum (4.5:1 for text)

---

## Typography

### Font Families

#### Cormorant Garamond (Serif)
- **Weights:** 300, 400, 500, 600, 700
- **Styles:** Normal, Italic
- **Usage:** Headlines, display text, manifesto statements, editorial voice
- **Best for:** Large titles, emphasis, sophisticated branding
- **Fallback:** `serif`

#### Inter Tight (Sans-serif)  
- **Weights:** 300, 400, 500, 600
- **Styles:** Normal
- **Usage:** UI elements, body text, labels, buttons
- **Best for:** Clean, modern, highly legible interface text
- **Fallback:** `sans-serif`

#### JetBrains Mono (Monospace)
- **Weights:** 300, 400, 500
- **Styles:** Normal
- **Usage:** Code snippets, technical labels, data display, analytics
- **Best for:** Fixed-width text requiring alignment and precision
- **Fallback:** `monospace`

### Type Scale & Styles

#### Display Headings
```
H1 — 104px | Weight: 300 (Cormorant Garamond)
    Line-height: 0.92 | Letter-spacing: -0.02em
    Usage: Page titles, manifesto statements
    
H2 — 72px | Weight: 300 (Cormorant Garamond)
    Line-height: 1.02 | Letter-spacing: -0.02em
    Usage: Section headers, major statements
    
H2 Display — 56px | Weight: 400 (Cormorant Garamond)
    Line-height: 1.02 | Letter-spacing: -0.015em
    Usage: Content section headers
    
H3 (Subtitle) — 22px | Weight: 400 (Cormorant Garamond)
    Line-height: 1.45 | Font-style: italic
    Usage: Subheadings, descriptive text
```

#### Body Text
```
Body — 13px | Weight: 400 (Inter Tight)
    Line-height: 1.7 | Color: #1C2A23 (ink-soft)
    Max-width: 560px
    Paragraph spacing: 14px
    Usage: Main reading copy
    
Lede (Introduction) — 22px | Weight: 400 (Cormorant Garamond)
    Line-height: 1.45 | Italic
    Color: #4A5A50 (ink-muted)
    Usage: Opening paragraphs, key messages
```

#### Metadata & Labels
```
Label — 9.5px | Weight: 600 (Inter Tight)
    Letter-spacing: 0.22em | Text-transform: uppercase
    Usage: Section labels, captions
    
Section Label — 10px | Weight: normal (Inter Tight)
    Letter-spacing: 0.3em | Text-transform: uppercase
    Usage: Category headers, tags
    
Masthead — 9.5px | Weight: normal (Inter Tight)
    Letter-spacing: 0.22em | Text-transform: uppercase
    Usage: Page headers, footers
    
Code/Monospace — 8-9px | Weight: normal (JetBrains Mono)
    Letter-spacing: 0.12-0.14em | Text-transform: uppercase
    Usage: Technical labels, API references
```

### Typography - Emphasis & Styling

- **Italic:** Used in Cormorant Garamond for emphasis, elegance, and editorial voice
- **Bold/Weight 600:** Used for emphasis in UI labels and important terms
- **Drop Caps:** Oversized first letters in editorial content (86px, color: `#8C6F3F`)
- **Pull Quotes:** 26px, italic, left-bordered with 2px `#B89968` rule, 36px top/bottom margin

---

## Spacing & Layout

### Core Spacing Scale

```
2px   — Micro-spacing, borders
4px   — Fine spacing
8px   — Small spacing
12px  — Medium-small
14px  — Paragraph spacing
18px  — Item gaps
24px  — Section spacing
28px  — Medium section spacing
32px  — Large spacing
36px  — Extra large spacing
40px  — XL spacing
44px  — Section transitions
48px  — Major section spacing
56px  — Large section gaps
64px+ — Page-level spacing
```

### Page Layout

#### Print/Page Dimensions
- **Format:** A4 (210x297mm at 96dpi ≈ 794x1123px)
- **Margins:** 72-92px on all sides (executive brief)
- **Page Background:** `#FAFAF5` (light) or `#0B1F17` (dark)
- **Gutter:** 28-40px between content blocks

#### Framing & Borders
- **Frame Border:** 1px solid `#B8A87E` (gold-rule-paper)
- **Frame Inset (secondary):** 1px solid `#B8A87E` at 45% opacity, inset 32px
- **Corner Ornaments:** 30x30px decorative corners at cardinal positions

#### Grid & Columns
- **Two-Column Layout:** `grid-template-columns: 1fr 1fr; gap: 48px`
- **Three-Column Ledger:** Columns: 46px | 1fr | 140px; Gap: 18px
- **Body Margins (tight):** top: 110px; left/right: 92px; bottom: 100px

### Padding & Inset Values

```
Container Padding:    24px–40px (content area padding)
Card Padding:         20px–32px (internal card spacing)
Button Padding:       12px–16px (vertical) × 20px–24px (horizontal)
Text Block Padding:   24px–32px (around text content)
Item Spacing:         12px–18px (between list items)
Border Padding:       28px–32px (around framed content)
```

---

## Components & Patterns

### Decorative Elements

#### Gold Accent Rules
- **Color:** `#B89968` (gold) | `#D4B577` (gold-bright) | `#8C6F3F` (gold-deep)
- **Usage:** Borders, dividers, emphasis rules
- **Thickness:** 1px (thin) to 2px (emphasis)
- **Margin:** 28px top/bottom for horizontal rules

#### Monogram (Brand Mark)
- **Size:** 92px × 92px
- **Ring 1 (outer):** 1px border, `rgba(184,153,104,.55)` (gold, 55% opacity)
- **Ring 2 (inner):** 8px inset, `rgba(184,153,104,.9)` (gold, 90% opacity)
- **Letter:** 44px, Cormorant Garamond, italic, weight 500, color `#D4B577` (gold-bright)
- **Smaller variant:** 72px × 72px for footer/signature use

#### Seals & Decorative Circles
- **Large Seal:** 560px diameter circle, positioned off-canvas for visual interest
- **Border:** 1px solid `rgba(184,153,104,.18)` (very light gold)
- **Inner Seal:** 60px inset, 1px border at 10% opacity
- **Dashed Inner:** 120px inset, 1px dashed at 15% opacity

### Card Patterns

#### Principle Card (Circular)
- **Size:** 569px × 569px
- **Circle Content:** 449px × 449px ellipse, centered
- **Text Block:** 405px width, centered within circle
- **Label Padding:** 95.5px horizontal centering
- **Copy Height:** 132px max (3-4 lines)

#### Ledger Item (Tabular List)
```
Grid: 46px (number) | 1fr (content) | 140px (tag)
Padding: 12px vertical, 0 horizontal
Border-bottom: 1px solid #B8A87E
First item: Border-top as well
```

- **Number:** 26px, Cormorant Garamond, italic, color `#8C6F3F` (gold-deep)
- **Title:** 16px, weight 500, color `#0A1410` (ink)
- **Description:** 11px, weight 400, line-height 1.5, max-width 460px, color `#4A5A50` (ink-muted)
- **Tag:** 8px, monospace, letter-spacing 0.14em, uppercase

#### Stat Block
- **Key (Stat):** 34px, Cormorant Garamond, italic, color `#D4B577` (gold-bright)
- **Value (Description):** 9px, Inter Tight, uppercase, max-width 140px, line-height 1.5

### Pull Quote / Emphasis Box
```
Font-size: 26px
Font-family: Cormorant Garamond, italic
Font-weight: 400
Color: #0F2A1F (forest-2)
Padding: 28px top/bottom × 24px left
Border-left: 2px solid #B89968 (gold)
Margin: 36px top/bottom
Max-width: 560px
```

---

## Visual Hierarchy

### Text Color Hierarchy

#### Dark Mode (`#0B1F17` background)
1. **Primary Text:** `#F4EFE4` (paper) — Main content
2. **Secondary Text:** `rgba(244,239,228,.88)` — Subtle emphasis
3. **Tertiary Text:** `rgba(244,239,228,.6)` — Captions, metadata
4. **Muted Text:** `rgba(244,239,228,.5)` — Footer, folio

#### Light Mode (`#FAFAF5` background)
1. **Primary Text:** `#0A1410` (ink) — Main content
2. **Secondary Text:** `#1C2A23` (ink-soft) — Subtle emphasis
3. **Tertiary Text:** `#4A5A50` (ink-muted) — Captions, metadata
4. **Muted Text:** `#393B3A` (ink-soft) — Deemphasized

### Accent Hierarchy
1. **Primary Accent:** `#D4B577` (gold-bright) — Most important
2. **Secondary Accent:** `#B89968` (gold) — Supporting
3. **Tertiary Accent:** `#8C6F3F` (gold-deep) — Minimal use

---

## Accessibility

### Contrast Standards
- **Text on backgrounds:** Minimum WCAG AA (4.5:1 for normal text, 3:1 for large)
- **Gold on dark backgrounds:** Verified for accessibility
- **Green on white:** High contrast maintained

### Typography Accessibility
- **Line length:** Max 560-640px for optimal readability
- **Line-height:** Minimum 1.45 for body text (1.7 for web)
- **Font size:** Minimum 13px for body, 9px for captions
- **Letter-spacing:** Adequate spacing for dyslexia support in headers

### Color Usage
- **Never rely on color alone** for information
- **Icons, labels, and text** accompany color-coded elements
- **Sufficient contrast** in all color combinations
- **Alternative text** for decorative images

---

## Implementation Notes

### When Using This System

#### 1. Font Loading

**HTML (Google Fonts):**
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500&family=Inter+Tight:wght@300;400;500;600&family=JetBrains+Mono:wght@300;400;500&display=swap" rel="stylesheet">
```

**CSS Font Stacks:**
```css
/* Headlines & Display */
font-family: 'Cormorant Garamond', serif;

/* UI & Body */
font-family: 'Inter Tight', sans-serif;

/* Code & Data */
font-family: 'JetBrains Mono', monospace;
```

#### 2. Color Variables

Use CSS custom properties for semantic color management:

```css
:root {
  /* Text */
  --ink: #0A1410;
  --ink-soft: #1C2A23;
  --ink-muted: #4A5A50;
  
  /* Background */
  --paper: #F4EFE4;
  --paper-warm: #EDE5D2;
  --paper-deep: #E6DCC2;
  
  /* Dark Mode */
  --forest: #0B1F17;
  --forest-2: #0F2A1F;
  --forest-3: #15362A;
  
  /* Accents */
  --gold: #B89968;
  --gold-bright: #D4B577;
  --gold-deep: #8C6F3F;
  
  /* Borders */
  --rule: #2A3A30;
  --rule-paper: #B8A87E;
}

/* Light Mode */
body {
  color: var(--ink);
  background: var(--paper);
}

/* Dark Mode */
body.dark {
  color: var(--paper);
  background: var(--forest);
}
```

#### 3. Spacing Scale

Use an 8px base unit for consistency:

```css
/* 8px-based scale */
--space-xs: 4px;    /* 0.5x */
--space-sm: 8px;    /* 1x */
--space-md: 12px;   /* 1.5x */
--space-lg: 24px;   /* 3x */
--space-xl: 32px;   /* 4x */
--space-xxl: 48px;  /* 6x */
--space-section: 56px; /* 7x */
```

#### 4. Typography Configuration

```css
/* H1 */
font-family: 'Cormorant Garamond';
font-size: 104px;
font-weight: 300;
line-height: 0.92;
letter-spacing: -2px;

/* H2 */
font-family: 'Cormorant Garamond';
font-size: 72px;
font-weight: 300;
line-height: 1.02;
letter-spacing: -1.5px;

/* Body */
font-family: 'Inter Tight';
font-size: 13px;
font-weight: 400;
line-height: 1.7;
color: var(--ink-soft);

/* Label */
font-family: 'Inter Tight';
font-size: 9.5px;
font-weight: 600;
letter-spacing: 2.2px;
text-transform: uppercase;
color: var(--gold-deep);
```

#### 5. Dark Mode Implementation

```css
/* Swap colors systematically */
body.dark {
  --ink: #F4EFE4;           /* Light text */
  --ink-soft: rgba(244, 239, 228, 0.88);
  --ink-muted: rgba(244, 239, 228, 0.6);
  --paper: #0B1F17;         /* Dark background */
  --paper-warm: #0F2A1F;
  --paper-deep: #15362A;
}
```

#### 6. Component Building

- Build with semantic HTML (no div-itis)
- Use CSS variables for colors and spacing
- Implement progressive enhancement
- Ensure responsive design with breakpoints
- Test accessibility at each stage (WCAG AA)

---

## Brand Voice through Design

- **Sophisticated:** Serif typography for editorial authority
- **Natural:** Deep greens, organic shapes, natural materials inspiration
- **Trustworthy:** Consistent spacing, clear hierarchy, clean layouts
- **Technical:** Monospace for data, grids for structure
- **Refined:** Generous whitespace, restrained color palette, careful ornaments

---

## References

- **Figma Design File:** [Nabat Brand Guidelines](https://www.figma.com/design/fRGnenV3KBzlGaRXLmAuPU)
- **Executive Brief:** Nabat AI Establishment Document (2026)
- **Previous:** Nabat Brand Guidelines – Color System, Typography, Layout

---

**End of Design System Document**

---

## Quick Reference

### Colors
| Purpose | Color | Hex |
|---------|-------|-----|
| Primary Brand | Deep Green | `#246C5F` |
| Action/Buttons | Bright Green | `#63D487` |
| Text | Dark | `#0A1410` |
| Background | Off-white | `#FAFAF5` |
| Accent | Gold | `#B89968` |

### Fonts
| Use | Font | Size | Weight |
|-----|------|------|--------|
| Headlines | Cormorant Garamond | 56–104px | 300–400 |
| Body | Inter Tight | 13px | 400 |
| Code | JetBrains Mono | 8–9px | 400 |

### Spacing
| Element | Space |
|---------|-------|
| Padding | 24–32px |
| Gap | 28–48px |
| Margin | 36–56px |

