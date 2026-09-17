---
name: precision-dark-ui
description: "Design or refine developer-product interfaces in a precise dark-material visual language: quiet near-black surfaces, stage-first cards, pill state controls, measured radii, restrained blue accents, and subtle micro-motion. Use for landing pages, library documentation, AI playgrounds, developer tools, pricing, or design-system work when this direction is requested. Do not use when another established design system should govern."
---

# Precision Dark UI

Create calm, precise interfaces for technical products. Preserve the project's identity and content; apply the design grammar without copying a reference product's branding, copy, logos, screenshots, testimonials, or proprietary typefaces.

## Start here

1. Inspect the existing app, framework, tokens, and reusable components before editing.
2. Identify the page archetype: marketing grid, product detail/playground, documentation, feature landing page, pricing, or mixed.
3. Read [references/visual-language.md](references/visual-language.md) for the core system.
4. Read [references/components-and-composition.md](references/components-and-composition.md) for the relevant archetype and component roles.
5. Before finishing, apply [references/responsive-motion-accessibility.md](references/responsive-motion-accessibility.md).
6. Use [assets/theme-tokens.css](assets/theme-tokens.css) only as an optional starter. Adapt its semantic tokens to the project's existing system rather than layering on duplicate globals.

## Working method

### 1. Establish hierarchy before decoration

Build in this order:

1. Page background and width constraints.
2. Surface roles: page, card, stage, floating panel, selected control.
3. Layout ratios and spacing rhythm.
4. Type hierarchy and line length.
5. Controls and interaction states.
6. Motion, responsive behavior, and accessibility.

Do not begin with glows, gradients, or generic cards. The style comes primarily from proportion, restrained contrast, and the correct element for each job.

### 2. Use a small, deliberate scale

- Favor an 8px rhythm with optical exceptions at 6, 12, 18, and 24px.
- Keep group gaps at least twice their internal label-to-control gaps.
- Use concentric radii: a nested surface must look related to its parent.
- Reserve blue for decisive progression, conversion, or numbered guidance—not routine selection.
- Let content visuals bleed to card edges when they are part of the card's story.
- Use hairline rows, open columns, or plain text when a card would add no semantic boundary.

### 3. Compose by product intent

- Marketing pages: centered hero, restrained copy width, editorial card grid, quiet footer.
- Product details: left-aligned title, sticky or horizontally scrollable navigation, stage first, controls second, implementation code last.
- Interactive playgrounds: dominant preview with a narrower control rail; stack cleanly on smaller screens.
- Feature pages: show the product through real framed visuals, then open feature columns, then line-separated FAQ rows.
- Pricing: keep plan identity, billing period, price, benefits, and CTA as separate visual layers.

### 4. Verify visually

Render the page at desktop, tablet, and narrow mobile widths. Compare:

- outer gutters and maximum widths;
- card padding versus inter-card gap;
- parent/child corner relationships;
- width ratios between preview and controls;
- line lengths, baseline rhythm, and optical alignment;
- hover, focus, pressed, selected, disabled, loading, and reduced-motion states.

If the page merely looks “dark and rounded,” the skill has not been applied deeply enough. Refine the hierarchy and element roles.

## Non-negotiable boundaries

- Do not recreate a reference product's branding or claim affiliation.
- Do not copy its logo, marketing copy, testimonials, screenshots, videos, or Saans font files.
- Do not force this style over an established product design system without explicit direction.
- Do not use `transition: all`, color-only state communication, inaccessible custom controls, or fixed-height text containers.
- Do not turn every section into a rounded card or every active state into a blue pill.
