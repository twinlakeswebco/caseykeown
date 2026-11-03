---
name: Casey Keown — Hometown magazine
description: A warm editorial profile with condensed blue headlines and real local photography.
colors:
  paper: "#f5f1e8"
  ink: "#172c55"
  blue: "#17357d"
  red: "#b7372d"
  muted: "#536079"
  line: "#c8c9c7"
  inverse-muted: "#d6ddec"
  inverse-line: "#62769f"
  record-line: "#9bacd2"
  photo-mat: "#d0cbca"
  white: "#fff"
typography:
  display:
    fontFamily: "Barlow, 'Arial Narrow', sans-serif"
    fontSize: "clamp(52px,7.3vw,96px)"
    fontWeight: 800
    lineHeight: 0.94
    letterSpacing: "-.025em"
  headline:
    fontFamily: "Barlow, 'Arial Narrow', sans-serif"
    fontSize: "52px"
    fontWeight: 800
    lineHeight: 1.03
    letterSpacing: "-.02em"
  title:
    fontFamily: "Barlow, 'Arial Narrow', sans-serif"
    fontSize: "31px"
    fontWeight: 800
    lineHeight: 1.1
  body:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
  lead:
    fontFamily: "Georgia, serif"
    fontSize: "26px"
    fontWeight: 400
    lineHeight: 1.4
  label:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "12px"
    fontWeight: 700
    letterSpacing: ".13em"
rounded:
  square: "0"
spacing:
  caption: "10px"
  text: "22px"
  compact: "24px"
  medium: "32px"
  columns: "56px"
  section: "104px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.paper}"
    rounded: "{rounded.square}"
    padding: "16px 22px"
  button-primary-hover:
    backgroundColor: "{colors.red}"
    textColor: "{colors.white}"
  button-light:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.blue}"
    rounded: "{rounded.square}"
    padding: "16px 22px"
  button-light-hover:
    backgroundColor: "{colors.red}"
    textColor: "{colors.white}"
  press-row:
    padding: "34px 0"
    textColor: "{colors.ink}"
  connect-row:
    padding: "19px 0"
    textColor: "{colors.paper}"
---

# Design System: Casey Keown

## Overview

**Creative North Star: "Hometown magazine"**

The approved “Hometown magazine” direction uses warm paper, condensed deep-blue headlines, restrained red punctuation, and a large real portrait. Its character is local, confident, and personable; the density comes from editorial type, generous gutters, and a ruled archive.

Depth stays flat. Photography and full-width blue bands provide visual weight, while publisher metadata and quiet captions give the page the feel of a personal magazine profile.

**Key Characteristics:**

- Warm ivory paper with blue type and restrained red accents.
- Condensed, heavy headlines paired with plain body copy and a serif biography lead.
- Real photography with visible attribution.
- Square controls, thin rules, and flat surfaces.

## Colors

### Primary

- **Hometown Blue** (`blue`): buttons and the podcast/contact bands.
- **Editorial Ink** (`ink`): principal text and the masthead rule.

### Secondary

- **Scoreboard Red** (`red`): wordmark punctuation, hover feedback, and focus outlines on paper.

### Neutral

- **Warm Paper** (`paper`): page canvas and inverse foreground.
- **Quiet Slate** (`muted`): supporting copy, captions, and dates.
- **Archive Rule** (`line`): press separators.
- **Inverse Mist** (`inverse-muted`): supporting text on blue.
- **Inverse Rule** (`inverse-line`): contact separators on blue.
- **Record Line** (`record-line`): podcast record illustration strokes.
- **Photo Mat** (`photo-mat`): image-containment background.
- **White** (`white`): hovered button and contact-link foreground.

**The Red Punctuation Rule.** Use red for small accents and interaction feedback; blue and paper carry the large surfaces.

## Typography

**Display Font:** locally loaded Barlow Condensed at weight 800, registered as `Barlow`, with Arial Narrow and sans-serif fallbacks.

**Body Font:** Arial, Helvetica, sans-serif. **Biography Lead:** Georgia, serif.

The narrow, heavy display face supplies magazine character; body text remains direct and readable. The serif lead adds a brief editorial change of voice.

