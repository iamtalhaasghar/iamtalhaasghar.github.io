---
name: Talha Asghar Portfolio
description: Academic portfolio and personal website for a senior backend engineer
colors:
  primary: "#059669"
  primary-light: "#d1fae5"
  primary-dark: "#047857"
  secondary: "#0284c7"
  secondary-light: "#e0f2fe"
  secondary-dark: "#0369a1"
  neutral-bg: "#fafbfc"
  neutral-surface: "#f1f5f9"
  neutral-text: "#0f172a"
  neutral-text-light: "#475569"
  neutral-border: "#e2e8f0"
  dark-bg: "#0b0e14"
  dark-surface: "#131720"
  dark-card: "#161b24"
  dark-text: "#e6e8ee"
  dark-text-light: "#9aa3b2"
  dark-border: "rgba(255, 255, 255, 0.08)"
typography:
  display:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "clamp(2rem, 5vw, 3.5rem)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "clamp(1.25rem, 3vw, 1.75rem)"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "0"
  label:
    fontFamily: "Inter, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "0.02em"
  mono:
    fontFamily: "JetBrains Mono, ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: "8px"
  md: "12px"
  lg: "16px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  2xl: "48px"
components: {}
---

# Design System: Talha Asghar Portfolio

## Overview

**Creative North Star: "The Precision Engineer"**

Cleanroom meets code editor. Every element has deliberate purpose. No decoration without function. The portfolio itself demonstrates the discipline it advertises — surgical precision, engineered confidence. The design is intentionally restrained: color appears only as signal, space is measured not accidental, typography carries hierarchy through weight not gimmick. The site's construction quality reflects the engineer's construction quality.

**Key Characteristics:**

- Deliberate, not decorated — every pixel has a reason
- Color as signal, not noise — green for trust, blue for depth
- Hierarchy through weight contrast — 400 vs 700, not size alone
- Depth through shadow, not flatness — offset + blur, never zero-offset glow
- Motion as state indicator — transitions signal changes, not delight
- Content-first — the interface recedes, the work speaks

## Colors

The palette is technical and calibrated — like instruments in a cleanroom. Greens signal trust and precision; blues provide depth and authority. Neutrals are faintly cool, not stark white.

### Primary

