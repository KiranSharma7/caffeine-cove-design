---
name: Caffeine Cove
description: Warm light in a dark room. A specialty café site lit like its own cove ceiling.
colors:
  dark-roast: "#1C0F0A"
  crema: "#F6EDE1"
  cove-glow: "#E3A24C"
  cove-glow-bright: "#EDB466"
  # planned: specified in caffeine-cove-landing-brief.md, not yet in styles.css
  latte: "#EDE3D6"
  marigold: "#F3B457"
  logo-espresso: "#54160B"
  plate-blue-pale: "#BFDDF2"
typography:
  display:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "clamp(3rem, 7.4vw, 8.5rem)"
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: "-0.03em"
    fontVariation: "\"SOFT\" 100"
  headline:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "2.6rem"
    fontWeight: 400
    lineHeight: 1.15
    fontVariation: "\"SOFT\" 100"
  title:
    fontFamily: "Fraunces, Georgia, serif"
    fontSize: "clamp(1.25rem, 1.6vw, 1.6rem)"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "-0.015em"
    fontVariation: "\"SOFT\" 100"
  body:
    fontFamily: "Figtree, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "clamp(1.05rem, 1.4vw, 1.375rem)"
    fontWeight: 400
    lineHeight: 1.4
  label:
    fontFamily: "Figtree, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 500
  label-strong:
    fontFamily: "Figtree, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "1rem"
    fontWeight: 600
rounded:
  pill: "999px"
  circle: "50%"
  # planned frames (brief): tiles 20px, feature cards and video 28px
  tile: "20px"
  frame: "28px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "40px"
  gutter: "clamp(16px, 3.9vw, 72px)"
  bar-height: "60px"
components:
  button-primary:
    backgroundColor: "{colors.crema}"
    textColor: "{colors.dark-roast}"
    typography: "{typography.label-strong}"
    rounded: "{rounded.pill}"
    padding: "0 8px 0 26px"
    height: "52px"
  button-primary-arrow:
    backgroundColor: "{colors.dark-roast}"
    textColor: "{colors.crema}"
    rounded: "{rounded.circle}"
    size: "36px"
  button-primary-arrow-hover:
    backgroundColor: "{colors.cove-glow}"
    textColor: "{colors.dark-roast}"
  button-link:
    textColor: "{colors.crema}"
    typography: "{typography.label-strong}"
    height: "44px"
  call-button:
    backgroundColor: "{colors.cove-glow}"
    textColor: "{colors.dark-roast}"
    rounded: "{rounded.circle}"
    size: "44px"
  call-button-hover:
    backgroundColor: "{colors.cove-glow-bright}"
  header-bar:
    textColor: "{colors.crema}"
    rounded: "{rounded.pill}"
    padding: "0 8px 0 20px"
    height: "{spacing.bar-height}"
  nav-link:
    textColor: "{colors.crema}"
    typography: "{typography.label}"
    padding: "10px 0"
  mobile-call-pill:
    backgroundColor: "{colors.cove-glow}"
    textColor: "{colors.dark-roast}"
    typography: "{typography.label-strong}"
    rounded: "{rounded.pill}"
    padding: "14px 22px"
---

# Design System: Caffeine Cove

## Overview

**Creative North Star: "The Lit Cove"**

Caffeine Cove is named for, and built inside, a room of curved bulkheads with warm LED light hidden in the coves. The site works the same way. Most of each surface is dark roast, and light comes through it: amber on the one word that matters, crema on the type, and a glowing photo of the counter. Nothing is lit evenly. Every screen should feel like walking in from a bright shopping-centre corridor to somewhere warmer and softer.

The type is a soft, round-shouldered serif (Fraunces with its SOFT axis at full) set large and tight, paired with a plain, friendly sans for everything functional. Forms are fully rounded pills and circles, like the curved ceilings. Edges between sections are hand-made rather than ruled: the hero ends in a torn cream brush stroke, not a straight line. Density is low. One headline, one line of fact and two actions is a complete hero.

The brand is premium but friendly, never stuffy. Craft shows in small exact things: concentric radii, a 3px arrow nudge on hover, a staged 100ms entrance. It never shows in ornament.

**Key Characteristics:**
- Dark-roast base with light coming through; amber is the light source, used sparingly.
- Soft serif display (Fraunces SOFT 100) over a quiet Figtree UI.
- Pills, circles and concentric radii; no sharp corners on interactive elements.
- Torn-paper and brush transitions instead of hard section rules.
- Real photography of the room and the food carries the colour; the UI stays warm-neutral.

