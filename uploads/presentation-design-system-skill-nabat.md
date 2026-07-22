---
name: presentation-design-system-enterprise
description: |
  Comprehensive design system for enterprise-grade presentation decks focused on 
  geospatial intelligence, climate tech, and data-driven storytelling. Two-column 
  card-based architecture with deep forest/emerald green palette, Poppins typography, 
  and trust-first visual language optimized for investor and technical stakeholder 
  communication. Emphasis on signal-to-noise ratio, semantic grouping, and weight-driven 
  hierarchy without decorative excess.
version: "1.0"
---

# Enterprise Presentation Design System
## Geospatial Intelligence & Climate-Tech Focus

## 1. Visual Theme & Atmosphere

This presentation system embodies **trust-first intelligence design**—a visual language built for stakeholders reviewing investment theses, technical specifications, and impact narratives. The aesthetic borrows from Bloomberg, Stripe, and Palantir: clarity over expression, data-as-design, and modular information architecture that reads equally well on a 27" presentation monitor or a printed PDF.

The design philosophy is **narrative-driven cards**: each slide contains a single positioning statement (left column) supported by structured evidence blocks (right column). No decorative imagery. No unnecessary transitions. No color spectacle. The deep forest/emerald green anchors the brand trustworthiness; the near-white background and subtle mint overlays create visual breathing room; muted gold/sand accent circles highlight secondary data insights. Typography does all the work through weight contrast and tight hierarchy—600–700 weight for headlines, 400–450 weight for body, and careful tracking to maintain readability at projection scale.

**Key Characteristics:**
- Two-column split layout: positioning statement (left) + evidence grid (right)
- Card-based container system with rounded rectangles (12–20px radius)
- Subtle 1px borders instead of drop shadows — precision over drama
- Poppins font family (600–700 weight headlines, 400–450 weight body)
- Deep forest/emerald green as primary anchor (`#1a4d3e`, `#2d7a6d`)
- Near-white canvas with warm/green tint (`#f8faf8`, `#fafbf8`)
- Light mint overlay containers (`#e8f3f0`, `#f0f4f2`)
- Muted gold/sand accent circles (`#c9a876`, `#b8956f`)
- Dark charcoal text (`#1a1a1a`, `#2a2a2a`) for maximum readability
- Semantic grouping labels ("Remote Sensing", "Geospatial AI", "Impact Monitoring")
- Minimal line icons + numeric data as primary visual language
- No decorative imagery — every graphic serves information architecture
- High signal-to-noise ratio: every pixel justifies its presence

---

## 2. Color Palette & Roles

### Primary Brand & Anchor
- **Deep Forest** (`#1a4d3e`): Primary brand accent. Used for primary CTA buttons, section headers, navigation anchors, and the left-column positioning statement background. Conveys stability, sustainability, and earth stewardship.
- **Emerald** (`#2d7a6d`): Secondary forest shade. Used for hover states on forest buttons, secondary headlines, and accent borders on key evidence blocks.
- **Forest Light** (`#4a9a87`): Tertiary forest tone. Used for secondary buttons, disabled states, and muted navigation elements.

### Background & Surface
- **Canvas White** (`#f8faf8`): Dominant slide background. A near-white with a barely-perceptible warm/green undertone that signals sustainability without announcing it.
- **Canvas Off-White** (`#fafbf8`): Alternate background for alternate slides in a deck sequence. Minimal contrast to white, used for gentle visual rhythm.
- **Mint Overlay** (`#e8f3f0`): Light translucent background for evidence block containers. Suggests freshness and data integrity without visual loudness.
- **Mint Deep** (`#f0f4f2`): Secondary mint shade for bordered cards and inset containers.
- **Pure White** (`#ffffff`): Reserved for card surfaces, modal overlays, and high-contrast UI controls.

### Accent & Highlight
- **Muted Gold** (`#c9a876`): Secondary accent circle used to highlight metric numbers, timestamp labels, and positive-sentiment data points. Reads as "refined insight" without the loudness of bright yellow.
- **Sand Tone** (`#b8956f`): Darker gold variant for hover states, active indicators, and metric emphasis.

