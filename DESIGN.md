---
name: J&J Garage Doors LLC
description: A family garage-door crew from Elizabeth, NJ, in calm paper-and-navy bands with the logo's gold as the one warm accent.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0d2138"
  body: "#2a3a4c"
  soft: "#4a5868"
  navy: "#183a63"
  deep: "#0d2138"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d4e3"
  gold: "#f3b324"
  gold-2: "#ffc845"
  gold-ink: "#7a5400"
  line: "rgba(13,33,56,.12)"
  focus: "#1f5fa8"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 78px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "20px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: ".02em"
rounded:
  field: "10px"
  row: "18px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-xs: "12px"
  gutter-sm: "16px"
  gutter: "20px"
  gutter-lg: "40px"
  gap-sm: "10px"
  gap-md: "16px"
  gap-lg: "24px"
  section: "64px"
  section-lg: "96px"
  wrap: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  service-row:
    backgroundColor: "rgba(255,255,255,.06)"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "10px 12px 10px 22px"
    height: "64px"
  arrow-circle:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    size: "44px"
  arrow-circle-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
  input-field:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  step-number:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
  eyebrow:
    backgroundColor: "rgba(13,33,56,.06)"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "9px 14px"
---

# Design System: J&J Garage Doors LLC

## Overview

**Creative North Star: "The Calm Band"**

The page is a stack of full-bleed bands that alternate off-white paper with two night navies, so each new section is obvious without rules or boxes. One of J&J's own job photos (two black doors on a gray house) sits under a navy overlay in the hero. The logo's gold is the only warm colour on the page. It is a fill: buttons, the arrow circle on hover, step numbers, the floating text circle. Almost everything is borderless and softly rounded. Depth comes from moving between bands, not from shadows.

The tone is a family crew that takes its time. One webfont (Cal Sans) handles every heading and every tappable label, the system stack carries running text at a relaxed 16/1.7, and motion appears only twice: the hero headline bounces in letter by letter, and content below the first screen rises 12px as it arrives. The page is bilingual (English and Spanish) as a whole: both languages are in the markup, and one attribute on `<html>` decides which is shown.

This is the pitch-site house "calm band style" (after lpmr.co.uk), using this client's logo colours and photo. An earlier liftable-door world for this project is retired and is in git history only. Don't mix the two.

**Key Characteristics:**
- Full-bleed bands in this order: paper header, photo hero, paper, navy, paper, deep navy with line texture, paper, navy, deep footer.
- Gold is used as a fill. On light ground, gold as text is the darker gold-ink.
- Cal Sans 400 for headings and tappable labels (buttons, rows, field labels, phone numbers); system sans for body text.
- Borderless soft shapes: 24px cards, 18px rows, 10px fields, full pills.
- Flat surfaces. The only shadow is on the floating text circle.
- Two motions: the hero H1 letter bounce-in and a 12px fade-up. Both are off under reduced motion and without JS.

## Colors

Cool paper and two night navies, with one warm accent taken from J&J's logo gold.

### Primary
- **Logo Gold** (gold): the brand's one warm accent, used only as a fill: primary buttons, the arrow circle on hover, step numbers, the floating text circle, the eyebrow dot, `::selection`, and the house-mark strokes. On dark bands it is also the colour of the accent phrase in a heading and of icon glyphs (Facebook mark, phone icon). Text on a gold fill is always Ink.
- **Bright Gold** (gold-2): hover state of the primary button only.
- **Gold Ink** (gold-ink): gold as text or line-icon colour on light ground (6.3:1 on paper). Used for the accent phrase in headings on paper, the claims icons, the header phone icon and the hover colour of the header number.

