# Visual language

This reference defines a calibrated dark interface system for technical products. Treat the numbers as strong defaults, not immutable brand specifications.

## Design thesis

The interface is dark, but darkness is not the design. Its character comes from:

- precise surface roles separated by very small value changes;
- compact controls inside generous page whitespace;
- large rounded containers with smaller concentric inner radii;
- technical typography paired with restrained display type;
- selective elevation for active or floating material;
- very limited bright color;
- product demonstrations that carry more visual weight than decoration.

## Semantic surface ladder

Use each tone for one job. Do not create arbitrary near-black variants.

| Role | Dark default | Light default | Use |
|---|---:|---:|---|
| Page | `#121212` | `#fdfdfd` | Site canvas |
| Stage | `#131313` to `#171717` | `#f9f9f9` | Preview, code, embedded visual |
| Card | `#181818` to `#1a1a1a` | `#ffffff` | Bounded editorial unit |
| Floating panel | `#1b1b1b` | `#ffffff` | Controls, dropdowns, menus |
| Hover | `#1c1c1c` or white at 6–8% | black at 3–5% | Pointer affordance |
| Selected | white at 8–10% or `#2a2a2a` | black at 6–8% | Current state |

Separate adjacent dark surfaces with one or more of:

- a 1px ring at white 4–7%;
- a faint top-edge inset highlight;
- a soft material shadow for floating surfaces only;
- a meaningful spacing break.

Avoid high-contrast borders. The result should be legible at a glance but quiet when viewed peripherally.

## Color

- Primary text: near-white (`#fbfbfb` or `#ffffff`).
- Supporting text: cool neutral around `#b1b1b1`.
- Muted labels: `#979797` or white at roughly 55–65%.
- Faint metadata: `#767676` to `#8f8f8f`.
- Primary accent: crisp blue around `#0071fc`.
- Optional informational accent: cyan around `#55cfff`.

Use the blue for primary conversion, a meaningful next step, or numbered instructional markers. Routine active tabs should normally use neutral material contrast. Never make blue a decorative wash across the page.

## Typography

Use the project's type system when one exists. Otherwise:

- interface/body: `Inter`, `SF Pro Text`, or a clean system sans;
- code/technical values: `Roboto Mono`, `SFMono-Regular`, or a system mono;
- display: a restrained grotesk already licensed by the project, falling back to the sans stack.

Recommended roles:

| Role | Size / line height | Notes |
|---|---|---|
| Marketing hero | 44px / 1.15 | 30–32px mobile; slightly tight tracking |
| Product detail title | 36px / 42px | Left aligned |
| Section title | 30px / 36px | 23–24px mobile |
| Card title | 15–18px / 22–24px | Medium weight |
| Body | 14–16px / 21–24px | Keep measure controlled |
| UI label | 13px / 14–18px | Medium for controls |
| Eyebrow/meta | 11–13px / 14–18px | Muted, never tiny for novelty |
| Code | 12–13px / 1.7 | Comfortable scanning |

Keep long-form prose around 60–75 characters per line. Use tabular numerals for prices, timers, or changing values.

## Spacing rhythm

Think in nested levels:

| Level | Typical range | Examples |
|---|---:|---|
| Page section | 88–112px | Major narrative break |
| Section heading to content | 28–40px | Heading into grid or FAQ |
| Grid gap | 18–24px | Cards and framed visuals |
| Card padding | 24–32px | Editorial cards |
| Panel padding | 16px | Tool controls |
| Component group | 12–16px | Fields or button groups |
| Label to control | 8px | Form field |
| Inline relation | 4–8px | Icon plus label, metadata |

The outer relationship must feel looser than the inner one. If every gap is 16px, the hierarchy disappears.

## Radius hierarchy

- Large marketing, pricing, and testimonial cards: 24px.
- Nested stages and substantial panels: 16–18px.
- Utility panels, dropdowns, and library rows: 12px.
- Inputs, sliders, and square icon controls: 8–12px.
- Inline code: 6px.
- Segmented controls and compact CTAs: 26–48px or fully pill-shaped.

For concentric geometry, reduce an inner radius by approximately the inset distance. Example: a 24px card with a 12px inset usually wants an inner radius around 12–16px, not another 24px.

## Container geometry

- Broad outer shell: max width around 1240px, 24px desktop gutters, 12–16px mobile gutters.
- Primary editorial content: max width around 1008px.
- Documentation copy: max width around 686px.
- FAQ: max width around 640px.
- Hero supporting copy: 480–560px.

Center marketing compositions. Left-align product and documentation compositions.

## Quiet material treatment

Cards should not look like luminous glass. A useful dark card treatment is:

- card surface around `#181818`;
- 1px outer ring at white 5%;
- a faint top inset highlight;
- no large shadow unless the card is floating;
- hover value shift of only a few percentage points.

Add a real soft shadow only to dropdowns, popovers, active sliding indicators, or floating tool panels. Elevation communicates layer, not decoration.
