---
name: ClearedCo
description: A fogged dusk window you wipe clear; window cleaning and pressure washing, Canfield, Ohio.
colors:
  indigo: "#2a2260"
  indigo-2: "#332a72"
  hero-end: "#3b3184"
  indigo-ink: "#1f1a46"
  violet: "#6f64b8"
  lavender: "#c9c2ff"
  lav-soft: "#b4acdf"
  mist: "#efedfa"
  mist-2: "#e3e0f5"
  frame-paint: "#f1eff9"
  muted: "#4d4682"
  field-stroke: "#857cc2"
  water: "#3cc4dd"
  water-deep: "#0f8aa0"
  error: "#b3243b"
  white: "#ffffff"
  facebook-blue: "#1877f2"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(46px, 14vw, 96px)"
    fontWeight: 900
    lineHeight: 0.92
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(34px, 9vw, 56px)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(28px, 7vw, 40px)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 700
    lineHeight: 1.35
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1
rounded:
  glass: "3px"
  tag: "6px"
  field: "12px"
  card: "14px"
  pill: "999px"
  round: "50%"
spacing:
  gutter-phone: "20px"
  gutter-wide: "32px"
  chip-gap: "8px"
  stack-tight: "10px"
  stack: "22px"
  section-phone: "30px 0 52px"
  section-desktop: "48px 0 84px"
components:
  button-primary:
    backgroundColor: "{colors.lavender}"
    textColor: "{colors.indigo-ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.white}"
    textColor: "{colors.indigo-ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "56px"
  button-send:
    backgroundColor: "{colors.indigo}"
    textColor: "{colors.white}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    height: "56px"
    width: "100%"
  button-send-hover:
    backgroundColor: "{colors.indigo-2}"
  input-field:
    backgroundColor: "{colors.white}"
    textColor: "{colors.indigo-ink}"
    rounded: "{rounded.field}"
    padding: "14px"
    height: "54px"
  chip:
    backgroundColor: "{colors.white}"
    textColor: "{colors.indigo-ink}"
    rounded: "{rounded.field}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.indigo}"
    textColor: "{colors.white}"
  service-row:
    textColor: "{colors.indigo-ink}"
    typography: "{typography.lead}"
    padding: "8px 2px"
    height: "62px"
  service-row-arrow:
    backgroundColor: "{colors.mist-2}"
    textColor: "{colors.indigo-ink}"
    rounded: "{rounded.round}"
    size: "40px"
  service-row-arrow-hover:
    backgroundColor: "{colors.violet}"
    textColor: "{colors.white}"
  link-card:
    backgroundColor: "{colors.white}"
    textColor: "{colors.indigo-ink}"
    rounded: "{rounded.card}"
    padding: "16px 18px"
    height: "64px"
  photo-tag:
    backgroundColor: "rgba(31,26,70,.82)"
    textColor: "{colors.white}"
    rounded: "{rounded.tag}"
    padding: "5px 10px"
---

# Design System: ClearedCo

## Overview

**Creative North Star: "The Fogged Dusk Window"**

The whole page is the view through a window at dusk, in the logo's own indigo-to-violet. Its signature is a painted wooden sash with mullions that holds live glass: condensation haze over a dusk yard, beaded drops that swell and run, and a fog the visitor wipes clear with a finger (or that wipes itself when left alone). The same painted frame holds the one real work photo, so the evidence sits inside the same window as the demonstration. Sections are not boxed; they are separated by a moving water line, as if the page were water rising and falling against glass.

Everything around the window stays plain and heavy: dark indigo grounds, cool mist light sections, heavy uppercase system type, pill buttons, and a single clear-water cyan that appears only when a form control is hovered or focused. Density is low and phone-first: one column, 17px minimum reading size, 44px+ touch targets, generous vertical rhythm. Depth comes from the painted frame, the fog and the drops, never from cards floating on cards.

The world was shaped by Ellie's pitch-site house rules, which are binding on future edits: the system font stack is mandated (no webfonts); the layout is designed at 360-430px first and adapts up; there is no sticky bottom bar; the phone number (or the Messenger link until a phone exists) appears top-right in the header only; color accents appear on hover, not at rest; form controls outline in one accent (water) on hover and focus; service rows highlight only their arrow; the Facebook link sits directly under the work photo.

**Key Characteristics:**
- Logo indigo grounds (never black), alternating with mist-lavender light sections.
- One living element made of the trade's material: water on glass, inside a painted wooden sash.
- Heavy (900) uppercase system type for headings; 17px body floor.
- Moving water-line seams between every section instead of borders or hard cuts.
- Accent appears on interaction only; cyan is reserved for form controls.

## Colors

A two-temperature indigo palette lifted straight from the logo gradient, with a single cool water cyan held back for interaction.

