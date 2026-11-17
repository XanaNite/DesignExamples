# Static Bloom Design Spec

## Overview

Static Bloom is a bold, independent First Row direction built from gig-poster energy and DIY print systems. It asks fans to make noise, show up, and support artists directly.

- **Concept direction:** Independent print
- **Primary page:** `concepts/static-bloom.html`
- **Design style:** Poster-scale type, visible grids, hard borders, acid accents, and limited-edition objects
- **Primary user value:** A direct, participatory way to keep independent music alive

## Brand Strategy

### Positioning

Static Bloom presents the audience as a necessary part of the artist's future. It resists polished platform conventions and treats membership as a rally, a fanzine, or a scene.

### Tone of voice

- Direct and declarative
- Rebellious but inclusive
- Plainspoken
- High-energy without becoming noisy in copy

Example headline patterns:

- "NO FANS. NO FUTURE."
- "The crowd is part of the sound."
- "A little rebellious. Very easy to get."

## Visual Language

### Color

| Role | Value | Usage |
|---|---|---|
| Off-white | `#f2f1e8` | Main surface |
| Acid green | `#b9e83a` | Emphasis, perks, buttons, and contact text |
| Near-black | `#191a16` | Text, borders, and contact background |
| Soft gray | `#4f5049` | Supporting text |
| Faint gray | `#e6e5d9` | Hero artwork |
| Hard rule | `rgba(25,26,22,.55)` | Structural lines |

### Typography

- **Display:** Playfair Display
- **Body:** DM Sans
- **Mono:** DM Mono

| Element | Treatment |
|---|---|
| Hero title | DM Sans, 700 weight, approximately 62–124 px, -0.105em tracking, 0.78 line height |
| Emphasized word | Acid background, near-black text, no italic |
| Section title | Playfair Display, 500 weight |
| Eyebrows | Mono, 10 px, uppercase |
| Metadata and labels | Mono, compact and heavily tracked |

### Shapes and Imagery

- Use poster-like blocks and visible grid lines.
- Apply hard 2 px borders instead of soft shadows.
- Use a small number of offset and rotated elements.
- Reference:
  - Gig posters
  - Stickers
  - Barcodes
  - Zines
  - Hand stamps
- Preserve a sense of print imperfection without sacrificing layout clarity.

## Page Structure

1. **Header:** Mono wordmark and 2 px bottom border.
2. **Hero:** Declarative headline, fan proposition, actions, and poster art.
3. **The idea:** Direct explanation of the artist-fan relationship.
4. **Member moments:** Rough cuts, pop-up listening parties, and artist-run drops.
5. **About:** Fan and artist value statement.
6. **Why it works:** Rationale for disruptive, scannable communication.
7. **Contact:** Near-black close with acid-green emphasized text.
8. **Footer:** Brand and navigation.

## Component Specifications

### Poster Hero

- Desktop: balanced 1:1 two-column composition.
- Minimum hero height: 650 px.
- The artwork uses a 34 px grid, a 2 px frame, and a rotated acid poster.
- Add a circular loud-and-proud sticker and a barcode motif.

### Headline Treatment

- Keep the hero all-caps and tightly tracked.
- Use an acid-green background only on the key emphasized phrase.
- Preserve readable line breaks across desktop and mobile.

### Perk Cards

- Three-column desktop layout.
- 2 px top and bottom borders.
- 2 px vertical separators.
- Cards include numbered labels, mono icons, headings, and concise copy.

### Buttons

- Primary: acid green background, near-black text, 2 px near-black border.
- Contact: acid green light button over the near-black contact surface.
- Secondary: underlined text link.

## Responsive Behavior

- At 800 px or less: use reduced two-column hero padding and adjust the headline.
- At 560 px or less:
  - Stack the hero copy and artwork.
  - Scale the headline to 62–88 px.
  - Set hero artwork to 96vw high with a 410 px maximum.
  - Convert perk cards to stacked rows with 2 px top borders.
  - Add the 2 px section and card rules consistently.

## Accessibility

- Preserve semantic page landmarks and heading hierarchy.
- Keep poster artwork decorative and hidden from assistive technology.
- Use near-black text on acid green and maintain strong contrast.
- Do not communicate meaning through rotation or grid placement alone.
- Retain visible focus states and skip-navigation support.
- Respect reduced-motion preferences.

## Implementation Notes

- Source: `concepts/static-bloom.html`
- Shared styles: `styles.css`
- Concept selector: `.static`
- Key variables:
  - `--paper: #f2f1e8`
  - `--ink: #191a16`
  - `--muted: #4f5049`
  - `--line: rgba(25,26,22,.55)`
  - `--accent: #b9e83a`
