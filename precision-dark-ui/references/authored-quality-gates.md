# Authored quality gates

Apply these gates to the rendered result before handoff. They catch technically polished interfaces that still feel interchangeable or generated.

## 1. Specificity gate

Temporarily ignore the copy. Ask what visible structure belongs specifically to this product, task, or content.

Fail when replacing the name and prose would leave a plausible generic developer-tool or AI landing page. Revise the organizing device, hierarchy, or content representation—not merely the colors.

## 2. Silhouette gate

Blur, squint at, or zoom out from the screenshot.

Fail when the dominant silhouette is a vertical stack of similarly sized rounded rectangles, repeated two-column panels, or alternating card grids. Open the composition with rules, alignment, plain rows, editorial type, or one content-derived visual artifact.

## 3. Trope-accumulation gate

Count unmotivated template signals:

- faux logo or monogram;
- uppercase accent eyebrow;
- oversized transformational headline;
- translucent blurred header;
- pill navigation;
- glowing number markers;
- generic statement callout;
- default three-card grid;
- decorative gradient or glow;
- improvised symbol icons.

One justified pattern may be appropriate. Three or more without a product-specific reason is a failed composition; remove or replace the set rather than polishing it.

## 4. Component-budget gate

- Use one primary navigation model per viewport.
- Give each surface role a distinct job.
- Do not bound ordinary prose or a structure already communicated by rules and alignment.
- If the same bordered pattern repeats more than three times, test an open list, table, timeline, or grouped sequence.
- Reserve shadows for floating or selected material.

## 5. Rhythm gate

Inspect boundaries, not just individual spacing tokens. Fail when parent section padding, child padding, and adjacent section padding combine into accidental blank bands or when every relationship uses the same gap.

## 6. Type and icon gate

- Confirm every used font weight exists.
- Keep the weight scale small.
- Verify that monospace communicates technical meaning.
- Check small muted text against its real background.
- Replace text-symbol and one-off drawn icons with the established icon system.

## 7. Responsive and interaction gate

Capture at least one wide desktop, one intermediate width near navigation collapse, and one narrow phone view. Verify:

- navigation does not duplicate, truncate, or hide destinations without an affordance;
- all touch targets reach 44×44px;
- tables, code, and comparisons reflow or scroll locally;
- focus, selected, pressed, disabled, loading, and reduced-motion states remain distinct;
- direct hover and expert keyboard feedback do not lag behind input.

## 8. Implementation gate

Preserve the host architecture. Reject unexplained inline event handlers, spacer elements, scattered one-off styles, arbitrary font weights, duplicated magic values, or custom controls that native semantics can replace.

## Regression scenario

Use this scenario when evaluating meaningful changes to the skill:

> Create a practical internal guide that helps developers supervise AI-assisted coding work and decide when a change is ready for review. Include a quick reference, a six-part operating sequence, a worked example, stop conditions, a copyable evidence template, and a printable checklist.

The result should route to the internal-playbook archetype. Observable invariants:

- no marketing-scale hero or faux brand;
- one navigation model per viewport;
- the six-part sequence is not six cloned cards;
- cards are reserved for bounded tools or evidence artifacts;
- the layout has a content-derived evidence or review structure;
- intermediate navigation remains complete and usable;
- touch targets, text contrast, semantic choice controls, and implementation hygiene pass their gates.