- **Display:** personal name; use the frontmatter display role. Hero introduction uses `clamp(50px,5vw,74px)`, line-height 1.01, and tracking -.025em.
- **Headline:** section headings; contact heading increases to 82px with line-height 1.
- **Title:** press headlines; podcast and photo statements use 38px at line-height 1.1.
- **Body:** base role in frontmatter; editorial paragraphs use 16px, press summaries 14px, and intro copy 19px at line-height 1.5.
- **Lead:** serif biography opening. Supporting paragraph measures include 34ch for the intro detail, 60ch for podcast copy, and 65ch for press summaries.
- **Label:** uppercase hometown marker. Other metadata varies by context: press tracking .05em, introductory footer .09em, and podcast detail .1em.

## Layout

The centered content container is capped at 1280px and uses `calc(100% - 96px)` on wide screens. Main editorial pairings are equal two-column grids with the column-gap token. Sections use the section spacing token above and below. The masthead is at least 100px high.

The desktop portrait is 580px high with a cover crop at center 38%; at widths of 1400px and above it becomes 630px high. The press archive uses `210px 1fr 28px` columns and 42px gaps. Podcast content uses `105px 1fr auto` columns. Photo art uses a contained 650px image; the adjacent portrait uses a 430px cover crop.

At widths of 1000px and below, container side gutters become 28px, paired-grid gaps become 32px, and the press metadata column narrows to 160px with 25px gaps. The podcast becomes an 80px illustration plus content, with its action below the text. The hometown masthead label is hidden.

At widths of 640px and below, side gutters become 20px, paired grids become one column, and sections use 65px vertical padding. The masthead minimum height is 78px; the first navigation item and nav arrow are hidden. The name uses `clamp(44px,12vw,70px)` on one line. Hero introduction is 58px, section headings 43px, press headings 29px, and the contact heading 68px. Portraits and photo art become natural-height images; the hero portrait caps at 520px and the secondary portrait at 450px. Press rows become `1fr 20px`, with publisher/date in a full-width horizontal row. The record illustration is hidden, captions place credit on its own line, and footer content wraps.

These rules are extracted from HTML/CSS. Browser preview was stopped; this document does not claim visual verification.

## Elevation & Depth

There are no box shadows. Depth comes from paper against blue bands, image crops, spacing, and one-pixel dividers.

**The Flat Paper Rule.** Separate content with space, thin rules, and inverse blue bands; keep surfaces free of decorative shadows.

## Shapes

Controls and imagery use square corners. Press and contact lists use horizontal rules rather than enclosing cards. The circular record illustration is a specific podcast motif, not a general container shape. Arrow icons are thin, unfilled strokes (1.5px), normally 20px square.

## Components

### Buttons

Firm rectangular editorial actions. The primary and light variants use the frontmatter colors and padding, a 35px label-to-icon gap, bold 14px text, and a minimum height of 52px. Both turn red with white type on hover; background transitions last .2s. The light variant keeps its label on one line.

Keyboard focus is a 3px outline offset by 6px: red on paper and paper inside the blue bands. Reduced-motion preference disables transitions and smooth scrolling. No custom active-state treatment is implemented.

### Navigation

An unboxed horizontal link row in bold 13px text, with 30px gaps and 12px vertical link padding. It moves to 19px gaps below 1000px and 17px gaps with 12px text below 640px. Hover turns links red; no selected-item state is implemented.

### Text Links

Compact bold 13px inline links with 24px icon gaps. Ordinary links inherit their foreground and use a 5px underline offset. Preserve the shared hover and keyboard-focus treatments.

### Press Archive Rows

Whole-row links with thin separators, publisher/date metadata, a condensed headline, a quiet summary, and a trailing arrow. Use the responsive grid behavior in Layout. Metadata is part of the editorial identity; do not hide it to shorten a row.

### Contact Rows

Inverse links on blue, separated by quiet inverse rules, with a minimum height of 86px and 24px content-to-arrow gap. Titles are bold 19px; secondary labels are 12px with a 3px top margin. Hover turns the row foreground white; keyboard focus remains paper.

### Wordmark

A compact `CK` in the display family (38px, line-height 1, weight 800), followed by a red period. The mobile masthead version is 32px. It links back to the top.

## Do's and Don'ts

### Do:

- Do use the named palette and condensed headline family.
- Do keep visual headings at or below 96px.
- Do retain source and photography attribution.
- Do stack columns and keep press metadata horizontal on small screens.
- Do preserve visible keyboard focus and reduced-motion behavior.

### Don't:

- Don't introduce generated identity imagery.
- Don't add raised cards, rounded pills, gradients, or decorative shadows to this flat editorial system.
- Don't substitute restaurant menu or booking conventions for the personal profile.
