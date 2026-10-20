---
name: DC Exterior
description: One-page free-quote site for an exterior contractor, in the calm band style and DC's own ad colours.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0b2340"
  body: "#2a3a4c"
  soft: "#4a5868"
  navy: "#0d2c4d"
  deep: "#061b31"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  yellow: "#f8d404"
  yellow-2: "#ffe13d"
  yellow-ink: "#705f00"
  blue: "#038df8"
  blue-soft: "#5fb4ff"
  line: "rgba(11,35,64,.12)"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(21px, 5.6vw, 25px)"
    fontWeight: 400
    lineHeight: 1.15
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.3
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter-desktop: "40px"
  stack-sm: "16px"
  stack-md: "20px"
  stack-lg: "28px"
  band-phone: "64px"
  band-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.yellow-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-quiet:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-text:
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
  card-form:
    backgroundColor: "{colors.card}"
    textColor: "{colors.body}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "20px 0"
  step-number:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-message:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: DC Exterior

## Overview

**Creative North Star: "The Ad's Navy Band, Made Into a Page"**

The site is DC Exterior's own Facebook ad stretched to a full page: the ad's navy band becomes the hero and the closing bands, its headline yellow becomes the one warm fill, and the logo's bright blue carries icons and focus. Between the navy bands sit calm off-white paper bands, where the work content lives. The result reads as a sturdy local trade: plain, confident, nothing decorative that the business itself does not own.

Density is low and phone-first. Every band is one idea (who and the offer, what we fix, how a quote works, the quote form, the closing line), stacked as full-width bands with generous vertical padding. Depth comes from band colour alternation and a faint diagonal line texture on the navy grounds, not from shadows. Type is Cal Sans for every heading, label and button, over a system sans body at 16/1.7.

There is no photography: no real job photos exist, and the ad's house is an illustration, so the hero is a plain textured navy field with the real logo. Contact is Messenger only; no phone or email affordance is ever drawn.