### Text & Semantic
- **Ink Dark** (`#1a1a1a`): Primary text color. Used for headline and body copy on light backgrounds. Maintains 12:1 contrast ratio with canvas white.
- **Charcoal** (`#2a2a2a`): Secondary text. Used for supporting copy, captions, metadata, and navigation labels.
- **Mute Gray** (`#5a5a5a`): Tertiary text. Used for timestamps, secondary metadata, and disabled UI states.
- **Light Gray** (`#8e8e8e`): Placeholder text in inputs, disabled buttons, and very light supporting text.
- **Hairline Light** (`#d9d9d5`): Subtle 1px borders on evidence cards in light regions.
- **Hairline Dark** (`#4a4a4a`): Subtle 1px borders on dark-background sections.

### Semantic Intent
- **Success** (`#2d7a6d`): Green tint (same as forest accent) used for positive metrics, "on track" indicators, and checkmarks.
- **Warning** (`#c9a876`): Gold tint used for caution labels, pending metrics, and attention-seeking highlights.
- **Alert** (`#d97966`): Warm red used for at-risk metrics, deadline warnings, and error states — rare and highly intentional.
- **Neutral** (`#8e8e8e`): Gray for neutral data, disconnected indicators, and "unknown" states.

---

## 3. Typography Rules

### Font Family

**Poppins** is the system's singular typeface family. All roles — display, body, labels, data — use Poppins with varying weights and sizes. This creates a cohesive, recognizable voice across slides and reinforces the system's precision.

- **Display**: Poppins weight 600–700 at sizes 32–56px
- **Body**: Poppins weight 400–450 at sizes 14–18px
- **Labels & Captions**: Poppins weight 500–600 at sizes 11–14px
- **Data & Numbers**: Poppins weight 700 at sizes 18–40px

Fallback stack: `Poppins, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`

### Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing | Use |
|------|------|--------|-------------|----------------|-----|
| Slide Title | 40px | 700 | 1.2 | -0.4px | Section opener, single-purpose headline |
| Section Header | 32px | 600 | 1.25 | 0px | Sub-section title, column header |
| Evidence Title | 24px | 600 | 1.3 | 0px | Evidence block heading inside right column |
| Body Large | 18px | 400 | 1.6 | 0.3px | Positioning statement, narrative prose |
| Body Standard | 16px | 400 | 1.55 | 0.2px | Default paragraph text, descriptions |
| Label Bold | 14px | 600 | 1.4 | 0.1px | Semantic grouping labels ("Remote Sensing") |
| Label Standard | 14px | 500 | 1.4 | 0px | Secondary labels, metadata |
| Caption | 12px | 500 | 1.5 | 0px | Timestamps, footnotes, disclaimers |
| Data Large | 40px | 700 | 1.0 | -0.5px | Key metric numbers (impact figures, growth rates) |
| Data Medium | 28px | 700 | 1.0 | -0.3px | Secondary metric numbers |
| Data Small | 18px | 700 | 1.0 | 0px | Inline data / inline comparison numbers |
| Button | 14px | 600 | 1.4 | 0.1px | CTA button labels |

### Principles

- **Weight hierarchy over size**: The system uses 400 (regular), 500 (medium), 600 (semibold), and 700 (bold) weights to establish hierarchy. Size changes are intentional but secondary to weight contrast.
- **Tight tracking on display**: Headlines at 32px+ use slight negative letter-spacing (-0.3 to -0.5px) to create visual tightness, evoking precision and data density.
- **High readability at projection**: All body text maintains minimum 1.5 line-height for comfortable reading from distance. No text smaller than 12px.
- **Number emphasis via weight**: Data numbers always use weight 700 at display sizes (18–40px), creating immediate visual hierarchy that readers scan for insights.
- **Semantic labels as anchors**: Grouping labels like "Remote Sensing" or "Geospatial AI" use weight 600 at 14px to mark semantic boundaries without visual noise.
- **No italics, no all-caps**: Emphasis is achieved through weight contrast only. All text uses sentence case. No decorative type treatments.

---

## 4. Component Styling

### Positioning Statement (Left Column)

