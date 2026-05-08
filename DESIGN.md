---
name: The Blonde Hedgehog
description: Michelin Key boutique hotel on Alderney, Channel Islands — warm, unhurried, genuinely remote.
colors:
  gold: "#B8965A"
  gold-light: "#D4AF7A"
  cream: "#F5F0E8"
  cream-dark: "#EDE6D6"
  ink: "#1A1A18"
  ink-soft: "#3a3a36"
  moss: "#2C3B2D"
  stone: "#8C7B6B"
  white: "#FDFCF9"
typography:
  display:
    fontFamily: "'Spectral', Georgia, serif"
    fontSize: "clamp(1.5rem, 2.8vw, 2.2rem)"
    fontWeight: 400
    lineHeight: 1.18
    letterSpacing: "normal"
  headline:
    fontFamily: "'Jost', system-ui, sans-serif"
    fontSize: "clamp(3rem, 5.5vw, 5.8rem)"
    fontWeight: 300
    lineHeight: 1.06
    letterSpacing: "-0.02em"
  title:
    fontFamily: "'Jost', system-ui, sans-serif"
    fontSize: "clamp(1.8rem, 3.5vw, 3rem)"
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  body:
    fontFamily: "'Jost', system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 300
    lineHeight: 1.6
    letterSpacing: "normal"
  label:
    fontFamily: "'Jost', system-ui, sans-serif"
    fontSize: "0.68rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.22em"
rounded:
  none: "0"
  soft: "12px"
  pill: "100px"
spacing:
  xs: "0.5rem"
  sm: "0.9rem"
  md: "2rem"
  lg: "4rem"
  section: "clamp(4rem, 8vw, 7rem)"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "0.9rem 2.2rem"
  button-primary-hover:
    backgroundColor: "{colors.gold-light}"
    textColor: "{colors.ink}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.white}"
    rounded: "{rounded.none}"
    padding: "0.9rem 2.2rem"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.gold}"
    rounded: "{rounded.none}"
    padding: "0.9rem 2.2rem"
  button-ghost-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
  nav-cta:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0.5rem 1.25rem"
---

# Design System: The Blonde Hedgehog

## 1. Overview

**Creative North Star: "The Warm Stone House"**

Not a hotel that impresses — a house that receives. The analogy is physical: walking into a well-loved granite building on the Atlantic edge of the Channel Islands, where the walls are honest, the light is warm, and no one is trying to perform hospitality at you. The design system inherits this quality. Space is used like silence in a good sentence: deliberately, because it earns its emptiness. Warmth comes from material choices — a brass-toned accent, linen-weight neutrals, a serif face that reads like handwriting — not from decoration.

The typographic system pairs Jost (a refined geometric sans, cool but not cold) with Spectral (a screen-optimised classical serif, warm and slightly literary). Jost carries the structural weight: headings, navigation, labels. Spectral carries the emotional weight: italic emphasis, pull quotes, card titles, the scrub quotation. The pairing creates the core brand tension — structured but not corporate, warm but not cosy.

Color is restrained-to-committed. The cream-and-ink base accounts for the majority of every surface. Harbour Brass (the gold accent) appears at decision points: CTAs, active states, eyebrow labels, the scroll indicator. It is never used decoratively. The Island Moss surface appears once — the CTA section — as a distinct tonal register that signals arrival and action.

This system explicitly rejects: the conventions of generic hotel chains (Marriott / Hilton corporate templates); over-designed boutique-hotel sites that announce themselves with black-heavy maximalism; quaint British B&B aesthetics with floral ornament and dated warmth; and the hero-metric template (big number + small label grid) that is the cliché of every SaaS-adjacent hospitality brand. If the design could belong to any hotel, it has failed.

**Key Characteristics:**
- Linen-weight neutrals as the ambient surface; ink as deep structure; brass as the single voice
- Two-family type system: geometric sans for structure, classical serif for emotion
- Sharp-cornered components (zero radius on buttons and cards) — confidence, not softness
- Sections breathe at section-level spacing; components are tight within sections
- Motion is choreographed but unhurried: ease-drawer for accordions, ease-out-expo for reveals

## 2. Colors: The Island Palette

A committed palette centered on warm neutrals with a single brass accent. Depth is tonal, not shadow-heavy.

### Primary
- **Harbour Brass** (`#B8965A` / `oklch(65% 0.095 70)`): The single voice of the brand. Used for CTAs, active nav states, eyebrow labels, focus rings, the scroll indicator, card category tags, and internal text links. Never decorative. Its rarity is the point — every instance carries weight.
- **Morning Brass** (`#D4AF7A` / `oklch(75% 0.088 75)`): Warmer, lighter variant of Harbour Brass. Used for italic emphasis in display headings (`h1 em`, `h2 em`), button hover states. Softer presence than the primary accent.