### Primary
- **Logo Indigo** (indigo): page ground, header, footer, numbered step discs, the send button and checked chips. It is the "night" of the dusk.
- **Indigo Second Light** (indigo-2): the second dark section (Recent work) and the send button's hover, one step lighter so alternating dark sections read as distinct.
- **Hero Dusk** (hero-end): the hero gradient's lower end; the hero ramps from indigo at 30% to this toward the bottom.
- **Logo Violet** (violet): the logo's light end. Used for text selection, the service-row arrow on hover/focus, and seam lines on light grounds (at 55% alpha).
- **Lavender Fill** (lavender): primary button fill and border, header and footer icon tint, the checked-chip tick box.

### Secondary
- **Clear Water** (water): the only interaction accent. Global focus outline (3px, offset 3px), and the border plus 3px 25%-alpha halo on inputs and chips on hover/focus.
- **Deep Water** (water-deep): the same role inside light sections, where the bright cyan would fail contrast. Light sections redefine the water variable to this value.

### Neutral
- **Indigo Ink** (indigo-ink): all text on light grounds; primary button text.
- **Mist** (mist): light section ground; also the "done" textarea fill.
- **Mist Shade** (mist-2): service-row dividers, resting arrow and link-card arrow discs, done-panel border.
- **Muted Violet Ink** (muted): secondary text on mist (step descriptions, "(optional)" hints, send hint).
- **Soft Lavender** (lav-soft): secondary text on indigo (brand subline, footer list).
- **Field Stroke** (field-stroke): resting 2px border of every input, chip and chip tick box.
- **Frame Paint** (frame-paint): base paint of the window sash and sill; the canvas shades it from near-white to a cool lilac grey.
- **Error Red** (error): form error message only.
- **Facebook Blue** (facebook-blue): third-party brand color, scoped to the Facebook link card (its glyph, and its arrow disc on hover). Nowhere else.

### Named Rules
**The Never Black Rule.** Dark grounds are logo indigo or its lighter steps. No #000 or neutral grey surfaces anywhere; shadows are tinted indigo (rgba(20,12,60,...)) inside the frame.

**The Water Is For Hands Rule.** Cyan appears only in response to a hand: hover or focus on a form control or button. Nothing in the resting page is cyan.

## Typography

**Display Font:** the system stack (-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif), mandated by the house rules.
**Body Font:** the same stack.

**Character:** One family at two extremes: 900-weight uppercase headings echo the logo's heavy wordmark, while body copy stays at 400-500 in sentence case. Hierarchy is carried by weight and size, not by a second face.

### Hierarchy
- **Display** (900, clamp(46px,14vw,96px); desktop clamp(64px,7.4vw,96px); line-height 0.92; -0.02em; uppercase): the hero headline only.
- **Headline** (900, clamp(34px,9vw,56px), line-height 1, uppercase, balanced wrap): section headings ("What we clean", "Get your free quote"). The Recent work heading steps to clamp(44px,5vw,64px) on desktop.
- **Title** (900, clamp(28px,7vw,40px), uppercase): sub-headings inside a section ("Where we work", "How it works").
- **Lead** (700-800, 22px, line-height 1.35): service rows, step titles, area line, footer name, done-panel heading, link card on wide screens.
- **Body** (400-500, 17px, line-height 1.55): all running text; the hero promise rises to clamp(17px,4.6vw,20px) at 34ch max.
- **Label** (800, 17px): buttons, form labels and legends, header contact.

### Named Rules
**The 17px Floor Rule.** Nothing a visitor must read is smaller than 17px. The two 13px exceptions (brand subline, photo tag) are short decorative captions and must not spread.

**The Uppercase Is For Headings Rule.** Uppercase belongs to headings and the wordmark. Buttons, labels and rows stay in sentence case.

## Layout

Phone-first single column with a 20px gutter (32px from 600px), capped at a 1180px wrap. Sections alternate dark and light, each joined by a 44px (64px desktop) animated water-line seam whose fill is the next section's color.

- **Phone (<600px):** hero stacks headline, promise, two full-width buttons (10px gap), then the framed window filling the rest of the viewport (clamp(280px,46svh,380px)). The window bleeds 4px past the gutter.
- **600px+:** buttons sit side by side at intrinsic width; the window returns inside the gutter; done-panel buttons go two-up.
- **1024px+:** hero becomes two columns (1fr / 1.05fr, 56px gap), window height min(560px,64svh). The services section becomes 1.2fr / 1fr (72px gap). Recent work becomes photo (max 440px) beside heading and link card (72px gap). Header grows to 76px.
- **Phone landscape (max-height 500px):** hero goes two-up with the window at calc(100svh - 120px).
- **Rhythm:** sections pad 30px top / 52px bottom (48/84 desktop); blocks within sections stack at 22px; sub-sections separate by 44-56px. The form caps at 640px.
- **Header:** static, not sticky; 64px tall (76px desktop); brand left, contact top-right. No sticky bottom bar at any width.