### Secondary
- **Night Navy** (navy): the mid band (services, close), the work photo's placeholder ground and the Facebook row.
- **Deep Navy** (deep): the hero base and overlay tint, the "How it works" band and the footer. Both of these carry the diagonal line texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`). Same value as Ink, but a separate token because its job is different.

### Tertiary
- **Form Blue** (focus): the one outline colour for the form. Text fields and chips get it on hover and focus, the submit button gets it as an outline, and it is also the global `:focus-visible` ring on light ground and the input caret. It is kept separate from gold on purpose, because gold is the button fill.
- **Signal Red** (error): inline error sentences and the border of a field with an error.

### Neutral
- **Paper** (paper): page ground, header, light bands. Also `theme-color`.
- **Card White** (card): the quote form card.
- **Field Tint** (field): fill for text inputs and choice chips on the white form card. It is a tint, not a contrast boundary (about 1.2:1 against white). Fields are identified by their labels and the blue hover/focus outline.
- **Ink** (ink): headings and labels on light ground, text on gold, the selected chip fill, the house-mark tile.
- **Body Slate** (body): running text on light ground.
- **Soft Slate** (soft): ledes, secondary text, placeholders, the language toggle, the small "Garage Doors LLC" line.
- **On-Dark** (on-dark): headings and links on navy bands.
- **On-Dark Soft** (on-dark-soft): running text on navy bands.
- **Hairline** (line): the 1px divider between claims.

### Named Rules
**The Gold Is a Fill Rule.** Gold (#f3b324) appears as a fill with Ink text on it. On light ground it never appears as text. Use Gold Ink there. On navy it may colour an accent phrase or a glyph.

**The Accent on Hover Rule.** Interactive accents start out neutral. The arrow circle is a faint white tint at rest and turns gold only on hover or focus.

**The Two Outline Colours Rule.** Focus rings are Form Blue on light ground and Gold on navy, deep and hero bands. No third ring colour.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans at a single weight (400) is rounded and friendly. It sets the headings and every tappable label, so buttons and rows read in the same voice as the headlines. The system body stays neutral and roomy at 1.7.

### Hierarchy
- **Display** (400, clamp(40px, 11.4vw, 78px), 1.02): the hero H1 only, white on the photo, max 12ch (15ch in Spanish). Its last phrase is set on its own line in gold.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08, balanced wrap): section H2s. On dark bands the last phrase may be gold.
- **Title** (400, 20px, 1.2): service row labels. In the same Cal Sans role: claims (clamp(20px, 5.4vw, 24px)/1.15), step titles (21px, 22px on desktop), Facebook row (clamp(19px, 5.2vw, 22px)), field labels and legends (17px), button labels (18px), and the header number (17px, 20px on desktop).
- **Lede** (400, clamp(17px, 4.6vw, 19px), max 40ch, pretty wrap): the line under a section heading. The hero promise is the same role at clamp(17px, 4.7vw, 20px)/1.5, max 32ch (40ch on desktop).
- **Body** (400, 16px, 1.7): running text. Inputs are also 16px, so iOS doesn't zoom.
- **Label** (500, 14px, .02em): the eyebrow pill. Helper and error text is 14–15px system.

### Named Rules
**The One Face, One Weight Rule.** Cal Sans is only ever set at 400, and size alone carries the hierarchy. Don't add a bold weight or a second display face.

**The Tappable in Display Rule.** Anything a thumb presses (buttons, rows, the phone number, field labels) is set in Cal Sans. Body copy and helper text stay in system sans.

## Layout

The container is a single centred wrap, max 1160px, with side gutters of 20px (16px at 400px and below, 12px at 359px and below, 40px from 760px). Sections pad 64px top and bottom on phones and 96px from 760px. The hero has its own padding (56/72 on phones, 96/112 from 760px, 120/136 from 1024px). Common gaps are 10, 12, 16, 20, 24 and 28px. Heading blocks stack the eyebrow, H2 and lede at 16px gaps with a max width of 640px.

On phones everything is one column. From 760px the hero buttons sit side by side (min 220px each) and the service rows go to two columns. From 1024px:
- the hero photo moves to the right 62% and a horizontal navy gradient holds the words on the left
- the about section splits into two columns with a 64px column gap
- service rows go to three columns
- the work photo takes the left column (1.35fr) with the heading and Facebook row stacked on the right
- the quote section puts a sticky heading beside the form
- the close band puts the name on the left and the big number on the right
- the steps go into three columns

The header is not sticky. It holds the house mark and wordmark on the left, the Español/English toggle, and the tap-to-call number top right. Below 380px it drops the phone icon, and below 360px it drops the mark.

### Motion
- **Hero H1 bounce-in:** the visible language's H1 is split into letter spans (with `nowrap` word wrappers). Each letter animates from `opacity:0; translateX(50px)` to rest over 1s with `cubic-bezier(.34,1.56,.64,1)`, each one 20ms after the last. The H1 stays hidden until Cal Sans loads (400ms at most). While it plays, the H1 has an `aria-label` and the letters are `aria-hidden`. When the last letter's animation ends (or the language is switched), the plain HTML is put back. Use this on the hero H1 only.
- **Fade-up:** elements marked `.rise` that start below the first screen get `.below` (opacity 0, translateY 12px) and transition back over 400ms ease-out when they come into view. Everything is visible at rest, without JS and under reduced motion.
- **Chip pick flash:** when a service row pre-selects a chip, the chip flashes gold and fades back over 900ms ease-out.
- **Float slide:** the floating circle comes up from 120px below over 350ms `cubic-bezier(.2,.8,.2,1)`.
- **State transitions:** 200ms for buttons and arrows, 150ms for fields and chips, and a 120ms press scale of .98 on buttons.

## Elevation & Depth

The page is flat. Depth comes from band contrast (paper against navy against deep), from faint white tints on navy (6–12% white for rows, ghost hovers and arrows), and in the hero from the photo under a navy gradient overlay (86% to 70% top to bottom on phones; on desktop a horizontal gradient from solid deep at 38% to about 42–50% on the right). The diagonal line texture on deep bands is at 3.5% white, faint enough that it never reads as lines through text.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,22,40,.3)`): the floating text circle only, so it reads above whatever band it is over.