**Key Characteristics:**
- Alternating full-width bands: navy hero, paper, deep navy, paper, navy, deep footer.
- One warm fill (the ad's yellow) for the primary action, step numbers and the floating message circle.
- Logo blue for line icons and focus on light grounds; yellow takes over focus on dark grounds.
- Cal Sans at weight 400 for every display role; system sans for reading.
- Pill buttons and chips, a 24px-cornered white form card, flat surfaces.
- Motion limited to a hero letter bounce-in and a 12px fade-up for content below the first screen.

## Colors

A two-navy, one-yellow, one-blue palette drawn straight from DC's ad and logo, set on a cool off-white paper.

### Primary
- **Ad Headline Yellow** (`yellow`): the single warm fill. Primary buttons, numbered step discs, the floating message circle, the hover/focus state of row arrows, and text selection. On navy grounds it is also the accent colour for the second clause of a heading ("out of your home.", "works.", "in every season.") and for the header's Messenger icon.
- **Lifted Yellow** (`yellow-2`): hover state of the primary button only.
- **Yellow on Paper** (`yellow-ink`): reserved darkened yellow for the rare case yellow must appear as text on a light ground (5.8:1). Currently unused in the build; keep it as the only legal route.

### Secondary
- **Logo Blue** (`blue`): the logo's house blue. Line icons in the service rows, the focus outline on light grounds, input caret, hover borders on fields, chips and quiet buttons. Never a fill and never body text (3.4:1 on white).
- **Logo Blue, Lifted** (`blue-soft`): the blue raised for use on navy, held for icons on dark grounds.

### Neutral
- **Cool Paper** (`paper`): page ground and the light bands.
- **Card White** (`card`): the quote form card and the light link card.
- **Field Mist** (`field`): input, chip and quiet-button fills inside the white card.
- **Navy Ink** (`ink`): headings on light, all text on yellow, selected chip fill.
- **Slate Body** (`body`): running text on light.
- **Soft Slate** (`soft`): secondary text, signs under service names, placeholders, helper notes.
- **Ad Navy** (`navy`): hero, header and closing band; also the proof link card. Matches the theme colour.
- **Deep Navy** (`deep`): the "how it works" band and footer, always with the line texture.
- **On-Dark** (`on-dark`) and **On-Dark Soft** (`on-dark-soft`): headings and body text on the navy grounds respectively.
- **Hairline** (`line`): 1px dividers between service rows.
- **Error Red** (`error`): field error border and message only.

### Named Rules
**The One Warm Fill Rule.** Yellow is the only warm colour on the page and on light grounds it appears only as a fill with Navy Ink text on it. Its one text use is the accent clause of a heading on a navy ground.

**The Blue Is a Signal Rule.** Logo Blue marks what you can act on or where focus is (icons, focus rings, hover borders). It never fills a button or a band.

**The Focus Swaps With the Ground Rule.** Focus outlines are 3px Logo Blue on paper and white, 3px yellow on navy and deep navy.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** System sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans gives the headings a rounded, sign-painted confidence that suits a trade; the system body keeps reading fast and native inside Facebook's in-app browser.

### Hierarchy
- **Display** (400, clamp 42–80px, 1.02): the hero H1 only, white on navy, max 11ch, second clause in yellow. 52px on landscape phones.
- **Headline** (400, clamp 30–48px, 1.08): band headings (H2), balanced wrap.
- **Title** (400, clamp 21–25px, 1.15): service names in rows and step titles (21px, 22px on desktop).
- **Label** (400, 18px, 1.2): buttons (line-height 1), form field labels and legends, the header "Message us" link (20px on desktop), link-card text. Cal Sans, never system sans.
- **Lede** (400, clamp 18–20px, 1.5): the hero promise (max 30ch on phone) and section ledes (max 38ch).
- **Body** (400, 16px, 1.7): all running text, inputs, chips, footer. Never below 16px for reading text.
- **Caption** (400, 14px, 1.3): the "(optional)" note beside a field label only.

### Named Rules
**The Single Weight Rule.** Cal Sans is always weight 400. Hierarchy comes from size, never from bolding the display face; the body face goes to 600 only for a short bold lead-in ("DC Exterior.").

**The Second Clause Rule.** A heading on a navy ground may set its closing clause in yellow; headings on paper stay all Navy Ink.

## Layout

A single centred column (max 1160px) with a 20px gutter on phones and 40px from 760px. Each band carries 64px vertical padding on phones and 96px from 760px. Content inside a band stacks on a 16 / 20 / 28px rhythm (heading group gap 16px, hero copy and form fields 20px, band-level blocks 28px). Heading groups are capped at 640px, the form at 600px.

Breakpoints: 760px (wider gutter, taller bands, hero buttons go side by side at min 220px), 1024px (two-column bands: hero copy 1.25fr beside the full logo; services and the quote form put the heading group in a sticky left column at top 40px with rows or form on the right; steps become three columns with 40px gaps). A landscape-phone rule (max-height 500px) shrinks the H1 and hero padding so both buttons stay on the first screen.

The header is transparent and absolutely positioned over the hero so the navy and its texture run unbroken to the top edge, respecting safe-area insets.

## Elevation & Depth

Flat by default. Depth is carried by band alternation (paper against navy against deep navy) and by the diagonal line texture on navy grounds: a repeating 135deg gradient of 1px white lines at 3.5% opacity every 23px. The only shadow in the system belongs to the floating message circle, which genuinely floats over content.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(6,27,49,.3)`): the floating Messenger circle only.

### Named Rules
**The Texture Only on Navy Rule.** The line texture appears on the hero and deep-navy bands; paper bands and cards stay untextured.

**The Rows Don't Lift Rule.** Interactive rows and link cards never gain a shadow or background on hover; only their arrow disc reacts.

## Shapes

Soft, friendly geometry: everything you press is a full pill or circle (999px), the form card has 24px corners, inputs 10px, the link card 20px and the post-submit note 16px. Arrow discs (44px), step numbers (48px) and the floating button (60px) are perfect circles. No borders on surfaces; hairline 1px dividers separate service rows; inputs and chips carry a 2px transparent border that turns blue on hover or focus.

## Components

### Buttons
Big, rounded and plain: one obvious yellow action per view.
- **Shape:** full pill, 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** yellow fill, Navy Ink text. Hover lifts to `yellow-2`; inside the form, hover adds a 2px blue outline.
- **Ghost:** transparent with a 2px 70%-white border and On-Dark text, used on navy beside the primary. Hover: solid white border, 10% white wash.
- **Quiet:** Field Mist fill, Navy Ink text, for secondary form actions (copy message, open Messenger). Hover: blue border.
- **Press:** scales to 0.98 over 120ms. Colour transitions 200ms. Hover styles apply only under `(hover:hover)`.

### Chips
- **Style:** pill, 48px tall, Field Mist fill, 2px transparent border, 16px system text.
- **State:** hover gives a blue border; selected turns Navy Ink fill with white text. Single-select (radio) job picker; tapping a service row pre-selects its chip.

### Cards / Containers
- **Corner Style:** 24px (form card).
- **Background:** Card White on paper.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** clamp 20–32px, 20px between fields.

### Inputs / Fields
- **Style:** Field Mist fill, 2px transparent border, 10px radius, 52px min height (textarea 120px), 16px text, blue caret.
- **Focus:** border turns Logo Blue, no outline ring. Hover does the same under a real pointer.
- **Error:** border and a 16px message below in Error Red.
- **Labels:** Cal Sans 18px Navy Ink above the field, with a 14px Soft Slate "(optional)" note.

### Navigation
The header carries only the logo mark (46px, 50px on desktop) at left and a Cal Sans "Message us" link with a yellow Messenger icon at right; the link turns yellow on hover. There is no menu. Footer links are On-Dark, 44px tap height, yellow on hover.

### Service Row (signature)
An icon-title-arrow row: 40px blue line icon, Cal Sans title with a Soft Slate line of signs separated by middots, and a 44px circular arrow disc on a 7% navy wash. Rows are divided by hairlines. On hover or focus only the disc reacts, turning yellow (with a blue focus ring on keyboard focus).

### Link Card
A 76px-tall, 20px-cornered card with a 28px brand icon, Cal Sans label and the same arrow disc. The proof variant ("See our work on Facebook") is navy with white text and a 14% white disc, placed directly under the service rows.

### Numbered Steps
An ordered list where each item leads with a 48px yellow disc holding a Cal Sans numeral in Navy Ink, beside a title and one line of body. One column on phones, three on desktop, on the deep-navy textured band.

### Floating Message Circle
A single 60px yellow circle, fixed bottom right inside safe areas, with a Messenger icon. It slides up from 120px below (350ms, `cubic-bezier(.2,.8,.2,1)`) once the hero is out of view, and hides while the quote form is on screen. It is never a bottom bar.

### Motion
- **Hero letter bounce-in:** the H1 splits into letters that slide in from 50px right with a slight overshoot (1s, `cubic-bezier(.34,1.56,.64,1)`, 20ms stagger). It waits for Cal Sans to load (600ms cap) so letters do not reflow mid-flight, then restores the plain heading. Hero H1 only.
- **Fade-up:** content that starts below the first screen rises 12px and fades in (400ms ease-out). Anything visible at load never animates.
- **Reduced motion:** both are disabled and the float stops transitioning.

## Do's and Don'ts

### Do:
- **Do** alternate bands of paper and navy/deep navy, with the line texture on navy grounds only.
- **Do** keep yellow a fill with Navy Ink text on light grounds; let it colour only the closing clause of a heading on navy.
- **Do** use Logo Blue for icons and focus on light grounds and switch focus to yellow on navy.
- **Do** set every heading, label and button in Cal Sans at weight 400.
- **Do** make every press target a pill or circle at least 44px (buttons 56px, chips 48px).
- **Do** gate hover styles behind `(hover:hover)` so taps don't leave them stuck.
- **Do** route every contact action to Messenger.

### Don't:
- **Don't** put yellow text on paper or white; use `yellow-ink` if it is ever unavoidable.
- **Don't** fill buttons or bands with Logo Blue, and don't set the logo on a black ground.
- **Don't** add shadows to cards, rows or buttons; the floating circle is the only lifted element.
- **Don't** draw phone, email or address affordances; the business publishes none.
- **Don't** stand in for missing job photos with stock or illustration.
- **Don't** replace the floating circle with a sticky bottom bar.
- **Don't** animate anything visible at load other than the hero H1.

## House exception: eyebrow pills

Ellie chose LPMR-style eyebrow pills for the calm band style (2026-10-19), overriding Impeccable's kicker ban. On this page they sit above the hero H1 ("Free quotes"), the services heading and the form heading: 14px/500 system sans, a 7px dot (yellow on navy, logo blue on paper), a faint tint (`rgba(11,35,64,.06)` on paper, `rgba(255,255,255,.12)` on navy), 9px 14px padding, full pill radius, no hover, no shadow, no arrow, marked up as `<p>`, never a heading. Keep them on a few headings only.