## Colors

A warm, low-key palette of roasted browns and milky creams, with one amber glow.

### Primary
- **Cove Glow** (`cove-glow`): the light in the room. The italic accent word in a headline ("*belong.*"), the call button, the mobile call pill, the arrow-circle hover and the focus ring. It never fills a large area.
- **Cove Glow Bright** (`cove-glow-bright`): hover state for Cove Glow fills only.

### Secondary (planned)
- **Marigold** (`marigold`): the one saturated panel on the page, used for the product spotlight. Text on it is Logo Espresso.
- **Plate Blue, pale** (`plate-blue-pale`): only as the backdrop of the spotlight photo card, where it echoes the café's cobalt plates. Nowhere else in the UI.

### Neutral
- **Dark Roast** (`dark-roast`): page background, the hero shade gradients, button text on light fills, the frosted header glass (at 42% opacity) and the mobile nav sheet (97%).
- **Crema** (`crema`): display type and primary text on dark, the primary button fill, and the cream sections that follow the hero (the brush edge is painted in it).
- **Crema Soft** (Crema at 84%): secondary text on dark, i.e. the lede and nav links at rest.
- **Latte** (`latte`, planned): tile and panel fill inside cream sections (e.g. menu grid tiles).
- **Logo Espresso** (`logo-espresso`, planned): heading colour on cream and marigold surfaces. Taken from the logo's inner ring.

### Named Rules
**The One Lamp Rule.** Cove Glow is the light source, so there is one per view: one accent word, one call button, one focus ring. If two amber things compete, one of them goes crema.

**The Plates Carry the Blue Rule.** Cobalt blue appears through food photography only. The single UI exception is the pale-blue spotlight card backdrop.

**The Roast-and-Crema Rhythm.** Sections alternate dark roast and crema (with marigold once). Never put two adjacent sections in the same tone without a deliberate divider.

## Typography

**Display Font:** Fraunces (with Georgia, serif), SOFT axis 100
**Body Font:** Figtree (with system-ui, -apple-system, Segoe UI, sans-serif)

**Character:** Fraunces at full softness feels like a warm, slightly old-fashioned café sign. The rounded terminals keep it from becoming stately. Figtree is plain and approachable and keeps out of the way, so prices, hours and buttons read instantly for every age.

### Hierarchy
- **Display** (400, clamp(3rem → 8.5rem), line-height 0.95, -0.03em): hero headline only. One italic word in Cove Glow carries the emotion (tracking eases to -0.02em on the italic). On phones, clamp(3rem, 16.5vw, 5rem).
- **Headline** (400, 2.6rem, line-height 1.15): mobile navigation links. This is the reference size for section headings to come.
- **Title** (500, clamp(1.25rem → 1.6rem), line-height 1, -0.015em): the "Caffeine Cove" wordmark in the header.
- **Body** (400, clamp(1.05rem → 1.375rem), line-height 1.4): hero lede and lead paragraphs, in Crema Soft on dark. Keep running text to 65–75ch.
- **Label** (500, 0.9375rem): navigation links.
- **Label Strong** (600, 1rem): button and link text.

### Named Rules
**The Soft Serif Rule.** Every Fraunces instance sets `font-variation-settings: "SOFT" 100`. A sharp Fraunces is a different brand.

**The One Italic Rule.** A display line gets at most one italic word, and it is the word that carries the feeling ("belong", "fancy").

**The Prices Are Text Rule.** Prices, hours and addresses are live Figtree text, never baked into images.

## Layout

One shared container aligns the header bar, the hero copy and every section: `min(1320px, 100% − 2 × gutter)`, with a fluid gutter (16px on phones, up to 72px). The header floats over the hero with a fluid top inset (12–28px) and a fixed 60px bar height.

The hero is full-bleed and full-height (100svh, capped at 1080px). Copy is anchored bottom-left, clear of both the header and the brush edge (whose height is `max(48px, 9.5vw)`, or 60px on phones). The photo crops toward the counter and barista (object-position 60–62%).

Spacing steps of 8 / 16 / 24 / 32 / 40px. Vertical gaps between content blocks use fluid clamps (e.g. 18–28px below the title, 28–44px above the actions).

Breakpoints: at **960px** the desktop nav collapses into a toggle and a full-screen sheet; at **720px** the bar and mark tighten, the shade switches from a left-and-bottom wash to a vertical one, and the display size switches to the vw-based phone clamp.