### Named Rules
**The One Shadow Rule.** Only the floating text circle has a shadow. Cards, rows, buttons and the form card stay flat. Rows and the Facebook row explicitly set `box-shadow: none` on hover.

## Shapes

The shapes are soft and have no borders. Corners come in four sizes: 10px fields (and the 36px house-mark tile), 18px service rows (the Facebook row is 20px), 24px cards (the form card and the work photo), and full pills for buttons, chips, the eyebrow and every circle (arrow 44px, step number 48px, float 60px). Borders appear only as 2px transparent strokes that colour in for state (button outline, field and chip focus, error), plus the 1px hairline between claims. The photo is clipped to the 24px radius at 4:3 with `object-fit: cover` and is never stretched.

## Components

### Buttons
Big, soft pills with labels in Cal Sans.
- **Shape:** full pill (999px), min height 56px, 26px side padding, 18px Cal Sans label, optional 20px leading icon.
- **Primary:** gold fill, Ink label, matching gold border. On hover (pointer devices only) it brightens to gold-2. Inside the form it is full width and gets a 3px Form Blue outline (3px offset) on hover and focus.
- **Ghost:** transparent, On-Dark label, 2px border in 70% on-dark. On hover the border goes white and it gets a 10% white tint. Used only as the secondary hero action ("Text a photo").
- **Press:** scale .98 over 120ms.
- **Rule:** at most two buttons under the hero H1, the primary and the ghost. Never a Call button.

### Chips
- **Style:** pill, 48px tall, 18px padding (14px below 380px), Field Tint fill, 2px transparent border, 16px system text in Ink. They are visually hidden checkboxes or radios with real labels.
- **State:** hover gives a Form Blue border. Selected is an Ink fill with white text. Keyboard focus gives a Form Blue border plus a 3px Form Blue outline at 2px offset, so focus stays visible on the Ink fill. When a service row picks a chip, it flashes gold.

### Cards / Containers
- **Form card:** white, 24px radius, padding clamp(20px, 5vw, 32px), 22px gaps between fields, max 620px. No border, no shadow.
- **Work photo:** 24px radius, 4:3, navy behind, no caption.

### Inputs / Fields
- **Style:** Field Tint fill, 2px transparent border, 10px radius, 13×14px padding, min 52px tall (textarea min 110px, vertical resize), 16px system text in Ink, Soft placeholder, Form Blue caret. Labels sit above in 17px Cal Sans. "(optional)" is 14px Soft.
- **Hover / Focus:** the border turns Form Blue (on hover only for pointer devices).
- **Error:** the field gets `.bad`. The border turns Signal Red, and stays red while focused (a later, more specific rule), `aria-invalid` is set, and a plain-sentence error appears below in 15px red. Submitting scrolls to and focuses the first bad field.

### Navigation
- **Header:** paper, 64px tall (76px from 760px). The house-mark tile (Ink, 10px radius, gold mark) is followed by "J&J" in 21–24px Cal Sans over "Garage Doors LLC" in 11px uppercase system text. The language toggle is an underlined 15px Soft text button that turns Ink on hover. The tap-to-call number is in Cal Sans with a Gold Ink phone icon and turns Gold Ink on hover. Everything is at least 44px tall.
- **Footer:** deep navy with the line texture, 16px On-Dark Soft text, Facebook link in On-Dark that turns gold on hover. Bottom padding leaves room for the float (96px plus the safe area).

### Service Rows (signature)
These are links on navy, one per service, each with an arrow circle on the right.
- **Style:** a 6% white tint, 18px radius, min 64px tall, 20px Cal Sans in On-Dark. A 44px arrow circle sits on the right (10% white, On-Dark arrow).
- **Hover / Focus:** only the arrow changes. It fills gold with an Ink arrow. The row never gets an outline, border, ring, shadow or extra tint. The keyboard focus ring (3px gold, 3px offset) goes around the arrow circle, not the row.
- **Behaviour:** each row links to the quote form and pre-selects the matching chip, which flashes gold.

