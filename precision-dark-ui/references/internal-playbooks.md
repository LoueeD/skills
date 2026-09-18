# Internal playbooks and operational guides

Use this archetype for internal standards, checklists, operating procedures, review guides, runbooks, and practical reference material. The reader is trying to find, apply, and verify information—not be persuaded by a product launch.

## Design thesis

Write one sentence before implementation that ties the visual structure to the subject. Good theses name an information behavior, for example:

- evidence reads like a ledger connecting claims to observations;
- a review process reads like a sequence of gates with explicit exit criteria;
- a runbook reads like a compact operating sheet with exceptions close to the relevant step.

If the thesis only says “modern, dark, clean, or technical,” it is not specific enough.

## Information order

Prefer this sequence when the material supports it:

1. Plain title and one short orientation paragraph.
2. Immediate contents or compact quick-reference tool.
3. The operational sequence or decision model.
4. A worked example tied to the sequence.
5. Exceptions, stop conditions, or escalation rules.
6. Copyable template or checklist.

Do not turn the introduction into a marketing hero. A useful default is a 30–36px title, 15–16px introduction, and 40–56px before the first practical artifact. Omit eyebrows, version badges, and slogans unless they carry real document metadata.

## Content transformation

Model repeated information before styling it:

- sequence: numbered open rows, a timeline, or a process rail;
- repeated fields: a table, definition list, or aligned columns;
- evidence: claim-to-check mappings or a ledger;
- exceptions: line-separated alerts located beside the affected step;
- reusable prompts or templates: progressive disclosure with a clear copy action;
- final verification: native checklist or concise sign-off table.

When a pattern repeats more than three times, stop cloning a card. Compress the shared structure and let the changing information carry the rhythm.

## Geometry and rhythm

- Reading measure: usually 680–760px.
- Optional desktop contents rail: about 176–208px with a 40–56px gap.
- Major operational section spacing: 40–56px.
- Repeated step spacing: 24–36px.
- Heading-to-explanation gap: 8–12px.
- Label-to-value gap: 6–8px.
- Body copy: 14–16px with 1.55–1.7 line height.

Account for nested spacing at section boundaries. Parent padding plus the last child's padding plus the next section's padding must not create an accidental blank band.

## Surface and component budget

Use the page canvas, rules, alignment, and whitespace as the default material. A practical guide normally needs only a few bounded surfaces:

- one quick-reference or summary tool;
- one worked example or evidence artifact;
- code, prompt, or template regions that require clipping and copy controls;
- floating controls only when they actually float.

Do not box the title, every process step, ordinary explanatory prose, a table already defined by rules, and the conclusion. In a blurred or zoomed-out view, text rhythm and alignment—not a stack of rounded rectangles—should define the page.

## Navigation

Choose one destination model per viewport:

- desktop: quiet contents rail or compact top contents, not both;
- tablet: a disclosure menu is safer than a long clipped horizontal strip;
- phone: a labelled contents button and sheet, or a native disclosure before the article.

Keep utility actions such as print, copy, theme, or source separate from destination navigation. Do not invent a brand bar when the document has no real brand. A plain document title is stronger than a faux logo.

## Typography and symbols

- Use only font weights that are available in the loaded typeface.
- Prefer two or three weights across the page.
- Use monospace only for code, identifiers, commands, measured values, or actual document metadata.
- Use the host icon set or one coherent icon library. Do not use characters such as `+`, `✓`, `⧉`, arrows, or letter combinations as improvised interface icons.
- Keep semantic status text beside status icons; never rely on accent color alone.

## Implementation hygiene

Follow the host project's component and file structure. For a deliberately requested single-file artifact, keep concerns organized and still avoid inline event handlers, spacer elements, one-off inline styles, duplicated magic values, and manual controls that native semantics can replace.

Use a radio group for one-of-many modes unless the content is truly tabbed. Make all touch targets at least 44×44px, including copy, print, contents, and segmented options.

## Failure signatures

Revise the composition when several of these appear without product-specific reasons:

- a faux mark beside a generic product label;
- an oversized “from X to Y” or manifesto headline;
- an uppercase blue monospace eyebrow;
- a blurred translucent top bar;
- pill links for ordinary document navigation;
- glowing numbered squares for a long process;
- two shaded panels repeated for every step;
- a rounded statement card immediately below the introduction;
- every practical artifact wrapped in another rounded container.