## Elevation & Depth

Mostly flat surfaces; depth lives in the material of the window. The painted sash is drawn in canvas with light from the upper left: rails shaded from near-white to lilac grey, brush marks along the grain, a rebate line at the glass, and indigo-tinted cast shadows from the top rail, left stile and mullions onto the glass. The sill is a wider ledge with a lit top face and a soft shadow beneath. Inside the glass, fog thickens toward the bottom of each pane and drops act as tiny inverted lenses.

### Shadow Vocabulary
- **Window drop** (`box-shadow: 0 22px 40px -18px rgba(0,0,0,.55)`): under every framed window, so it hangs off the wall.
- **Link card lift** (`box-shadow: 0 12px 28px -14px rgba(0,0,0,.55)`): the white Facebook card on the indigo work section.
- **Logo disc** (`box-shadow: 0 2px 8px rgba(0,0,0,.3)`): the round logo in header and footer.
- **Field halo** (`box-shadow: 0 0 0 3px rgba(60,196,221,.25)`): focus state of inputs and chips; a state, not elevation.

### Named Rules
**The Depth Is Material Rule.** Shadows are soft, negative-spread and below the object. Depth is earned by things that are physically raised (sash, sill, a card held in the hand), never by stacking surfaces.

## Shapes

Two families. Interactive pieces are soft: pill buttons (999px), 12px fields and chips, 14px cards, full circles for arrows, step numbers and the logo. The window world is crisp: glass and photos at 3px, the window shadow box and photo tag at 6px, the sash itself square-cornered with butt joints (stiles run between full-width rails) and four panes split at 46% height to match the mullions. Dividers are 1px mist-shade hairlines; control borders are 2px.

## Components

### Buttons
Confident, full-height pills.
- **Shape:** pill (999px), 56px minimum height, 2px border, 800 17px label, 10px icon gap.
- **Primary:** lavender fill and border, indigo-ink text. Hover: white fill and border.
- **Ghost:** transparent with lavender border, white text on indigo. Hover: lavender at 14% alpha. On light grounds (done panel) the border is indigo and text indigo-ink; hover/focus turns the border water and the fill mist.
- **Send:** full-width indigo fill on the quote form with the Messenger glyph. Hover/focus: border turns water, fill steps to indigo-2.
- **Press:** scale(.98). Transitions: background and color .2s, transform .15s.

### Chips
- **Style:** service checkboxes as 46px-tall labels, 12px corners, white fill, field-stroke border, with a 16px square tick box (4px corners) inside.
- **State:** hover and keyboard focus turn the border water (focus adds the halo). Checked: indigo fill, white text, the tick box fills lavender with an indigo-ink check. Checked chips still take the water border on hover/focus.

### Cards / Containers
- **Link card (Facebook):** white, 14px corners, 16px 18px padding, 64px min height, 30px Facebook glyph, a 36px mist-shade arrow disc pushed right that turns Facebook blue on hover. Max 460px on desktop. Always placed directly under the work photo.
- **Done panel:** white, 14px corners, 2px mist-shade border, 18px padding; holds the composed message in a mist-filled read-only textarea.
- **Shadow Strategy:** see Elevation & Depth.

### Inputs / Fields
- **Style:** white fill, 2px field-stroke border, 12px corners, 14px padding, 54px min height (textarea 96px, vertical resize), 500 17px indigo-ink text, indigo caret.
- **Hover / Focus:** border turns water; focus adds the 3px water halo and suppresses the outline. One accent only.
- **Error:** a single alert line in error red above the send button, marking the field aria-invalid and focusing it; fields themselves do not change color.

### Navigation
- **Header:** brand lockup (44px logo disc, 52px desktop; "CLEARED CO" 900 uppercase 17px, 22px desktop, .04em; "Canfield, Ohio" 13px soft lavender beneath) left. Contact link top-right: lavender 20px glyph plus 800 17px text, underline on hover. Until a phone exists it reads "Message us" and opens Messenger; once `CONFIG.PHONE` is set it becomes the formatted tap-to-call number. This is the only place the phone appears besides the footer list.
- **Footer:** 56px logo, full business name in lead weight, a soft-lavender list with icon links (Facebook, phone when set), 44px targets, safe-area bottom padding.

### Service Rows
The whole row is a link to the quote form (and preselects the matching chip); only the arrow reacts.
- 62px rows of 700 22px text between 1px mist-shade hairlines; a 40px mist-shade arrow disc at the right.
- Hover/focus: the arrow disc turns violet with a white arrow; keyboard focus puts a 3px violet ring on the disc. The row itself never gets a background, outline or shadow.

### Numbered Steps
44px indigo discs carrying a 900 22px counter, a 14px gap, then a lead-weight title and muted description.

