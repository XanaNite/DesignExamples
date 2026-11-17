# Afterglow Design Spec

## Overview

Afterglow is an editorial, tactile music-community direction for First Row. It frames a fan membership as a warm, human exchange between artists and the listeners who support them.

- **Concept direction:** Editorial warmth
- **Primary page:** `concepts/afterglow.html`
- **Design style:** Soft paper textures, literary typography, rounded forms, and coral accents
- **Primary user value:** Feeling personally connected to independent artists and their creative journeys

## Brand Strategy

### Positioning

Afterglow presents First Row as a closer kind of fan club rather than a conventional streaming or merchandise platform. The experience emphasizes listening, gathering, and keeping meaningful objects.

### Tone of voice

- Warm and reflective
- Intimate without being exclusive
- Emotion-led and specific
- Confident through understatement

Example headline patterns:

- "Good music stays with you."
- "The best part of music is feeling connected."
- "A warmer way to feel like you belong."

## Visual Language

### Color

| Role | Value | Usage |
|---|---|---|
| Paper | `#f5eee4` | Main page background |
| Ink | `#28231f` | Primary text and dark graphics |
| Coral accent | `#ce6048` | Emphasis, rules, and highlighted words |
| Muted text | `#69635d` | Supporting copy |
| Warm peach | `#e9c2b2` | Story art and perks background |
| Saturated coral | `#ed815e` | Sun and record artwork |

Apply warm, low-saturation surfaces before bright accent colors. The coral accent should guide attention, not dominate body copy.

### Typography

The global typography stack is:

- **Display:** Playfair Display, Georgia, serif
- **Body:** DM Sans, Arial, sans-serif
- **Mono:** DM Mono, Courier New, monospace

| Element | Treatment |
|---|---|
| Hero title | Display, 500 weight, approximately 57–105 px, tight -0.065em tracking |
| Section title | Display, 500 weight, approximately 40–75 px |
| Emphasized words | Display or inherited face, italicized, coral |
| Eyebrows | Mono, 10 px, uppercase, 0.12em tracking |
| Body | DM Sans, 14–15 px, 1.7–1.8 line height |
| Metadata | Mono, 9 px, uppercase, 0.1em tracking |

### Shapes and Imagery

- Use imperfect circular and arch-like forms.
- Reference records, sunlit paper, sleeves, and physical objects.
- Add slight rotational offsets to ribbons, labels, and sign-offs.
- Keep artwork abstract and decorative; do not imply it is a real artist photograph.

## Page Structure

1. **Header:** FIRST ROW wordmark, navigate menu, and link to all directions.
2. **Hero:** Statement, supporting copy, primary and secondary calls to action, and a record-inspired visual.
3. **The idea:** Two-column story copy beneath a label and large editorial headline.
4. **Member moments:** Three perks—first play, small-room shows, and limited editions.
5. **About:** Brand belief and artist-fan relationship.
6. **Why it works:** A concise rationale for the direction.
7. **Contact:** Final invitation and email call to action.
8. **Footer:** Brand, message, and back-to-top link.

## Component Specifications

### Hero

- Desktop: two-column layout with a 1.02:0.98 proportion.
- Minimum hero height: 630 px.
- The copy sits above the decorative artwork.
- The artwork uses an arched container, concentric disc forms, a coral sun, and a rotated dark ribbon.

### Navigation Menu

- Use a native `details`/`summary` pattern.
- The menu expands to a compact panel containing in-page links.
- The summary changes visually from `+` to `−` when open.

### Perk Cards

- Use three columns on desktop.
- Separate cards with 1 px vertical rules.
- Each card contains a numbered label, icon, heading, and short description.
- Card minimum height: 220 px.

### Buttons

- Minimum height: 47 px.
- Dark or ink background for primary actions.
- Link style with an underline for secondary actions.
- Include an arrow or directional glyph as decorative affordance.

## Responsive Behavior

- At 800 px or less: reduce padding and switch the main hero toward a balanced two-column composition.
- At 560 px or less: stack the hero, remove the side note, and display story and perk sections as one column.
- Use `clamp()` for display headlines and decorative art.
- Mobile perk cards become stacked rows separated by borders.
- Preserve smooth in-page navigation on desktop and reduce motion behavior on mobile.

## Accessibility

- Maintain a skip link for keyboard users.
- Preserve a clear heading hierarchy: one H1, H2 section headings, and H3 perk headings.
- Decorative artwork must use `aria-hidden="true"`.
- Include visible `:focus-visible` states.
- Do not rely on color alone to communicate information.
- Use semantic `main`, `header`, `footer`, `nav`, and `section` elements.
- Support `prefers-reduced-motion: reduce`.

## Implementation Notes

- Source: `concepts/afterglow.html`
- Shared styles: `styles.css`
- Concept selector: `.afterglow`
- Primary variables:
  - `--paper: #f5eee4`
  - `--ink: #28231f`
  - `--muted: #69635d`
  - `--accent: #ce6048`