**Layout**
- Width: ~35–40% of slide
- Height: Full slide height (often scrolling past single viewport on long slides)
- Background: Forest Green (`#1a4d3e`)
- Text color: Pure White (`#ffffff`)
- Padding: 48px vertical, 32px horizontal
- Border-radius: 0px (column edge is flush to slide edge)

**Content Structure**
- Eyebrow label: Poppins 600, 12px, all-caps, tracking 0.1px, opacity 0.85 (muted but present)
- Main statement: Poppins 600, 32–40px, weight 600–700, line-height 1.25, -0.3px tracking
- Supporting paragraph: Poppins 400, 16px, line-height 1.6, opacity 0.9

**Example:**
```
REMOTE SENSING

Monitor Mangrove 
Restoration at Scale

Real-time satellite imagery and AI 
classification enable continuous 
impact tracking across protected sites.
```

### Evidence Block Card (Right Column)

**Default Card**
- Background: Mint Overlay (`#e8f3f0`)
- Border: 1px solid Hairline Light (`#d9d9d5`)
- Border-radius: 16px
- Padding: 24px (inner)
- Margin bottom: 16px
- Box-shadow: none (borders only, no drop shadows)

**Card Header**
- Title: Poppins 600, 18px, Ink Dark (`#1a1a1a`)
- Subtitle/metadata: Poppins 500, 13px, Mute Gray (`#5a5a5a`)

**Card Content Sections**
- Metric rows: Poppins 400, 14px, with inline Poppins 700, 18px data numbers
- List items: Poppins 400, 14px, line-height 1.6, with semantic bullet markers (not standard bullets—use Forest Green circles)
- Captions: Poppins 500, 12px, Charcoal (`#2a2a2a`)

**Accent Highlight on Card**
- Top border accent: 4px solid Forest Light (`#4a9a87`) added to top of card when marking "key insight"
- Numeric highlight circle: Muted Gold (`#c9a876`) circular background behind metric numbers (50px diameter, flexbox-centered)

**Interactive States**
- Hover: Background shifts to Mint Deep (`#f0f4f2`), border to Emerald (`#2d7a6d`)
- Active (selected): Border color becomes Forest Green (`#1a4d3e`), 2px solid
- Disabled: Opacity 0.5, border color shifts to Light Gray (`#8e8e8e`)

### Buttons

**Primary CTA** — Call-to-action on forest green backgrounds
- Background: Pure White (`#ffffff`)
- Text: Forest Green (`#1a4d3e`), weight 600, 14px
- Padding: 12px 28px
- Border-radius: 8px
- Border: 1px solid Pure White (invisible at rest)
- Transition: all 0.3s ease-out

States:
- Hover: Background lightens to off-white, border becomes Forest Green
- Active/Pressed: Background becomes Mint Overlay, text darkens to Ink Dark

**Secondary CTA** — Action on white/mint backgrounds
- Background: transparent
- Text: Forest Green (`#1a4d3e`), weight 600, 14px
- Border: 1px solid Forest Green
- Padding: 11px 27px (accounts for border)
- Border-radius: 8px

States:
- Hover: Background fills with Mint Overlay, border stays Forest Green
- Active: Background fills with Forest Green, text becomes Pure White

**Semantic Button** — Warning / alert action
- Background: Alert Red (`#d97966`)
- Text: Pure White, weight 600, 14px
- Padding: 12px 28px
- Border-radius: 8px
- Border: 1px solid Alert Red

### Evidence Grid Layout

**Two-up card grid** (default for right column)
- Gap between cards: 16px horizontal, 20px vertical
- Each card width: ~47% of right-column width
- Stacking: flows left → right, then wraps to next row

**Single-column layout** (alternative for deep/narrow spaces)
- Card width: 100% of right-column width
- Used when evidence is particularly dense or tall

**Data table inside evidence block**
- Header row: Poppins 600, 12px, Charcoal on Mint Deep background, 1px solid border below
- Body rows: Poppins 400, 13px, Ink Dark text, alternating row backgrounds (white / Mint Overlay)
- Numbers: Poppins 700, 14px, right-aligned
- Borders: 1px Hairline Light between rows
- Padding: 12px per cell

### Navigation & Slide Indicators