### Secondary
- **Island Moss** (`#2C3B2D` / `oklch(24% 0.035 145)`): The CTA section background — the only green surface on the entire homepage. Signals destination and action. Not used elsewhere.

### Neutral
- **Warm Island Linen** (`#F5F0E8` / `oklch(95% 0.012 80)`): Primary page background. Never pure white — the slight warmth is the point.
- **Sun-Faded Linen** (`#EDE6D6` / `oklch(91% 0.018 80)`): Slightly denser cream. Available for tonal separation within cream surfaces.
- **Bleached Cotton** (`#FDFCF9` / `oklch(99% 0.004 80)`): Used for text on dark surfaces and as the lightest available near-white. Never `#fff`.
- **Night Harbour** (`#1A1A18` / `oklch(13% 0.004 100)`): Primary dark. Hero background, footer, bento cell gap fill, nav, scrub section. Never `#000`.
- **Dusk Slate** (`#3a3a36` / `oklch(25% 0.006 100)`): Soft dark, available for nested dark surfaces.
- **Saltstone** (`#8C7B6B` / `oklch(55% 0.028 55)`): Muted warm gray-brown. Gallery captions, secondary body copy, section lead text on dark backgrounds.

### Named Rules
**The Brass Scarcity Rule.** Harbour Brass appears on ≤10% of any given surface. When it appears everywhere, it means nothing. Guard it: CTAs, labels, and active states only — never as a background fill outside the nav CTA pill.

**The No-White Rule.** Pure `#fff` and `#000` are prohibited. Every neutral is tinted warm toward the brand hue. The coldest white in the system is `#FDFCF9`; the deepest ink is `#1A1A18`.

## 3. Typography

**Display Font:** Spectral (with Georgia, serif fallback) — a screen-optimised classical serif designed for editorial use. Used exclusively for emotional weight: italic emphasis phrases within headings, card titles, pull-quote sections, footer brand name.

**Body / Structure Font:** Jost (with system-ui, sans-serif fallback) — a refined geometric sans. Used for all structural elements: page headings, navigation, body copy, labels, buttons.

**Character:** The pairing is deliberately asymmetric. Jost is the architecture; Spectral is the warmth. Italic Spectral phrases embedded inside Jost headlines (the `em` pattern throughout the system) create a hospitality signature — structured but personal, like a handwritten note on fine stationery.

### Hierarchy
- **Headline** (Jost 300, `clamp(3rem, 5.5vw, 5.8rem)`, lh 1.06, ls -0.02em): Page-level hero headings. Paired with italic Spectral `em` for emotional emphasis in Morning Brass.
- **Display** (Spectral italic 400, `clamp(1.5rem, 2.8vw, 2.2rem)`, lh 1.18): Card titles, pull-quote sections, footer brand name. Spectral in roman weight is also used for the scrub quote at `clamp(1.6rem, 3.8vw, 3rem)`.
- **Title** (Jost 300, `clamp(1.8rem, 3.5vw, 3rem)`, lh 1.15, ls -0.01em): Section-level headings (bento header, accordion header, CTA heading). May include italic Spectral `em` for moss-colored emphasis.
- **Body** (Jost 300, 1rem, lh 1.6–1.7): Long-form copy. Maximum line length 65ch (achieved via `max-width` constraints). Never exceed 75ch.
- **Small Body** (Jost 300–400, 0.82–0.86rem, lh 1.5–1.7): Card body copy, footer paragraphs, gallery captions.
- **Label** (Jost 500–600, 0.62–0.72rem, ls 0.14–0.28em, uppercase): Eyebrow labels, nav links, button text, category tags, the vertical accordion labels. Always uppercase. Decorative lines (1px solid Harbour Brass, 18–24px wide) flank labels that sit alone (eyebrow, scrub section).

### Named Rules
**The Italic Emphasis Rule.** Spectral italic is the only permitted emphasis pattern within Jost headlines. No bold, no underline, no color shift without the Spectral face. When a heading gets an emotional beat, it gets Spectral italic in Morning Brass.

**The Weight Discipline Rule.** Display and body headings are weight 300 — not medium, not bold. The system's authority comes from scale and spacing, not weight. Reserve weight 500–600 for labels and micro-copy only.

## 4. Elevation

This system is flat by default with tonal layering. Surfaces separate by color value, not by cast shadow. The Night Harbour ink backdrop of the bento grid (visible as the 3px gap between cells) acts as a pseudo-shadow — depth through color, not geometry.

