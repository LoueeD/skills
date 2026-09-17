# Components and composition

Use components according to their information role. Similar-looking controls are not interchangeable.

## Navigation

Desktop navigation is compact and pill-oriented:

- shell padding: about 16px vertically and 24px horizontally;
- brand-to-nav gap: about 34px;
- nav item: 36px high, 14px inline padding, fully rounded, 13px medium text;
- utility icon: 36×36px, circular or pill-like;
- right-side action gap: about 8px.

On mobile, collapse supporting brand text if necessary and move navigation into a blurred full-screen layer. Use 20px links at roughly 24px vertical intervals and a 44px primary action. Keep the header itself visually quiet.

## Marketing cards and grids

The home-style grid uses equal editorial cards:

- content width: 1008px;
- three columns with 24px gaps;
- card proportion near 320×344px;
- 24px outer radius;
- 16px inner stage radius with a 12px inset;
- 16px metadata inset near card edges.

At medium widths, use two columns and cap the grid near 664px. Below roughly 740px, use one column with 16px gaps. Do not squeeze three cards into narrow columns.

Use cards for bounded stories, demos, testimonials, and pricing. Do not place ordinary feature bullets or FAQ entries in cards by default.

## Product detail and documentation

A strong detail layout uses:

- 200px navigation rail;
- 56px gap between navigation and content;
- 32px top padding and generous bottom breathing room;
- sticky navigation around 84px from the viewport top;
- navigation rows 40px high with 8px inline padding and 12px radius;
- group labels around 11px and link labels around 13px.

At tablet widths, transform the rail into a horizontal, scrollable strip. Do not leave a cramped mini-sidebar.

Detail headers use a 46px product icon with a 12px radius, a 36px title, and a 16px subtitle. Keep about 12px between title and description and roughly 21px between major header groups.

## Tabs versus segmented controls

Use a pill segmented control when selecting one compact state from a small set, such as preview/code or monthly/yearly:

- 36px outer height;
- 3px internal padding;
- 30px sliding indicator;
- fully rounded shell;
- 12px inline label padding;
- neutral selected material, not blue.

Use plain text tabs for major identity choices such as Solo versus Team. Separate them with spacing and type weight; avoid nesting them inside another pill. This makes the hierarchy visibly different from a small mode switch.

## Buttons and utilities

- Standard CTA: 40px high, 16px inline padding, 26px radius, 13px medium.
- Compact hero CTA: 32px high with 12px inline padding only when the page is otherwise spacious.
- Touch CTA: at least 44px high.
- Copy/theme/overflow action: square ghost button, 32–36px, 8–10px radius or circular in the top bar.

Utility actions start transparent and gain a quiet fill on hover/focus. Primary actions may use blue. Avoid multiple competing blue actions in one region.

## Interactive playground

Prefer this order:

1. Live stage.
2. Narrow controls panel.
3. Implementation code.

The stage should dominate. A useful desktop composition is `minmax(0, 1fr) 244px` with a 12–24px gap. Stack below roughly 860px.

Stage defaults:

- minimum height: 380px for general demos, around 480px for voice/conversation demos;
- 16px radius;
- flat stage surface around `#171717`;
- generous internal padding, commonly 40–48px for a focused demo;
- focused content measure around 370px when showing conversation or voice content.

Control panel defaults:

- 16px radius and 16px padding;
- 16px between groups;
- 8px between label and control;
- 13px labels;
- full-bleed hairline separators between larger groups when useful.

Active controls should look slightly lifted through neutral material and a delicate ring/shadow. Avoid neon fills.

## Sliders, swatches, and inputs

- Compact choice pill: 32px high, 12px inline padding, 36px radius, 4px gap.
- Slider/value well: 32px high, 8px radius, visible fill, and a narrow grab indicator.
- Swatch: about 26px; selected state uses an external color ring plus an internal separation ring.
- Text input/composer: 39–44px minimum, 12px radius, 12px inline padding.

Use native inputs under the styled layer where possible. Labels remain visible; placeholders are examples, not labels.

## Code blocks

Implementation code is a flat stage, not a glossy card:

- background around `#171717`;
- 16px radius;
- 24px block and 26px inline padding;
- 12–13px mono text with 1.7 line height;
- copy button at the top-right, about 32×32px with 9px radius;
- subtle horizontal overflow fades for long lines.

Code follows the interactive demonstration so the story moves from experience to configuration to implementation.

## Conversation UI

Differentiate speaker roles structurally:

- user messages: compact bubbles, maximum width around 88%, 14px or pill radius;
- assistant/system response: mostly plain text without a bubble;
- applied changes or tool receipts: mono text with a quiet left rule;
- composer: low, broad field with a 28×28px send action.

Do not put every message in the same bubble. The asymmetric treatment improves scanning and makes automated actions legible.

## Feature landing page

Recommended sequence:

1. Centered hero with an eyebrow/product marker.
2. Product imagery or demonstrations.
3. Open feature columns.
4. Line-separated FAQ.

Hero geometry:

- 44px title, roughly 620px maximum width;
- 16px supporting copy, 480px maximum width, 16px below the title;
- CTA row 24px below, approximately 11px gap;
- 56–64px vertical breathing room.

For a two-column visual mosaic, a strong asymmetric ratio is roughly 497:334 with a 24px gap. Let the larger item span two rows when it tells the primary story. Preserve media aspect ratios on mobile instead of assigning arbitrary fixed heights.

Feature lists should often be open columns rather than cards: three columns, about 272px each, with generous 80–100px gutters. Stack to one column with 40px vertical gaps on mobile.

FAQ entries should be 16px vertical rows separated by hairlines. Avoid carding every question.

## Instruction cards

For a three-step process:

- three columns with 18px gaps;
- 32px card padding, 24px radius, 20px internal gap;
- 21×21px numbered marker with a soft halo;
- 15px title and 14px body;
- product example area about 220px high, bleeding to the bottom and sides of the card.

Collapse to two columns, allowing an odd final card to span when compositionally helpful, then to one column below phone width. Reduce padding to 24px.

## Pricing and testimonials

Pricing cards:

- about 325px wide, 325px minimum height;
- 20px padding, 24px radius, 24px internal rhythm;
- price at 36/42 with tabular numerals;
- feature rows at 13/20 with 12px vertical gap;
- full-width 40px CTA.

Keep billing period in a neutral segmented control. Keep plan identity as plain text tabs or separate headings.

Testimonial cards:

- three columns with 18px gaps;
- 240px minimum height;
- 32px padding and 24px radius;
- 16/24 quote;
- 36px avatar with an 11px gap to author details.

Use genuine project content. Never copy testimonials or names from a reference product.
