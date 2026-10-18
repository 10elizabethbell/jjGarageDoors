---
name: J&J Garage Doors LLC
description: A family garage door crew's black-and-gold job flyer, made physical on a slate-night page.
colors:
  ground: "#1a2330"
  ground-2: "#202b3a"
  panel: "#273447"
  panel-hover: "#30405a"
  field-well: "#151d28"
  field-stroke: "#3a4a60"
  line: "rgba(242,239,230,.14)"
  ink: "#f4f1e8"
  ink-2: "#bcc5d2"
  placeholder: "#8794a6"
  gold: "#f3b324"
  gold-hover: "#ffc845"
  on-gold: "#1a2330"
  focus: "#8fd0ff"
  err: "#ffb4a6"
  slat-steel: "#5d6b7e"
  hem-black: "#1b2431"
  frame-white: "#d9dde3"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(40px, min(11.4vw, 17svh), 96px)"
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(34px, 9.5vw, 64px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(20px, 5.6vw, 26px)"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    lineHeight: 1.1
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 700
    lineHeight: 1.4
rounded:
  field: "8px"
  control: "10px"
  scene: "14px"
  round: "50%"
spacing:
  xs: "8px"
  sm: "14px"
  md: "22px"
  lg: "34px"
  xl: "56px"
  gutter: "18px"
  wrap: "1180px"
components:
  button-fill:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.on-gold}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "56px"
  button-fill-hover:
    backgroundColor: "{colors.gold-hover}"
    textColor: "{colors.on-gold}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "56px"
  button-line-hover:
    backgroundColor: "rgba(243,179,36,.12)"
    textColor: "{colors.ink}"
  chip:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "8px 15px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.on-gold}"
  input:
    backgroundColor: "{colors.field-well}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "12px 14px"
    height: "52px"
  row-arrow:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.round}"
    size: "42px"
  row-arrow-active:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.on-gold}"
  contact-tile:
    backgroundColor: "{colors.panel}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "60px"
  contact-tile-hover:
    backgroundColor: "{colors.panel-hover}"
  gold-panel:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.on-gold}"
    rounded: "{rounded.control}"
    padding: "18px"
    height: "76px"
---

# Design System: J&J Garage Doors LLC

## Overview

**Creative North Star: "The Flyer on the Driveway at Night"**

The page is J&J's own black-and-gold job flyer turned into a physical object: a stack of heavy uppercase slabs set on a slate-night ground, lit by one color, the logo gold. The material of the trade is the ornament. Section breaks are the bottom hem of a corrugated roll-up door (steel slats, a gold weather strip, a dark rubber seal, a center handle notch), the work photo is revealed by that same door rolling up, and the hero is a canvas garage door the visitor lifts with a finger, spilling warm light onto the driveway.

Density is phone-first and generous with touch: every interactive target clears 44px, primary actions are 56px tall, lists are full-bleed ruled rows rather than cards. Type does the heavy lifting; there are no illustrations beyond the door itself, no stock imagery, no icon cards. The page is bilingual English/Spanish, with both languages present in the markup and one shown at a time, so every component must hold either language's length.

The system font stack is a deliberate house rule set by the site's builder (Ellie) for pitch sites, not an oversight. The flyer voice comes from weight (900), caps, and tight negative tracking, never from a loaded face.

**Key Characteristics:**
- Slate-night ground, never pure black; warm-white ink; logo gold as the only accent fill.
- Heavy system caps (900, uppercase, negative tracking, line-height under 1) stacked like flyer type.
- Roll-up door material (corrugated slats + gold hem) as dividers and reveals.
- Full-bleed hairline-ruled lists instead of cards.
- Phone-first single column; desktop adapts at 1024px into two-column splits.
- Bilingual EN/ES throughout, toggled at the document root.

## Colors

One warm accent on a cool, deep slate: the palette of a lit garage seen from the street after dark.

### Primary
- **Logo Gold** (`gold`): the J&J brand gold. The only accent fill on the page: primary buttons, the selected chip, the Facebook panel, the active row arrow, phone numbers, the second line of the hero slab, the door hem strip, the mark, and the global focus outline. Hover lifts to **Hot Gold** (`gold-hover`). Text on gold is always slate (`on-gold`), never white.

### Secondary
- **Porch-Light Blue** (`focus`): a cool outline accent reserved for form controls (input and chip hover/focus borders, the chip "picked" pulse). It exists so a focus ring stays visible against a gold-filled control.