- **Calibrated Emerald** (#059669): Primary accent. Used for links, active states, theme color, social icon hover. Signals trust and precision.
- **Emerald Light** (#d1fae5): Light tint. Used for tag backgrounds, success states, subtle highlights.
- **Emerald Deep** (#047857): Darker variant. Used for hover states, emphasis on colored backgrounds.

### Secondary

- **Technical Blue** (#0284c7): Secondary accent. Used for links in prose, reference citations, secondary actions. Provides depth without competing with primary.
- **Blue Light** (#e0f2fe): Light tint. Used for info states, subtle highlights.
- **Blue Deep** (#0369a1): Darker variant. Used for link hover states.

### Neutral

- **Clean Paper** (#fafbfc): Page background. Faintly cool gray — like clean paper, not stark white.
- **Instrument Surface** (#f1f5f9): Card backgrounds, secondary surfaces. Slightly more contrast than background.
- **Precision Text** (#0f172a): Primary text. Deep slate for maximum authority and contrast.
- **Muted Readout** (#475569): Secondary text, metadata, dates. Darker than typical muted text for better readability.
- **Calibrated Border** (#e2e8f0): Borders, dividers, subtle structure. Like blueprint grid lines.

### Dark Mode

- **Deep Instrument** (#0b0e14): Page background. Near-black with slight blue undertone.
- **Dark Surface** (#131720): Elevated surfaces, cards. Slightly lighter than background.
- **Dark Card** (#161b24): Card backgrounds. Subtle lift from surface.
- **Bright Readout** (#e6e8ee): Primary text in dark mode. High contrast, easy to read.
- **Muted Dark** (#9aa3b2): Secondary text in dark mode. Reduced but still readable.
- **Faint Border** (rgba(255, 255, 255, 0.08)): Borders in dark mode. Subtle structure.

### Named Rules

**The Signal Rule.** Color appears only to communicate meaning — green for active/trust, blue for reference/depth. Decorative color is banned. If a colored element were made grayscale, its function should still be clear from position and weight.

**The Contrast Rule.** Body text maintains ≥4.5:1 contrast against its background. Large text maintains ≥3:1. On colored surfaces, tint secondary text from that hue — never gray.

## Typography

**Display/Body Font:** Inter (with system fallbacks)
**Mono Font:** JetBrains Mono (with monospace fallbacks)

**Character:** Inter is a neutral, geometric sans-serif designed for user interfaces. Using it for both display and body creates unity — the hierarchy comes from weight contrast (700 vs 400), not font family contrast. JetBrains Mono is a technical monospace designed for code, with ligatures and clear character distinction.

### Hierarchy

- **Display** (700, clamp(2rem, 5vw, 3.5rem), 1.1): Hero headlines, page titles. Maximum authority through weight, not decoration.
- **Headline** (600, clamp(1.25rem, 3vw, 1.75rem), 1.2): Section headings, card titles. Clear hierarchy from display.
- **Body** (400, 1rem, 1.6): Prose, descriptions, general content. Optimized for 45-75ch measure.
- **Label** (500, 0.875rem, 1.4, 0.02em tracking, uppercase): Metadata, dates, tags, navigation. Distinct from body through weight, size, and spacing.
- **Mono** (400, 0.875rem, 1.5): Code blocks, technical terms, data. JetBrains Mono for clarity.

### Named Rules

**The Weight Contrast Rule.** Hierarchy is primarily expressed through font-weight contrast, not size contrast. Display uses 700, body uses 400 — the gap is unmistakable. Size differences are moderate; weight differences are strong.

**The Mono Role Rule.** Monospace font appears only for code, data, or technical measurement. It never decorates "technical-looking" text that is actually prose or labels.

## Layout

The layout is structured and predictable — like an engineering document. Content flows linearly with clear section boundaries. The primary reading path is vertical: profile → news → latest posts → publications.

### Spacing

- **4px base scale:** All spacing is a multiple of 4px. This provides useful middle steps that an 8px-only scale misses.
- **Tight groups, generous separation:** Related content (date + title + description) uses 4-8px gaps. Distinct sections use 24-48px gaps.
- **More space above headings than below:** Section headings have more margin-top than margin-bottom, creating clear section boundaries.

### Grid

- **Max content width:** 65ch for prose (optimal reading measure)
- **Container:** Centered with responsive padding
- **Responsive:** Single column on mobile, two-column on desktop where appropriate

### Density

- **Moderate:** Not sparse (wastes space), not dense (overwhelms). Content density matches information value.
- **White space as precision:** Empty space is deliberate, not accidental. It signals that the layout was engineered, not assembled.

### Named Rules

**The Prose Measure Rule.** Body text stays within 45-75ch. Wider measures hurt readability; narrower measures waste space. The content area is constrained to maintain this range.

**The Grouping Rule.** Related content is grouped by proximity before adding containers or decoration. If two elements are close, they are related. If they are far, they are distinct.

## Elevation & Depth

The system uses soft shadows for depth — offset + blur, never zero-offset glow. Shadows signal state (hover, focus, elevation), not decoration.

### Shadow Vocabulary

- **Subtle** (`0 1px 2px rgba(0,0,0,0.12), 0 1px 3px rgba(0,0,0,0.08)`): Resting cards, inputs. Gentle lift from surface.
- **Medium** (`0 4px 16px -4px rgba(0,0,0,0.28), 0 2px 6px -2px rgba(0,0,0,0.12)`): Hovered cards, dropdowns. Active state indication.
- **Large** (`0 12px 40px -8px rgba(0,0,0,0.35), 0 4px 12px -4px rgba(0,0,0,0.15)`): Modals, elevated panels. High z-index surfaces.
- **Glow** (`0 0 0 1px rgba(0, 229, 153, 0.1), 0 4px 20px -4px rgba(0, 229, 153, 0.12)`): Theme-colored glow for focused/accent elements.

### Named Rules

**The Shadow State Rule.** Shadows appear as a response to state (hover, elevation, focus), not as a default decoration. Flat surfaces are flat at rest. Shadows indicate interaction or importance.

**The No-Glow Rule.** Zero-offset colored halos are decoration, not depth. Shadows must have a vertical offset to signal elevation. The glow token is reserved for accent emphasis, not general depth.

## Shapes

The form language is refined and consistent — not sharp (aggressive), not round (playful). Corners are gently curved at 8-16px radius.

### Radius Scale

- **Small** (8px): Tags, badges, small controls. Tight, precise.
- **Medium** (12px): Cards, inputs, dropdowns. Standard container radius.
- **Large** (16px): Profile image, modal containers. Generous, approachable.

### Named Rules

**The Radius Consistency Rule.** All containers of the same role use the same radius. Cards are always 12px. Tags are always 8px. Mixing radii within a role creates visual noise.

**The No-Pill Rule.** Pills (fully rounded corners) are reserved for small controls and tags. Cards, modals, and content containers never use pill radius — it undermines the engineered precision.

## Components

### Profile Image

- **Shape:** Rectangle with large radius (16px)
- **Shadow:** Medium shadow at rest, large on hover
- **Transition:** Subtle scale (1.02) and shadow change on hover
- **Purpose:** Professional headshot, not casual avatar

### Timeline Items (News, Latest Posts)

- **Shape:** No visible border. Background differentiation only.
- **Background:** Card color on page background
- **Shadow:** None at rest, medium on hover
- **Transition:** Subtle translate (-2px) and shadow on hover
- **Purpose:** Content cards, not decorative containers

### Social Icons

- **Size:** 48px touch target
- **Shape:** Circular with transparent background
- **States:** Opacity gate (0.6 default, 1.0 hover), scale on active
- **Purpose:** Contact actions, not decorative elements

### Section Headers

- **Accent:** 4px vertical bar with gradient (green → blue)
- **Typography:** Display weight (700), larger size
- **Spacing:** More margin-top (2.5rem) than margin-bottom (1.5rem)
- **Purpose:** Section boundaries, not decorative labels

### Date Badges

- **Shape:** Small radius (8px), surface background
- **Typography:** Mono font, small size, muted color
- **Purpose:** Metadata, not visual decoration

### Cards (CV sections, project cards)

- **Shape:** Medium radius (12px), card background
- **Shadow:** Subtle at rest, medium on hover
- **Border:** None (shadow provides depth)
- **Purpose:** Content containers, not decorative frames

## Do's and Don'ts

### Do:

- **Do** use weight contrast (400 vs 700) for hierarchy, not size alone
- **Do** keep prose within 45-75ch measure
- **Do** use shadows to indicate state (hover, focus), not decoration
- **Do** maintain 4.5:1 contrast for body text, 3:1 for large text
- **Do** group related content by proximity before adding containers
- **Do** use monospace font only for code, data, or technical measurement
- **Do** keep motion purposeful — transitions signal state changes, not delight
- **Do** theme browser surfaces (selection, scrollbars, focus rings) from the palette

### Don't:

- **Don't** use color decoratively — every colored element must communicate meaning
- **Don't** use zero-offset colored shadows as depth — that's glow, not shadow
- **Don't** use monospace font to make prose look "technical"
- **Don't** mix radius sizes within the same component role
- **Don't** add animation just to make polish visible
- **Don't** use gradient text — emphasis comes from weight or size
- **Don't** use hard offset shadows (4px 4px 0) outside neobrutalist contexts
- **Don't** add decorative borders above 1px on cards or list items