**Slide Title Bar** (top of slide, optional)
- Background: Canvas White (`#f8faf8`)
- Height: 56px
- Slide number: Poppins 600, 12px, Mute Gray, left-aligned with 24px padding
- Breadcrumb nav: Poppins 500, 12px, Charcoal, center-aligned (e.g., "Impact → Mangrove → Restoration")
- Top divider: 1px solid Hairline Light

**Progress indicator** (bottom-right corner, subtle)
- Current slide / total slides: Poppins 500, 11px, Light Gray
- Visual bar: 2px solid Forest Light behind text
- Opacity: 0.6

### Data Visualization Components

**Metric Card with Accent Circle**
```
┌─────────────────────────────┐
│  Mangrove Coverage          │
│                             │
│      ◯ 2,847                │  ← Gold circle, 50px diameter
│      hectares               │
│      +18% YoY               │  ← Success green, 500 weight
└─────────────────────────────┘
```

**Timeline / Process Flow**
- Horizontal line: 2px solid Forest Light
- Step circles: 40px diameter, alternating Forest Green (completed) / Mint Overlay (future)
- Step labels: Poppins 600, 12px, Charcoal, centered below circle
- No decorative connectors—line-only connection between steps

**Icon + Label Pairs**
- Icons: 24px line-based icons (not filled), Forest Green stroke
- Label: Poppins 600, 13px, Charcoal, 8px below icon
- Grouping label: Poppins 600, 12px, Mute Gray, 12px above icon group

---

## 5. Layout Principles

### Spacing System

**Base unit**: 8px

**Common spacing tokens:**
- `xs`: 4px
- `sm`: 8px
- `md`: 12px
- `lg`: 16px
- `xl`: 24px
- `xxl`: 32px
- `block`: 48px
- `section`: 64px

**Application:**
- Column padding: 32px horizontal (half-block)
- Card padding: 24px (3 × base)
- Gap between cards: 16px (2 × base)
- Gap between sections: 48px (full block)
- Button padding: 12px vertical, 28px horizontal

### Two-Column Slide Grid

**Standard layout:**
- Left column: 35–40% of slide width
- Right column: 60–65% of slide width
- Gutter: 24px (3 × base)
- Column padding: 32px all sides
- Total slide width: 1440px (16:9 presentation standard)
  - Left column: 504px + 32px padding = 568px
  - Gutter: 24px
  - Right column: 848px + 32px padding = 912px
  - Total: 568 + 24 + 912 = 1504px (accounting for rounding)

**Single-column slides** (alternate layout):
- Full-width centered content
- Max content width: 1200px
- Padding: 48px horizontal, 64px vertical
- Used for title slides, transition slides, full-width visualizations

### Whitespace Philosophy

**Generosity as trust signal**: The system uses whitespace intentionally to suggest financial stability and operational clarity. A slide with one positioning statement and three evidence blocks feels **deliberate and curated**, not rushed or dense. Empty space is never "wasted"—it's the frame around each idea.

**Breathing room metrics:**
- Minimum line-height: 1.5 on all body text
- Minimum gap between sections: 48px
- Minimum card padding: 24px
- No element crowding to fill space

### Border Radius Scale

| Value | Use |
|-------|-----|
| 0px | Column edges (left positioning column), full-bleed sections |
| 8px | Buttons, small inline elements, input fields |
| 12px | Small data cards, compact evidence blocks |
| 16px | Standard evidence block cards (default) |
| 20px | Large feature cards, hero data containers |
| 50% | Metric highlight circles, avatar placeholders |

### Visual Rhythm

The standard slide follows this rhythm:

```
[Left Column]          [Right Column]
┌──────────────────┐  ┌──────────────────┬──────────────────┐
│ POSITIONING      │  │ Evidence Block 1 │ Evidence Block 2 │
│ STATEMENT        │  ├──────────────────┴──────────────────┤
│                  │  │ Evidence Block 3 (full-width)       │
│                  │  ├──────────────────┬──────────────────┤
│ (Single idea,    │  │ Evidence Block 4 │ Evidence Block 5 │
│  no interruption)│  └──────────────────┴──────────────────┘
└──────────────────┘
```

This creates a visual hierarchy: left column is *thesis*, right column is *proof*.

---

## 6. Depth & Elevation

