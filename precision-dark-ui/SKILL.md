---
name: precision-dark-ui
description: "Design or refine authored developer-product interfaces in a precise dark-material visual language: quiet near-black surfaces, deliberate hierarchy, measured geometry, restrained accents, and subtle motion. Use for landing pages, library documentation, internal playbooks, interactive concept guides, AI playgrounds, developer tools, pricing, or design-system work when this direction is requested. Do not use when another established design system should govern."
---

# Precision Dark UI

Create calm, precise interfaces for technical products. Preserve the project's identity and content; apply the design grammar without copying a reference product's branding, copy, logos, screenshots, testimonials, or proprietary typefaces.

## Start here

1. Inspect the existing app, framework, tokens, reusable components, content, and real assets before editing.
2. Identify the page archetype from the user's task—not from the components you want to use: marketing grid, product detail/playground, product documentation, internal playbook, interactive concept guide, feature landing page, pricing, or mixed.
3. Write a one-sentence visual thesis tied to the product or content. Name the dominant information form and the one navigation model before choosing surfaces.
4. Read [references/visual-language.md](references/visual-language.md) for the core system.
5. Read [references/components-and-composition.md](references/components-and-composition.md) for the relevant archetype and component roles.
6. For an operational guide, checklist, standard, or internal playbook, read [references/internal-playbooks.md](references/internal-playbooks.md).
7. For an educational surface built around live demonstrations, read [references/interactive-documentation.md](references/interactive-documentation.md).
8. Before finishing, apply [references/responsive-motion-accessibility.md](references/responsive-motion-accessibility.md) and [references/authored-quality-gates.md](references/authored-quality-gates.md).
9. Use [assets/theme-tokens.css](assets/theme-tokens.css) only as an optional token and primitive source. Select what the composition needs; do not import it as a complete visual template.

## Working method

### 1. Model the content before decoration

Build in this order:

1. User task and retrieval path.
2. Information forms: sequence, comparison, reference, evidence, controls, or narrative.
3. One dominant organizing device and one navigation model per viewport.
4. Page background, width constraints, and surface roles.
5. Layout ratios, spacing rhythm, type hierarchy, and line length.
6. Controls, interaction states, motion, responsive behavior, and accessibility.

Do not begin with a hero, glows, gradients, pills, or generic cards. The style comes primarily from product-specific structure, proportion, restrained contrast, and the correct element for each job.

### 2. Use a small, deliberate scale

- Favor an 8px rhythm with optical exceptions at 6, 12, 18, and 24px.
- Keep group gaps at least twice their internal label-to-control gaps.
- Use concentric radii: a nested surface must look related to its parent.
- Choose motion by interaction frequency and intent before choosing a duration.
- Reserve blue for decisive progression, conversion, or numbered guidance—not routine selection.
- Let content visuals bleed to card edges when they are part of the card's story.
- Use hairline rows, open columns, or plain text when a card would add no semantic boundary.
- Use only font weights the loaded font actually provides. A small scale such as 400/500/600 is preferable to arbitrary intermediate values.
- Reserve monospace for code, identifiers, changing values, or genuinely technical metadata—not as a default signal that a page is “developer focused.”

### 3. Compose by product intent

- Marketing pages: centered hero, restrained copy width, editorial card grid, quiet footer.
- Product details: left-aligned title, sticky or horizontally scrollable navigation, stage first, controls second, implementation code last.
- Interactive playgrounds: dominant preview with a narrower control rail; stack cleanly on smaller screens.
- Internal playbooks: modest title, immediate orientation, compact reference tool, open operational sequence, worked evidence, then checklist or template.
- Interactive guides: concise principle, live demonstration, explanation, implementation, sources, then adjacent navigation.
- Feature pages: show the product through real framed visuals, then open feature columns, then line-separated FAQ rows.
- Pricing: keep plan identity, billing period, price, benefits, and CTA as separate visual layers.

### 4. Verify visually and reject template output

Render the page at desktop, tablet, and narrow mobile widths. Compare:

- outer gutters and maximum widths;
- card padding versus inter-card gap;
- parent/child corner relationships;
- width ratios between preview and controls;
- line lengths, baseline rhythm, and optical alignment;
- hover, focus, pressed, selected, disabled, loading, and reduced-motion states.
- the blurred silhouette: repeated rounded rectangles must not dominate;
- whether the same composition could plausibly sell an unrelated AI product after replacing the copy.

If the page merely looks “dark and rounded,” or remains convincing after swapping in unrelated product copy, the skill has not been applied deeply enough. Revise the content structure and organizing device before tuning decoration.

## Non-negotiable boundaries

- Do not recreate a reference product's branding or claim affiliation.
- Do not copy its logo, marketing copy, testimonials, screenshots, videos, or proprietary font files.
- Do not force this style over an established product design system without explicit direction.
- Do not use `transition: all`, color-only state communication, inaccessible custom controls, or fixed-height text containers.
- Do not turn every section into a rounded card or every active state into a blue pill.
- Do not invent a faux logo, badge, or brand mark for an unbranded tool or internal document.
- Do not combine a giant transformational headline, uppercase accent eyebrow, glassy header, pill navigation, glowing numbered markers, and rounded statement card as a default composition.
- Do not show two navigation systems for the same destinations in one viewport.
- Do not repeat the same bordered component more than three times when an open list, table, timeline, or grouped sequence would scan better.
- Do not use text symbols, emoji, handcrafted SVGs, or CSS drawings as substitute interface icons. Use the host product's icon system or a coherent library.
