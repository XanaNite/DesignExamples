# Velvet Signal Design Spec

## Overview

Velvet Signal is an intimate, after-hours First Row direction. It presents membership as personal access to the people and moments around an artist.

- **Concept direction:** After-hours club
- **Primary page:** `concepts/velvet-signal.html`
- **Design style:** Ink-dark surfaces, warm brass, soft theatrical light, and ticket graphics
- **Primary user value:** Access to private, limited, and close-up artist moments

## Brand Strategy

### Positioning

Velvet Signal translates membership into an invitation: unreleased music, intimate gatherings, and limited artist objects. Exclusivity should feel welcoming and relationship-led, not status-driven.

### Tone of voice

- Lower-lit and composed
- Slightly cinematic
- Warm rather than formal
- Direct about the value of access

Example headline patterns:

- "The music doesn't end at the encore."
- "A little access. A lot of meaning."
- "Exclusivity with a human pulse."

## Visual Language

### Color

| Role | Value | Usage |
|---|---|---|
| Ink background | `#11111b` | Main surface |
| Deep violet | `#211b2c` | Hero art and member area |
| Secondary ink | `#171620` | Story and about surfaces |
| Brass accent | `#d9af75` | Emphasis and call-to-action |
| Warm ivory | `#f4ede0` | Primary text |
| Muted pearl | `#b6b0ae` | Supporting text |
| Ticket cream | `#e5d7c1` | Membership ticket |

### Typography

- **Display:** Playfair Display
- **Body:** DM Sans
- **Mono:** DM Mono

The Velvet Signal hero reverses the standard hierarchy: DM Sans carries the main headline, while Playfair Display carries the italic emphasis.

| Element | Treatment |
|---|---|
| Hero title | DM Sans, 500 weight, approximately 54–96 px, -0.07em tracking |
| Emphasis | Playfair Display, 500 weight |
| Section title | Playfair Display, 500 weight, approximately 40–75 px |
| Eyebrows | Mono, 10 px, uppercase |
| Ticket | Mono labels and a heavy DM Sans headline |

### Shapes and Imagery

- Use halo-like radial gradients.
- Build a silhouetted or stage-like figure rather than a literal event photograph.
- Use a perforated ticket as the strongest access motif.
- Keep vertical labels and tiny mono copy as atmospheric detail.
- Rotate the ticket and add deep shadows to create an object in space.

## Page Structure

1. **Header:** FIRST ROW wordmark, navigation menu, and all-directions link.
2. **Hero:** Evening-themed headline, member proposition, actions, and ticket artwork.
3. **The idea:** Access-focused explanation and two-column story.
4. **Member moments:** Unreleased cuts, close-up sessions, and members' editions.
5. **About:** Artist honesty and mutual appreciation.
6. **Why it works:** Rationale for premium intimacy.
7. **Contact:** Brass contact area with dark text.
8. **Footer:** Brand and navigation.

## Component Specifications

### Hero Artwork

- Desktop: 0.9:1.1 copy-to-art ratio.
- Minimum height: 690 px.
- Use a violet stage surface.
- Layer radial brass light, a dark figure, the ticket, and vertical text.
- Ticket dimensions: 37% of the art width, minimum 200 px height.

### Navigation Menu

Use the shared `details` navigation pattern. The dark page uses the existing `--paper` variable for menu surface, keeping contrast consistent.

### Perk Cards

- Three columns on desktop.
- Brass or accent-colored icons.
- Numbered labels and concise member benefit copy.
- Shared 1 px light rule system.

### Buttons

- Primary button: brass `#d9af75` background with `#17151b` text.
- Text link: warm ivory.
- Contact button: dark ink with warm ivory text.

## Responsive Behavior

- At 800 px or less: maintain the hero in two columns with reduced copy and artwork widths.
- At 560 px or less:
  - Stack copy and artwork.
  - Scale the hero headline to 51–70 px.
  - Set hero artwork to 96vw with a 410 px maximum height.
  - Stack perk cards and story columns.

The ticket and figure must remain decorative and should not obscure readable hero copy.

## Accessibility

- Skip link and visible keyboard focus remain mandatory.
- Keep all decorative artwork out of the accessibility tree.
- Use the warm ivory text on dark surfaces for primary reading.
- Verify that brass accent text maintains sufficient contrast against dark surfaces.
- Preserve semantic landmarks and H1/H2/H3 hierarchy.
- Respect `prefers-reduced-motion: reduce`.

## Implementation Notes

- Source: `concepts/velvet-signal.html`
- Shared styles: `styles.css`
- Concept selector: `.velvet`
- Key variables:
  - `--paper: #11111b`
  - `--ink: #f4ede0`
  - `--muted: #b6b0ae`
  - `--line: rgba(244,237,224,.22)`
  - `--accent: #d9af75`