### Shadow Philosophy

**No drop shadows.** This system uses 1px borders and color-blocking instead of shadows. On a presentation screen or printed PDF, drop shadows lose contrast and create visual clutter at projection scale.

**Elevation through color:**
- Base level: Canvas White (`#f8faf8`)
- Elevated level: Pure White (`#ffffff`) or Mint Overlay (`#e8f3f0`)
- Accent level: Forest Green (`#1a4d3e`)

**Borders as depth:**
- 1px solid Hairline Light (`#d9d9d5`): subtle separation on light backgrounds
- 1px solid Emerald (`#2d7a6d`): emphasis on interactive or key cards
- 2px solid Forest Green (`#1a4d3e`): active/selected states

**Top accent border:**
- 4px solid Forest Light (`#4a9a87`) added to top of evidence card to mark "key insight" — acts as visual bookmark

---

## 7. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Large Desktop | ≥1440px | Two-column layout maintained, no clipping |
| Desktop | 1280–1439px | Column widths proportionally maintained, minimal overflow |
| Tablet | 1024–1279px | Two-column stacks to single-column; evidence grid becomes 1-up instead of 2-up |
| Mobile | <1024px | Single-column full-width; positioning statement becomes header bar (sticky or top-pinned) |

### Collapsing Strategy

**Tablet (1024–1279px):**
- Left column positioning statement becomes a collapsible panel (toggle icon, top-left)
- Right column expands to full width
- Evidence cards reflow to single-column grid
- Font sizes reduce by 1 step (32px headline → 28px, etc.)

**Mobile (<1024px):**
- Positioning statement moves to a fixed header bar (56px height, collapsible)
- Evidence cards display in single-column full-width
- Card padding reduces to 16px
- Metric numbers reduce: 40px → 32px, 28px → 24px
- Title bar slide indicators hidden; replaced with slide counter (e.g., "Slide 4 of 12")

### Touch Targets

- All buttons: minimum 44px height (WCAG AAA)
- All interactive cards: minimum 16px padding for easy tapping
- Evidence block titles: clickable for collapse/expand on mobile

---

## 8. Do's and Don'ts

### Do

- **Lead with positioning**: Every slide's left column should contain a single, memorable statement. One idea per column.
- **Use weight contrast**: Differentiate hierarchy through Poppins 400 → 600 → 700 weight progression. Avoid size changes unless necessary.
- **Pair metric with gold accent**: Any key performance number should sit inside or adjacent to a Muted Gold (`#c9a876`) circle for instant visual scanning.
- **Apply 1px borders only**: Use subtle borders on cards and containers. Shadows are forbidden.
- **Reserve Forest Green for emphasis**: Use Deep Forest (`#1a4d3e`) for primary CTAs, top-level headers, and the left column background. Use Emerald (`#2d7a6d`) for secondary emphasis and hover states.
- **Maintain 16–24px card padding**: This creates a sense of spacious, curated information design.
- **Use semantic labels**: Group evidence by meaningful category ("Remote Sensing", "Geospatial AI", "Impact Monitoring") to aid stakeholder navigation.
- **Let numbers dominate**: Data should be your primary visual language—use large Poppins 700 figures, then supporting text.
- **Treat whitespace as design**: Empty area on a slide is as important as filled area. Never fill space just to fill it.
- **Maintain 1.5+ line-height**: This ensures readability at projection scale and from distance.

### Don't

- **Don't decorate**: No gradients, patterns, or decorative shapes. No photography unless it serves the data directly (e.g., a satellite image for "Remote Sensing" positioning).
- **Don't mix typefaces**: Poppins only. Never introduce a secondary font.
- **Don't use drop shadows**: Borders (1px) only for elevation and separation.
- **Don't crowd the left column**: Maximum 3–4 sentences of positioning statement. One idea per slide.
- **Don't use more than 3 accent colors**: Forest Green + Muted Gold + (rarely) Alert Red. That's the complete palette.
- **Don't add animation or transitions**: In a presentation context, motion is distracting. Let the slide content stand alone.
- **Don't use all-caps text**: Sentence case only. Semantic labels use small-caps via CSS if necessary, but avoid default ALL-CAPS.
- **Don't reduce text below 12px**: Readability at projection scale is non-negotiable.
- **Don't italicize**: Emphasis via weight (600 → 700), not style.
- **Don't use semantic red/yellow/green for non-critical data**: Reserve Alert Red for actual alerts. Use Forest Green for positive, Muted Gold for cautionary.
- **Don't add decorative icons**: Icons must encode information, never just beautify.