Shadows exist only as functional responses to state, never as ambient decoration:

### Shadow Vocabulary
- **Nav ambient** (`0 4px 32px rgba(0,0,0,0.35)`): Applied to the floating pill nav to separate it from variable hero content beneath. Fixed; does not change on interaction.
- **CTA button glow** (`0 8px 32px rgba(184,150,90,0.4)`): Appears on `.btn-primary:hover`. A warm Harbour Brass diffusion that confirms the primary action. Only on hover — not at rest.
- **Focus ring halo** (`0 0 0 4px rgba(184,150,90,0.2)`): Accompanies the 2px Harbour Brass `:focus-visible` outline on buttons. Provides adequate glow without visual noise at rest.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest. Shadows appear only as a response to state or to physically separate a floating element from the page. A card at rest has no shadow. A button at rest has no glow. Decoration earns its presence through interaction.

## 5. Components

### Buttons
Assured and unhurried. Sharp corners signal confidence; the subtle shimmer and vertical lift on hover signal responsiveness without urgency.

- **Shape:** No border radius (0px) — the sharp corner is a deliberate brand statement.
- **Anatomy:** All buttons share: 0.76rem Jost 600 uppercase text, ls 0.14em; padding 0.9rem 2.2rem; a full-coverage shimmer overlay (`rgba(255,255,255,0.11)`) that slides in from the left on hover; `translateY(-2px)` lift on hover; `scale(0.97)` depression on `:active`.
- **Primary** (`btn-primary`): Harbour Brass background, Night Harbour text. On hover: Morning Brass background, CTA glow shadow. The definitive action.
- **Outline** (`btn-outline`): Transparent background, Bleached Cotton text, 1px semi-transparent white border (`rgba(253,252,249,0.45)`). Used on dark/hero surfaces. Border strengthens to full white on hover.
- **Dark** (`btn-dark`): Night Harbour background, Bleached Cotton text. Used on cream surfaces as a secondary CTA.
- **Ghost** (`btn-ghost`): Transparent background, Harbour Brass text, 1px Harbour Brass border. On hover: fills to Harbour Brass background with Night Harbour text. Used for tertiary/enquiry actions.
- **Focus:** 2px Harbour Brass outline, 3px offset, accompanied by the focus ring halo shadow. Never color-only.
- **Nav CTA pill** (`nav-cta`): An exception — 100px radius pill, Harbour Brass background, Night Harbour text, smaller padding. Follows pill nav aesthetic. Not a general button variant.

### Cards / Bento Containers
- **Corner Style:** No border radius — all cells are sharp-cornered.
- **Background:** Night Harbour as base fill for the bento grid container; individual cells are image-filled with gradient overlays.
- **Shadow Strategy:** None at rest. The 3px Night Harbour gap between cells provides depth.
- **Grid gap as ink:** `gap: 3px; background: var(--ink)` on the grid container — the gap reveals the ink background, acting as a physical divider without explicit borders.
- **Image hover:** `scale(1.06)` with `filter: brightness(0.8)` at 0.9s ease-out. The slow timing matches the unhurried brand.
- **Content overlay:** `linear-gradient(to top, rgba(26,26,24,0.92) 0%, rgba(26,26,24,0.15) 55%)` — deep at the bottom, transparent at the top.
- **Internal padding:** `clamp(1.2rem, 2.5vw, 2rem)` — generous within the content area.

### Navigation
- **Style:** Floating pill nav, fixed at top center. Night Harbour background at 97% opacity (no backdrop-filter — solid surface). 1px `rgba(255,255,255,0.07)` border. `0 4px 32px rgba(0,0,0,0.35)` ambient shadow.
- **Logo:** Spectral 500 at 0.9rem. Harbour Brass on hover.
- **Links:** Jost 500, 0.72rem, uppercase, ls 0.1em. 70% white at rest; full white with a `rgba(255,255,255,0.07)` background fill on hover. Harbour Brass for active state.
- **Dropdowns:** 12px radius container, Night Harbour solid background, 1px faint border. Items reveal with `opacity + translateY(6px)` at 0.2s ease-out. Scale from top-left transform origin.
- **CTA:** Nav CTA pill (see Buttons — Nav CTA pill variant).
- **Mobile:** Full-screen overlay at 100vw/100vh. Spectral italic links at `clamp(1.5rem, 4vw, 2.2rem)`. Hamburger toggle with animated bars.

### Horizontal Accordion
A signature component of the system — the primary rooms/experiences browser.

