# Responsive, motion, and accessibility

Apply this checklist before declaring the interface complete.

## Responsive behavior

### Desktop to tablet

- Reduce a three-column editorial grid to two columns rather than shrinking cards below their useful width.
- Convert a sticky documentation rail into a horizontal scroll strip around 900px.
- Stack playground stage and 244px control rail around 860px.
- Reflow supporting pricing notes below the billing control when the row becomes crowded.
- Preserve deliberate image ratios; do not use a single arbitrary height for every viewport.

### Tablet to phone

- Use 12–16px page gutters.
- Reduce 44px hero titles to about 30–32px and section titles to 23–24px.
- Reduce large section gaps from 88–112px to 56–64px.
- Reduce card padding from 32px to 24px and grid gaps to 12–16px.
- Stack open feature columns with about 40px gaps.
- Keep primary touch actions at least 44px high.
- Allow tables and code to scroll within their own region; do not force the whole page wider.
- Collapse secondary brand text before crowding core navigation.

Use logical properties (`padding-inline`, `margin-block`) where practical. Check at intermediate widths, not only a desktop and one phone preset.

## Motion grammar

Motion is brief and material:

- micro response: 80ms;
- quick hover/state change: 150ms;
- fast panel or indicator: 250ms;
- medium reveal: 350ms;
- slow narrative reveal: 400–500ms;
- list stagger: around 40ms per item.

Preferred easing:

```css
--ease-smooth: cubic-bezier(.22, 1, .36, 1);
--ease-bounce: cubic-bezier(.34, 1.36, .64, 1);
```

Use small distances—typically 4, 6, 8, or 12px—and scale changes around `.96` to `.99`. Blur of 2–3px can soften a state swap; reserve 8px blur for a larger entrance.

Animate only `opacity`, `transform`, and narrowly scoped color/shadow properties when possible. Never use `transition: all`. Place hover styles behind `@media (hover: hover)`.

Use bounce easing sparingly for a small control or selected indicator. It should never make the whole page feel spring-loaded.

Honor reduced motion:

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    scroll-behavior: auto !important;
    animation-duration: .01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: .01ms !important;
  }
}
```

## Interaction states

Define all applicable states:

- default;
- hover;
- keyboard focus;
- pressed;
- selected/current;
- disabled;
- loading;
- success/error when relevant.

Keep selected and hover distinguishable. A selected row may use an 8% white fill and ring; hover might use only 5–6%. Pressed controls may scale to `.97` when appropriate.

## Accessibility checklist

- The first focusable item is a skip link that becomes visible on focus.
- Use real `button`, `a`, `input`, `select`, `textarea`, and heading elements.
- A navigation action uses a link; an in-place action uses a button.
- Every icon-only action has an accessible name and a visible tooltip where useful.
- Focus is clearly visible and not clipped by rounded overflow containers.
- Do not communicate status or selection by color alone.
- Body copy and muted labels meet contrast requirements against their actual surface.
- Form labels remain visible; errors are connected to their field and announced appropriately.
- Dynamic status uses `role="status"` or an appropriate live region without stealing focus.
- Drawers, popovers, and modals manage focus, Escape, and focus restoration.
- Decorative imagery has empty alt text; meaningful imagery has specific alt text.
- Text regions can grow without clipping; avoid fixed heights around content.
- Support zoom to 200% and reflow at narrow widths.

## Optical quality checklist

- Icons are visually centered, not merely mathematically centered.
- One-pixel rules align to the pixel grid.
- Nested corners are concentric.
- Images have a subtle inset outline when their edge could disappear into the surface.
- Label/control gaps are smaller than group/group gaps.
- Baselines align across mixed icon-and-text rows.
- Muted text is still readable; avoid opacity stacking that accidentally lowers contrast.
- A page has one obvious primary action per decision region.
- Decorative effects do not compete with the product demonstration.

## Failure patterns to remove

- Uniform 16px gaps everywhere.
- The same radius on parent and child containers.
- Blue active states for every control.
- Every content block inside a card.
- Large ambient gradients, neon glows, or generic glassmorphism.
- Overlarge hero text that pushes the product below the fold.
- Emoji used as product icons.
- Identical bubbles for every conversational role.
- Tooltips that contain essential information unavailable elsewhere.