### Facebook Row
A navy pill-card (20px radius, min 76px tall) right under the work photo. It has a 28px gold Facebook mark, the line "See more of our work on Facebook." in Cal Sans, and the same arrow circle (12% white at rest). Hover and focus behave exactly like a service row: only the arrow changes.

### Claims List
Three facts on paper, each a 40px Gold Ink line icon beside a clamp(20–24px) Cal Sans line in Ink, 16px vertical padding, separated by 1px hairlines. They aren't links: no arrows, no hover.

### Steps
A numbered list on deep navy. Each number is a 48px gold circle with an Ink numeral in 20px Cal Sans, in a 48px column beside a Cal Sans title (21–22px, On-Dark) and an On-Dark Soft line. One column on phones, three from 1024px with 40px gaps.

### Close Band
On navy: the business name as the H2, a "We do it all" line and the service area in On-Dark Soft, then the big tap-to-call number (Cal Sans clamp(30px, 9vw, 52px), gold phone icon, gold on hover), then the other two callers by name in 17px On-Dark.

### Floating Text Circle (signature)
A 60px gold circle with an Ink chat glyph, fixed bottom right (16px plus the safe area), that opens `sms:` with a pre-filled message in the current language. It slides in once the hero has scrolled past, and slides out while the quote form is on screen, so two controls that do the same thing are never visible together. While hidden it is `tabIndex=-1` and `aria-hidden`. It is the only element with a shadow. It is one circle, never a bar.

### Eyebrow Pill (owner-mandated exception)
A 14px/500 system label in a faint tint pill (6% Ink on paper, 12% white on dark), 9×14px padding, with a 7px gold dot. It sits above the hero H1 and above three section headings. It is a `<p>`, not a heading. It has no arrow, no hover, no shadow and is never a full gold fill. Ellie chose this pill style for the calm house style. The Impeccable craft floor flags eyebrows, so treat this as her recorded exception: don't make it a default for new surfaces, and don't add more.

### Bilingual mechanism
Every piece of copy is written twice, as `<span class="en">` and `<span class="es" lang="es">`. CSS hides the one that isn't active, based on `html[data-lang]`. A blocking script in `<head>` sets the language before first paint, from the saved choice (`localStorage` key `jj-lang`) or else from the browser's language. The header toggle flips `data-lang` and `lang`, saves the choice, and also swaps the placeholders (`data-ph-en`/`data-ph-es`), the photo's alt text (`data-alt-es`), the SMS bodies, the float's label and the text the form composes. Spanish runs longer, so the hero H1's max width widens to 15ch. New copy must always ship in both spans.

## Do's and Don'ts

### Do:
- **Do** alternate full-bleed bands (paper, navy, deep with texture) so each section boundary is a band change.
- **Do** use gold (#f3b324) only as a fill with Ink text on it; use gold-ink (#7a5400) when gold has to be text on light ground.
- **Do** set headings and every tappable label in Cal Sans 400; keep body in the system stack at 16px/1.7.
- **Do** give every form control (text fields, chips, the form's submit) a Form Blue (#1f5fa8) outline on hover and focus; keep error borders red even while focused.
- **Do** keep the hero to an eyebrow, the H1 with the place in it, one promise line and at most two pill buttons (gold primary, outlined ghost).
- **Do** keep the phone number top right in the header on the first screen, and repeat it only in the close band and footer.
- **Do** put the Facebook row directly under the work photo, and again in the footer.
- **Do** show all content at rest, without JS and under reduced motion; the bounce-in is for the hero H1 only.
- **Do** ship every string in both English and Spanish spans.
- **Do** keep tap targets at 44px or larger.

### Don't:
- **Don't** outline, ring, tint or shadow a service row or the Facebook row on hover or focus; only the arrow circle changes.
- **Don't** add a sticky bottom bar or a Call button under the hero title; the single floating text circle is the only fixed control.
- **Don't** put gold text on paper, white text on gold, or gold as a focus ring on light ground.
- **Don't** add shadows to cards, rows or buttons; the float is the one lifted object.
- **Don't** add captions under photos, a lead-in sentence above the work photo, or a services list in the hero.
- **Don't** make non-interactive labels (service areas, towns, claims) look like pills or buttons.
- **Don't** stretch or upscale photos; `object-fit: cover` at the photo's own shape.
- **Don't** let the deep-band texture rise above about 4% white, so no line ever reads through text.
- **Don't** bring back the retired liftable-door world's devices; this project's world is the calm band style.