### Neutral
- **Slate Night** (`ground`): the page ground and `theme-color`. The driveway after dark.
- **Slate Lift** (`ground-2`): alternate section band (languages/family, quote form) for rhythm without borders.
- **Panel Slate** (`panel`, hover `panel-hover`): filled surfaces at rest: chips, row arrow discs, contact tiles.
- **Field Well** (`field-well`) with **Field Stroke** (`field-stroke`): text inputs sit darker than the ground, recessed, with a 2px stroke.
- **Warm White** (`ink`): primary text, warm rather than paper-white.
- **Cool Mist** (`ink-2`): secondary text, sub-lines, hints, the third language slab.
- **Hairline** (`line`): warm-white at 14% for row rules and the footer rule.
- **Placeholder Gray** (`placeholder`), **Soft Coral** (`err`): input placeholder and inline validation text.

### Door Material
- **Slat Steel** (`slat-steel`), **Hem Black** (`hem-black`), **Frame White** (`frame-white`): the roll-up door. Slats are a repeating gradient between slat steel tones; the hem is a gold strip over a hem-black seal; the work-photo bay is framed in frame white like a door opening.

### Named Rules
**The One Gold Rule.** Gold is the only accent fill. Any new emphasis, state, or badge uses gold or nothing; no second warm or saturated hue enters the page.

**The Never-Black Rule.** The darkest page surface is slate night (`ground`). Pure #000 is not a surface color; near-black values appear only inside the door material (seals, handle notch, lanterns).

**The Slate-on-Gold Rule.** Text and icons on a gold fill are always `on-gold` slate.

## Typography

**Display Font:** system UI stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** same stack

**Character:** One family, pushed to its heaviest weight and set in caps for anything structural; body copy stays at normal weight and sentence case. The contrast between 900-weight caps and 400-weight prose is the whole hierarchy.

### Hierarchy
- **Display** (900, clamp 40px to 96px with a 17svh cap, line-height 0.9, -0.03em, uppercase): the hero slab, two stacked lines, second line in gold. Desktop clamps to 56-86px. The closing "WE DO IT ALL." (up to 128px) and the three-language slab (up to 92px) are the same slab voice at larger sizes.
- **Headline** (900, clamp 34px to 64px, line-height 0.95, -0.02em, uppercase, balanced wrap): section headings.
- **Title** (800, clamp 20px to 26px, -0.01em, sentence case): service row text; the family statement (800, up to 40px, line-height 1.3) and step titles (900, 21px, uppercase) are its siblings.
- **Lead** (400, clamp 17px to 20px, line-height 1.45, max 34em, `ink-2`): the hero promise and section sub-lines (18px, max 36em).
- **Body** (400, 17px, line-height 1.55): running copy, capped near 34em.
- **Label** (800, 16-17px): buttons, form labels, contact names.
- **Small** (700, 15px): hints, notes, errors, footer.
- **Group label** (900, 15px, +0.1em, uppercase, gold): the heading over each service list group. The only positively tracked type on the page.

### Named Rules
**The Weight-Not-Face Rule.** The system stack is a house rule. Hierarchy comes from weight (400 / 800 / 900), caps, and size; never introduce a webfont to get "character".

**The Tight Caps Rule.** Structural headings are uppercase with negative tracking (-0.02em to -0.03em) and line-height at or below 0.95. Positive tracking is reserved for small gold group labels and the logo lockup.

**The Tabular Phone Rule.** Phone numbers use tabular numerals and gold (or inherit gold on hover).

## Layout

Phone-first single column inside a centered wrap (max 1180px, 18px side gutters that respect safe-area insets; 12px under 430px). Sections pad 56px top and bottom. The working spacing steps are 8, 14, 22, 34, and 56px, with 10/18/26px as in-between fits.

Rhythm comes from alternating bands (`ground` and `ground-2`) and from the door-hem dividers between major sections, not from borders or cards. Lists are full-bleed: hairline rule above the first row and under every row, 62px minimum row height.

The hero on phone: header, display slab, promise, a two-up button grid (stacks to one column under 360px), then the door scene bleeding to the screen edges and filling the remaining viewport height (clamp 250-420px).

At 1024px and up: the hero splits into copy and scene (about 1.02fr / 1fr, 56px gap) with the scene as a rounded 540px panel; service lists go two-column (56px column gap); the work section pairs photo and gold panel (1.6fr / 1fr); family, steps (three columns), contact tiles (three columns), and the form (two columns) widen. Breakpoints are 1024px for desktop, with phone-size refinements at 429px, 374px, and 359px, and a short-landscape rule (max-height 500px) that narrows the scene.

## Elevation & Depth

Flat by default. Surfaces separate by tone (ground, ground-2, panel, field well), not by shadow. Depth is reserved for the door material: the hem divider casts a soft shadow onto the section below as it drops in, and the slats carry their own shading in gradient. The hero scene's depth is painted (lit garage interior, light spill on the driveway, sconce glow), not layered UI.

### Shadow Vocabulary
- **Hem drop** (`box-shadow: 0 10px 18px -6px rgba(0,0,0,.55)`): only under the roll-up door hem divider.