---

## 9. Agent Prompt Guide

### Quick Color Reference

```
Forest Green (primary):    #1a4d3e
Emerald (secondary):       #2d7a6d
Forest Light:              #4a9a87
Canvas White:              #f8faf8
Mint Overlay:              #e8f3f0
Pure White:                #ffffff
Muted Gold (accent):       #c9a876
Sand Tone (gold hover):    #b8956f
Ink Dark (text):           #1a1a1a
Charcoal (secondary):      #2a2a2a
Mute Gray:                 #5a5a5a
Alert Red:                 #d97966
```

### Example Component Prompts

**Positioning Statement Column:**
```
Create a left-column positioning statement: 
- Background: Forest Green (#1a4d3e)
- Width: 35% of slide
- Eyebrow: Poppins 600, 12px, uppercase, white, opacity 0.85: "GEOSPATIAL AI"
- Title: Poppins 700, 40px, white, line-height 1.2, -0.3px tracking: "Real-time Impact Monitoring"
- Body: Poppins 400, 16px, white, line-height 1.6, opacity 0.9: "Satellite imagery + machine learning enables continuous mangrove health tracking..."
- Padding: 48px vertical, 32px horizontal
- Border-radius: 0px
```

**Evidence Card:**
```
Create an evidence card in a 2-up grid:
- Background: Mint Overlay (#e8f3f0)
- Border: 1px solid Hairline Light (#d9d9d5)
- Border-radius: 16px
- Padding: 24px
- Top border accent: 4px solid Forest Light (#4a9a87)
- Title: Poppins 600, 18px, Ink Dark (#1a1a1a): "Mangrove Coverage"
- Metric number: Poppins 700, 40px, in a 50px Muted Gold (#c9a876) circle: "2,847"
- Unit: Poppins 400, 14px, Charcoal (#2a2a2a): "hectares"
- Change: Poppins 600, 13px, Forest Green (#1a4d3e): "+18% YoY"
- Gap below card: 16px
- On hover: Background → Mint Deep (#f0f4f2), Border → Emerald (#2d7a6d)
```

**Data Table Inside Card:**
```
Create a data table:
- Header row: Poppins 600, 12px, white text on Mint Deep (#f0f4f2) background, 1px solid border below
- Body rows: Poppins 400, 13px, alternating white / Mint Overlay backgrounds
- Column alignment: text left, numbers right
- Numbers: Poppins 700, 14px
- Row borders: 1px solid Hairline Light (#d9d9d5)
- Cell padding: 12px
```

**Metric Card with Gold Highlight:**
```
Create a metric card:
- Background: Pure White (#ffffff)
- Border: 1px solid Hairline Light (#d9d9d5)
- Border-radius: 16px
- Padding: 20px
- Metric number: Poppins 700, 36px, inside a 48px diameter circle background Muted Gold (#c9a876), Ink Dark text
- Label: Poppins 500, 13px, Charcoal (#2a2a2a), 12px below circle
- Supporting text: Poppins 400, 12px, Mute Gray (#5a5a5a)
```

**Primary CTA Button:**
```
Create a primary CTA button (on Forest Green background):
- Background: Pure White (#ffffff)
- Text: Forest Green (#1a4d3e), Poppins 600, 14px
- Padding: 12px 28px
- Border-radius: 8px
- Border: 1px solid Pure White
- Transition: all 0.3s ease-out
- Hover state: Background → off-white (#f5f5f3), Border → Forest Green (#1a4d3e)
- Active state: Background → Mint Overlay (#e8f3f0), Text → Ink Dark (#1a1a1a)
```

### Iteration Guide

