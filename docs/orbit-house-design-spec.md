# Orbit House Design Spec

## Overview

Orbit House is a bright, future-facing First Row direction. It presents fan support as shared momentum around an artist, where listening, gathering, and sharing form one community system.

- **Concept direction:** Future in motion
- **Primary page:** `concepts/orbit-house.html`
- **Design style:** Open green surfaces, cobalt structure, coral movement, and orbital diagrams
- **Primary user value:** Joining a visible community that helps independent music travel further

## Brand Strategy

### Positioning

Orbit House explains the fan-artist relationship through connection and participation. It is less about status or exclusivity and more about movement, discovery, and collective support.

### Tone of voice

- Optimistic and active
- Clear and accessible
- Community-oriented
- Forward-looking without technical jargon

Example headline patterns:

- "Music brings us into orbit."
- "Every artist has a constellation."
- "Modern, optimistic, built to connect."

## Visual Language

### Color

| Role | Value | Usage |
|---|---|---|
| Soft green | `#eff4ee` | Main background |
| Mist green | `#e3ebe1` | Story and about areas |
| Sage green | `#d8e6d4` | Perks and hero art |
| Deep teal ink | `#1a2726` | Primary text |
| Cobalt | `#264bbc` | System lines, nodes, and primary button |
| Coral | `#e96943` | Accent and central orbit |
| Acid lime | `#d9ff6e` | Emphasis in contact section |

### Typography

- **Display:** Playfair Display
- **Body:** DM Sans
- **Mono:** DM Mono

| Element | Treatment |
|---|---|
| Hero title | DM Sans, 500 weight, approximately 58–104 px, -0.085em tracking |
| Emphasis | Playfair Display, 500 weight, coral |
| Section title | Playfair Display, 500 weight |
| Eyebrows | Mono, 10 px, uppercase |
| Orbit labels | Mono, small, with high contrast |

### Shapes and Imagery

- Create a circular hero field.
- Use three intersecting elliptical paths.
- Represent community actions with circular nodes:
  - Listen
  - Show Up
  - Share
- Place a coral central "Fan Power" core at the center.
- Add a handwritten-like sticker to reinforce warmth and participation.

## Page Structure

1. **Header:** Wordmark, navigation, and all-directions link.
2. **Hero:** Community proposition and a visual orbit system.
3. **The idea:** Shared-momentum story with two-column copy.
4. **Member moments:** Fresh studio work, listening rooms, and community editions.
5. **About:** Forward motion and independent music.
6. **Why it works:** Rationale for the open, optimistic system.
7. **Contact:** Cobalt contact panel with lime emphasis.
8. **Footer:** Shared brand message.

## Component Specifications

### Orbit Hero

- Desktop: 0.85:1.15 copy-to-art ratio.
- Minimum hero height: 630 px.
- Use a circular or near-circular art container.
- Use at least three crossing ellipses at varied rotations.
- The central core should be about 21% of the artwork width.
- Orbit nodes should be 75 px circles on desktop.

### Navigation

Use the shared `details` menu. Links should be concise and point to the page sections.

### Perk Cards

- Three-column desktop grid.
- Cobalt icons.
- One numbered label, one icon, one heading, and one supporting paragraph per card.
- Separate cards with shared 1 px rules.

### Buttons

- Primary: cobalt `#264bbc` background.
- Contact section: existing light button styling for contrast.
- Secondary: underlined text link with arrow.

## Responsive Behavior

- At 800 px or less: reduce content and art padding while retaining the two-column hero.
- At 560 px or less:
  - Stack hero copy and orbit art.
  - Center the artwork and cap it at 410 px wide.
  - Set hero artwork to a 96vw height with a 410 px maximum.
  - Convert story and perk sections to a single column.

## Accessibility

- Keep orbit diagrams hidden from assistive technology.
- Do not make "Listen," "Show Up," or "Share" the only text for explaining their purpose.
- Keep H1, H2, and H3 headings in a correct hierarchy.
- Use cobalt and coral as visual accents while preserving readable text contrast.
- Maintain keyboard focus states and reduced-motion support.

## Implementation Notes

- Source: `concepts/orbit-house.html`
- Shared styles: `styles.css`
- Concept selector: `.orbit`
- Key variables:
  - `--paper: #eff4ee`
  - `--ink: #1a2726`
  - `--muted: #586661`
  - `--line: rgba(26,39,38,.22)`
  - `--accent: #264bbc`
