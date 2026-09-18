# Interactive documentation

Use this archetype for compact educational sites where the reader should understand a principle by manipulating it. It is not a replacement for broad API documentation, an operational playbook, or a marketing page.

## Page sequence

Build each concept page in this order:

1. State one concise principle in the title and opening paragraph.
2. Let the reader experience it in a live demonstration.
3. Explain the decision rule and important exceptions.
4. Show the implementation in runnable or copyable code.
5. Cite useful source material without interrupting the lesson.
6. End with previous and next concepts.

Keep the primary article near 640px. On desktop, use 28–32px inline gutters, about 112px above the article, and about 96px below it. On phones, use 16px gutters and reduce the vertical lead proportionally.

Suggested type geometry:

- page title: 18px, medium;
- section title: 16px, medium, with about 40px above and 16px below;
- subsection title: 14px, medium, with about 32px above and 12px below;
- body: 14px with approximately 1.8 line height;
- paragraphs: about 16px apart;
- code: 12px with approximately 1.625 line height.

The compact type is intentional. Preserve legibility through line height, measure, and contrast rather than enlarging every heading.

## Demonstration canvas

Prefer an open canvas over a card when the demo already has clear visual boundaries:

- minimum height: 192px;
- 24px inline and 40px block padding;
- 24px internal gap;
- about 32px margin above and below;
- center a single focused behavior rather than simulating an entire product.

Use a bounded card only when the example needs its own material, clipping, or independent elevation. A reader should immediately see which parts are instructional chrome and which part is the behavior under study.

## Comparison demonstrations

For a wrong/right or before/after lesson:

- use two equal-width columns up to about 512px total;
- use a 12px gap at narrow widths and up to 40px when space allows;
- keep examples at the same scale and apparent weight;
- identify status with text and an icon in addition to color;
- place short captions directly below the examples.

Do not exaggerate the wrong example. Teach the smallest meaningful difference so the comparison remains credible.

## Concept index

Use one column on phones and two columns when each tile retains a useful demonstration area. A practical tile has an approximately 144px stage, a 16px footer, 13px title, 12px description, and a radius near 18px. Use about 16px between tiles.

Unavailable concepts must look and behave disabled. Prefer hiding them behind an explicit preview filter or labelling them as upcoming instead of exposing empty links.

## Utility header and navigation

A fixed utility header can stay quiet while the article scrolls. Use it only when those utilities matter:

- use roughly 32px inline and 26px block placement on desktop;
- keep theme, search, source, and menu actions as ghost icon buttons;
- give every icon action a 44px target on touch screens, even if the visible glyph or circle is smaller;
- open search with Command/Ctrl+K when that shortcut is not already claimed.

For a small concept set, a faded desktop rail can sit outside the article measure. A width near 224px is usually enough. Choose either the rail or header links for concept destinations. On mobile, use an inset sheet—about 12px from the viewport edge and up to 256px wide—with a generous radius only if that shape belongs to the surrounding system.

A command palette is justified only when the concept set is large enough to need search. It can use a maximum width around 448px, at least 32px viewport clearance, a 48px search row, and a scrollable result list around 288px high. Manage focus, Escape, and focus restoration like a modal dialog.

## Code and source access

- Put an optional filename or language label in a quiet header above the code.
- Use real tab semantics and arrow-key behavior when switching between implementations.
- Keep copy control accessible and announce success through a status region.
- Animate a code panel's height only when the change helps preserve spatial context.
- Offer a canonical page and, when useful for agents or power users, a Markdown mirror or copy-as-Markdown action.
- Prefetch an adjacent lesson on hover or focus only when it produces a measurable navigation benefit.
- Do not publish placeholder content, private notes, or unavailable routes through the Markdown mirror.

## Interaction and accessibility

- Begin with a visible-on-focus skip link.
- Use native semantic controls inside demonstrations.
- Express mutually exclusive choices with tabs, a radio group, or a correctly labelled group of pressed buttons.
- Never make color the only wrong/right, active, success, or error signal.
- Keep sound off by default and provide an explicit remembered preference if sound materially helps the lesson.
- Keep the visual hierarchy intact at 200% zoom and when examples stack.

## Boundaries

Borrow the structural discipline, not another product's identity. Do not reproduce its name, wordmark, prose, proprietary media, or distinctive illustration set.