- **Mechanism:** Flex items with `flex: 1` default and `flex: 5.5` on hover. Transition at 0.75s with the ease-drawer curve (`cubic-bezier(0.32, 0.72, 0, 1)`). Collapsed items show a rotated 90° vertical label.
- **Image treatment:** `filter: brightness(0.6)` at rest; `scale(1.04) + brightness(0.42)` on hover (darkens to read white content clearly).
- **Content reveal:** `.acc-desc` and `.acc-link` are `opacity: 0, translateY(8px)` at rest; animate in at 0.4s with staggered delay (0.32s and 0.45s) on hover. On mobile: both are fully visible by default.
- **Mobile override at 640px:** Stack vertically (`flex-direction: column`), all items `height: auto`, images fixed at 200px height, content always visible.

### Gallery (GSAP Scroll Section)
- **Mechanism:** Pinned left column (sticky section heading + supporting copy) while right column scrolls. Images animate from `scale(0.8)` at entry to `scale(1.0)` at center and fade out with `opacity: 0.2` + `scale(0.95)` at exit. Controlled by ScrollTrigger scrub.
- **Layout:** 1fr / 1.6fr grid column split. Gallery images use `aspect-ratio: 16/11`.
- **Captions:** Saltstone, 0.68rem, ls 0.16em uppercase. Prefixed with a 18px Harbour Brass hairline.

### Text Scrub Section
- **Background:** Night Harbour — the only full-bleed dark section outside the footer.
- **Mechanism:** Spectral italic quote text split into individual word `<span>` elements. GSAP scrubs opacity from 0.15 → 1 as the user scrolls. CSS base color is `rgba(253,252,249,0.85)` as a readable fallback if GSAP fails.
- **Cite line:** Fades in via `.visible` class once the full quote has been read.

## 6. Do's and Don'ts

### Do:
- **Do** use Spectral italic exclusively for emotional emphasis phrases inside Jost headlines — the `em` pattern is the brand's typographic handshake.
- **Do** keep Harbour Brass (`#B8965A`) to ≤10% of any surface. Use it for CTAs, active states, labels, and focus rings only.
- **Do** use sharp corners (0 border radius) on all buttons and content cards. The no-radius decision is intentional brand confidence, not an oversight.
- **Do** write section spacing generously: `clamp(4rem, 8vw, 7rem)` or larger. Sections are cinematic chapters, not adjacent boxes.
- **Do** use the bento grid's 3px Night Harbour gap as the visual divider. Do not add additional card borders or drop shadows.
- **Do** prefix all focus states with `:focus-visible`, never `:focus`. Provide both outline and glow for buttons.
- **Do** guard the `prefers-reduced-motion` media query for all transitions, animations, GSAP blocks, and scroll effects.
- **Do** use `clamp()` for all display and title font sizes. Every size that matters should be fluid between its minimum and maximum.
- **Do** tint every neutral toward the brand hue — never pure `#fff` or `#000`.

### Don't:
- **Don't** use backdrop-filter or glassmorphism anywhere — not on the nav, not on overlays, not on card overlays. The nav uses a solid 97% opacity background. This is deliberate.
- **Don't** use gradient text (`background-clip: text` with gradient). Emphasis is weight, scale, and Spectral italic — never a gradient fill.
- **Don't** use the hero-metric template: big number + small label in a 3–4 column stats grid. This is explicitly prohibited as a SaaS cliché that undermines the Michelin Key brand.
- **Don't** place a credentials ticker or auto-scrolling marquee anywhere on the site. "Where the island slows everything down" cannot be followed immediately by a fast-scrolling badge strip.
- **Don't** use side-stripe borders (`border-left` or `border-right` > 1px as a colored accent). Rewrite with background tints or full borders.
- **Don't** use generic hotel chain layout conventions: Marriott/Hilton corporate templates, identical icon + heading + text card grids, stock photography that could be any hotel.
- **Don't** design toward an over-designed boutique hotel aesthetic: black-heavy, serif-maximalist, editorial overload, design that announces itself before the place does.
- **Don't** drift toward quaint British B&B aesthetics: floral patterns, cottage-cosy warmth, small-scale intimacy, dated serif-heavy headlines.
- **Don't** animate CSS layout properties (`height`, `width`, `padding`, `margin`). Only `transform` and `opacity` — GPU only.
- **Don't** use Playfair Display or Outfit. Both are training-data reflexes for luxury/boutique hotel UI. Spectral and Jost are the system's type voices; no third face is needed.
- **Don't** add badge overlays or floating stamp icons onto hero imagery. The hero communicates through the image itself and the headline — not through credential tags pinned to the photo.