### The Fogged Window (signature)
A painted sash (canvas `.frame`, `data-mullions` for the hero's four-pane version) around a pane holding three layers: a drawn dusk yard (sky gradient, stars, two tree lines, a neighbour's house with two lit windows, lawn) set as the pane's CSS background; a frost layer (the scene downsampled, a fog veil per pane row, light blooms, condensation grain) revealed through a wipe mask; and drops drawn on top. Fog regrows slowly; beads swell into runners that stop and go down the glass leaving trails; a finger or mouse soaks up water and pushes a runner off the lower edge of the stroke. After 4.5s idle a ghost hand wipes one pane in side-to-side passes, rests, then moves to another pane. Reduced motion: a still frame with one pane pre-wiped; hand wiping still works.

The work photo uses the same sash without mullions and holds a before/after slider: the before image is clipped by `--x` over the after, a plain solid 3px white divider with a 44px white knob (indigo chevrons), uppercase "Before" tag top-left and "After" top-right. It sweeps 50→74→30→50% once on first view (700ms per leg, ease-in-out), not at all under reduced motion.

### Water-Line Seams
SVG seams between sections: a filled path in the next section's color topped by a 2px non-scaling stroke (white at 55% on dark-to-light, violet at 55% on light-to-dark), animated as a sum of three sine swells. Phones redraw every other frame.

### Tunable Constants
Change behavior through these, not by editing the drawing code, so the pieces stay in agreement.

- **`T` (glass IIFE):** REGROW 0.0032 (fog return per frame), BRUSH 30 (finger radius, px), GHOST_IDLE 4500 (ms before self-wipe), GHOST_PASSES 1.4 (passes/s), GHOST_PAUSE 1.5 (s rest between panes), SWELL 0.7 (beads starting to swell per s), RUN_AT 3.2 (radius at which a bead runs), MAX_RUNNERS_PHONE 4 / _DESKTOP 9, BEADS_PHONE 45 / _DESKTOP 90, DPR_CAP 1.5 (phones render at 1x).
- **`PALETTE` (glass IIFE):** sky ['#3a2f7e','#5e50ae','#a592d8','#f0b5a6'], trees ['#463a86','#30276a'], lawn ['#342c6c','#251f52'], house '#271f58', lit '#ffd08a', glow '255,200,130', fog '238,235,252' at fogTop .56 / fogBottom .74, rim '25,18,64'. The scene stays in logo hues; the only warm notes are the low sun and the lit windows.
- **`PANES` (glass IIFE):** [[0,0,.5,.46],[.5,0,1,.46],[0,.46,.5,1],[.5,.46,1,1]]. The .46 split must equal `F.MULLION_Y`, and the frost veil bands in drawFrost use the same .46.
- **`F` (paintFrames):** RAIL 13, SILL 18, OVER 8, PAINT '#f1eff9', MULLION 10, MULLION_Y .46. `.window` padding (13px 13px 31px) equals RAIL on three sides and RAIL + SILL at the bottom; `.frame` overhangs by OVER (left/right -8px). Change them together.
- **`S` (seams):** SPEED 0.7, AMP 6 (viewBox units on a 1440x60 box, baseline y 30).
- **`CONFIG`:** PHONE '' (10 digits; when set, header and footer show tap-to-call and the form hands off by SMS instead of Messenger), FB_ID '61589631985029', FB_URL, NAME 'ClearedCo'.

## Do's and Don'ts

### Do:
- **Do** keep every dark ground on logo indigo, indigo-2 or the hero dusk ramp; light grounds on mist.
- **Do** join every section to the next with a water-line seam whose fill is the next section's color.
- **Do** put new proof photos inside the painted sash with a 3px-cornered image and the window drop shadow, and keep the Facebook link card directly beneath them.
- **Do** use water (water-deep inside light sections) as the single hover/focus outline color for inputs, chips and form buttons, with the 3px 25% halo on focus.
- **Do** keep service-row hover confined to the arrow disc turning violet.
- **Do** keep readable text at 17px or larger and touch targets at 44px or larger (buttons 56px, fields 54px, chips 46px).
- **Do** keep `PANES`, `F.MULLION_Y` and the `.window` padding in agreement when resizing the frame.

### Don't:
- **Don't** load a webfont; the system stack is a house mandate.
- **Don't** add a sticky bottom bar or a floating call button; the contact lives top-right in the header.
- **Don't** show the phone number anywhere but the header contact and the footer list.
- **Don't** use cyan (or any accent) at rest; accents answer a hover or focus.
- **Don't** give service rows a background, outline or shadow on hover.
- **Don't** use black or neutral grey grounds or shadows inside the window world.
- **Don't** use Facebook blue outside the Facebook link.
- **Don't** add small uppercase tracked labels above headings; the 13px uppercase style belongs only to the tag on a photo.