1. **Start with positioning**: Every slide must have a single, clear left-column statement. Draft that first.
2. **Then gather evidence**: List 3–5 supporting facts or metrics that validate the positioning statement.
3. **Group evidence by semantic category**: "Remote Sensing", "Geospatial AI", "Impact Monitoring"—these groupings become evidence card headers.
4. **Establish hierarchy through weight**: Use Poppins 700 for key numbers, 600 for titles, 400 for body. Size changes are secondary.
5. **Apply color restraint**: Forest Green for primary, Muted Gold for metric emphasis, Alert Red for warnings only. Nothing else.
6. **Check for signal-to-noise ratio**: Can a stakeholder understand the slide in 3 seconds by scanning the left column + the first 2 evidence cards? If not, cut something.
7. **Validate spacing**: 48px between sections, 24px card padding, 16px gap between cards. These create visual rhythm and luxury signal.
8. **Test at projection scale**: View mockups at 100% zoom, then zoom out to 50% to simulate viewing distance. Text must remain legible.

---

## 10. Known Gaps & Future Extensions

- **Dark mode variant**: A candidate dark-mode theme exists (pure black background, mint text, forest green accents) but is not documented here. Request if needed.
- **Animation layer**: Slide transitions and entrance animations are out of scope. This system focuses on static slide design. CSS transitions on hover/focus are recommended for interactivity.
- **Video/embedded asset integration**: Guidelines for embedding video or interactive charts within evidence cards are not yet documented.
- **Localization strategy**: Font stack and icon library assume Western European layouts. CJK, Arabic, and Devanagari fallbacks are available in the Poppins font but not explicitly styled here.
- **Print output**: PDF export guidelines (font embedding, color space, margin safety) are not yet documented.

---

## 11. Design Philosophy Statement

This system is built on the principle that **clarity is confidence**. In a presentation to investors, operators, and technical stakeholders, every design choice must earn its place. No decoration without function. No color without meaning. No text without purpose.

The deep forest green signals sustainability and earth stewardship—core to the climate-tech mission. The near-white canvas and mint overlays create breathing room, suggesting operational stability. The muted gold accents humanize the data without diluting precision. And Poppins throughout creates a single, recognizable voice across every slide.

The two-column architecture (positioning left, evidence right) mirrors how sophisticated audiences read: they scan the thesis first, then validate with data. Every slide follows this rhythm. Every slide answers one question. Every slide looks like it belongs to the same deck.

This is **trust-first design**. Not expressive. Not trendy. Not decorative. Effective.

---

## 12. Example Slide Layouts

### Title Slide
```
[Full-width centered, single-column]

IMPACT MONITORING ACROSS
PROTECTED MANGROVE SITES

Harnessing satellite imagery and machine learning to track 
ecological restoration in real time.

[Vertical spacing: 64px]
[Primary CTA button below: "See the Platform"]
```

### Content Slide (Standard Two-Column)
```
[Left Column - Forest Green Background]
GEOSPATIAL AI

Satellite Classification
at Scale

ML models process Sentinel-2 
imagery daily to identify mangrove 
extent, health, and change.

[Right Column - Evidence Cards in 2×3 Grid]
┌─────────────┬─────────────┐
│ Daily       │ Accuracy    │
│ Coverage    │ Rate        │
│ 2,847 ha    │ 94.2%       │
└─────────────┴─────────────┘
┌─────────────────────────────┐
│ Remote Sensing Capability   │
│ • Multispectral bands       │
│ • Sub-meter resolution      │
│ • Real-time alerts          │
└─────────────────────────────┘
```

### Metrics Slide (Single-Column, Data-Heavy)
```
[Full-width centered]

IMPACT SUMMARY: YEAR 1 RESTORATION

[Three metric cards in a row]
┌──────────┐  ┌──────────┐  ┌──────────┐
│ 2,847 ha │  │ +18% YoY │  │ 94.2%    │
│ Restored │  │ Growth   │  │ Accuracy │
└──────────┘  └──────────┘  └──────────┘

[Data table below, full-width]
Site        | Hectares | Health | Trend
─────────────────────────────────────
Abu Al Ab.  | 1,247    | 92%    | ↑ Improving
Khor Dubai  | 1,023    | 87%    | → Stable
Jebel Ali   | 577      | 89%    | ↓ Monitoring
```

---

**End of Design System Documentation**