### Named Rules
**The Only-the-Door-Casts Rule.** UI controls, tiles, and panels carry no shadow. Shadow belongs to the door object.

## Shapes

Gently rounded controls and straight-edged structure. Buttons, contact tiles, and the gold panel use a 10px radius; chips and text fields a slightly tighter 8px; the desktop hero scene a 14px panel radius. Row arrows are full circles. Headings, rows, bands, and the hem are square and full-width.

The work photo sits in a door bay: 6px top corners only, a 6px frame-white border on three sides, open at the bottom like a garage opening, 4:3. The door's center handle notch is the one bottom-rounded tab (4px). The mark is a miter-cornered house outline with a slatted door.

## Components

### Buttons
Big, blunt, thumb-sized.
- **Shape:** gently rounded (10px), 2px gold border on every variant, 56px minimum height.
- **Fill (primary):** gold with slate text, 800 weight 16px. Hover lifts to hot gold.
- **Line (secondary):** transparent with warm-white text and the gold border; hover tints with gold at 12%.
- **Press:** translates down 1px. Transitions 0.18s on color, 0.12s on transform.
- **Icon:** an optional 18px leading inline SVG (sms, phone).
- **Desktop:** buttons sit inline, padded 0 26px, at least 200px wide.

### Chips
Choice chips in the quote form (checkbox and radio both).
- **Style:** panel slate, 8px radius, 2px transparent border, 46px tall, 700 weight 16px.
- **Selected:** gold fill, slate text.
- **Hover / Focus:** border turns porch-light blue.
- **Picked pulse:** when a service row pre-selects a chip, the chip pulses (blue border, scale 1.04, 0.7s ease-out); disabled under reduced motion.

### Inputs / Fields
- **Style:** recessed field well, 2px field-stroke border, 8px radius, 52px min height, 500 weight 17px. Textarea 110px min, vertical resize.
- **Focus / Hover:** border turns porch-light blue; no glow.
- **Error:** soft coral 700-weight 15px message under the field, shown when the field is marked invalid.

### Navigation
A single header row, not a menu: gold house mark (40px; 34/30px on small phones) with "J&J" (900) over "GARAGE DOORS" (800, gold, tracked), the language toggle as an underlined text button in `ink-2`, and the main phone number right-aligned in 800 tabular figures with a gold phone glyph (glyph hidden under 430px). Every target is at least 44px.

### Service Rows
The signature list. Full-bleed rows ruled with hairlines, title-weight text left, a 42px panel-slate arrow disc right. On hover or focus the disc fills gold (focus adds the gold outline on the disc instead of the row). Each row links to the quote form and pre-selects the matching chip.

### Contact Tiles
Panel-slate tiles, 10px radius, 60px tall: a name in 800 left, the number in gold tabular figures right. Hover lightens to panel-hover. One per person; three columns on desktop.

### Gold Panel
The one large gold block (the Facebook link): gold fill, slate text in 900, icon left and arrow right on phone; on desktop it becomes a tall column with a 52px icon top and 40px arrow bottom, text at 30-40px.

### Roll-Up Door Hem (signature)
The section divider: a 64px window showing the bottom of a corrugated steel door (slats, a 4px gold strip, a 9px hem-black seal, a center handle notch), with near-black jamb edges. As it scrolls into view it rises 56px on a scroll-linked transform. Static under reduced motion.

### Photo Bay Reveal (signature)
The work photo sits in a door-opening frame; a roll-up door panel covers it and springs upward when 45% of the bay is visible. Without JS or under reduced motion the photo is simply shown.

### Garage Door Scene (signature)
The hero canvas: a sectional door at night between two lit sconces, on lap siding over a driveway. It lifts itself on a loop, can be dragged by touch or pointer, is a keyboard-operable vertical slider, spills warm light onto the driveway when open, and stops animating when off-screen. Hidden without JS.

## Do's and Don'ts

### Do:
- **Do** keep gold the only accent fill, with slate text on it.
- **Do** set structural headings in 900-weight uppercase with negative tracking and sub-1 line-height.
- **Do** use the system font stack; it is a house rule.
- **Do** keep every tap target at 44px or more and primary actions at 56px.
- **Do** write both `.en` and `.es` content for every visible string, and size components for the longer Spanish text.
- **Do** use the roll-up door hem between major sections and alternate `ground` / `ground-2` bands for rhythm.
- **Do** separate surfaces by tone; reserve shadow for the door material.
- **Do** give every motion a reduced-motion fallback that shows the end state.

### Don't:
- **Don't** use pure black as a page or section surface.
- **Don't** add a second accent hue or use porch-light blue as a fill; it is an outline color for form controls only.
- **Don't** put white text on gold.
- **Don't** turn service lists into icon cards, or add hero photos or testimonial carousels; the flyer world is type plus door material.
- **Don't** add drop shadows to buttons, chips, tiles, or panels.