## Elevation & Depth

Depth comes from light and layering, not stacked cards. The hero builds depth with photography under dark-roast gradient shades (left wash, bottom wash, top vignette). The header is the one frosted surface: Dark Roast glass at 42%, `blur(16px) saturate(140%)`, a 1px crema hairline and a soft drop shadow. Elsewhere, surfaces are flat at rest.

### Shadow Vocabulary
- **Floating bar** (`0 1px 0 rgba(255,255,255,0.04) inset, 0 10px 30px -12px rgba(0,0,0,0.45)`): the glass header only.
- **Lift on hover** (`0 12px 30px -8px rgba(0,0,0,0.5)`): primary button on pointer hover.

### Named Rules
**The Flat-at-Rest Rule.** Shadows only appear as a response to hover, or on the single floating header. Cards and tiles sit flat on their section colour.

## Shapes

The form language follows the curved bulkhead ceilings. Every interactive element is a full pill (999px) or a circle (50%). Nested shapes are concentric: the 52px primary pill holds a 36px circle inset 8px (26 = 18 + 8), and the 60px header bar holds 44px buttons with an 8px end inset. The focus ring follows the pill shape.

Image frames and tiles (planned) use large radii: 20px on menu tiles and 28px on feature cards and the video frame. Section transitions are organic: the cream brush-stroke edge (`assets/hero/brush-edge.webp`) and, per the brief, at most one curved divider elsewhere.

## Components

### Buttons
Soft and tactile: fully round, a small press-in on tap, and lift only on hover.
- **Shape:** full pill (999px); icon buttons are 44px circles.
- **Primary:** Crema pill, 52px tall, Dark Roast Label Strong text, with a trailing 36px Dark Roast circle holding an arrow. Padding 26px at the start and 8px at the end, so the circle sits concentric.
- **Hover (pointer only):** the button lifts with a soft shadow, the arrow circle turns Cove Glow, and the arrow nudges 3px right (200ms, ease-out-soft).
- **Active:** scale 0.96 (150ms ease-out).
- **Link button:** Crema text with a trailing arrow and a 44px minimum height; the arrow nudges 3px on hover. Use it as the secondary action next to a primary.
- **Call button:** 44px Cove Glow circle with a Dark Roast phone glyph; it turns Cove Glow Bright on hover and scales to 0.96 when pressed.

### Navigation
- **Header bar:** a floating frosted pill on the shared container, laid out on a three-column grid: brand left, nav centred, actions right.
- **Links:** Figtree 500 at 0.9375rem in Crema Soft. On hover the text turns full Crema and a 1px underline draws in from the left (300ms ease-out-soft).
- **Mobile (≤960px):** a 44px circular toggle (glass tint, hairline border) whose two 1.5px lines morph into an X. It opens a full-screen Dark Roast sheet (97%) with links in Fraunces Headline and a Cove Glow call pill. The header stays fixed while the sheet is open, and Escape closes it.

### Hero (signature)
A full-bleed room photo, darkened toward the copy, with the headline bottom-left and a cream brush edge pouring into the next section. The entrance staggers title, lede and actions 100ms apart (300ms: fade, 4px blur and a 12px rise). Under reduced motion it is a plain fade.

### Brush Edge (signature)
A torn cream paint stroke, 2400 × 332, stretched to the full width at a slightly flatter height. It is the transition from a dark section into a crema one. Clear its tallest shoulder before placing copy.

## Do's and Don'ts

### Do:
- **Do** keep one Cove Glow element per view: the accent word, the call button or the focus ring.
- **Do** set every Fraunces instance with `"SOFT" 100`.
- **Do** make nested rounded shapes concentric (outer radius = inner radius + inset).
- **Do** use the shared container for every section, so edges line up with the header bar.
- **Do** keep hover effects behind `@media (hover: hover)` and give every animation a reduced-motion fallback.
- **Do** keep touch targets at 44px or more.
- **Do** alternate dark-roast and crema sections, with marigold used once.

### Don't:
- **Don't** use cobalt or plate blue as a UI colour. The only exception is the pale-blue spotlight card backdrop.
- **Don't** use sharp corners on buttons, toggles or chips.
- **Don't** add shadows to surfaces at rest; the header is the only floating element.
- **Don't** set more than one italic word in a display line.
- **Don't** switch the display or UI faces. DM Serif Display and Manrope in the landing brief are superseded by Fraunces and Figtree.
- **Don't** put prices, hours or the address inside images.
