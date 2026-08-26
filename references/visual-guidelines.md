# Visual guidelines

## Contents

1. Deck-wide system
2. Typography system
3. Page anatomy
4. Visualization selection
5. Asset fidelity
6. Image-generation workflow
7. Post-generation inspection

## 1. Deck-wide system

Define one visual system before generating the first page:

- Canvas and safe margins
- Header, subtitle, footer, source note, page number, and logo coordinates
- Typography family, title scale, subtitle scale, body scale, caption scale, and number emphasis
- Background, primary text, structural, accent, risk, and neutral colors
- Grid, column widths, spacing increments, corner radii, stroke weights, icon family, and shadow policy
- Photograph, screenshot, product render, and diagram treatment

Carry these values forward unchanged unless a deliberate section-divider variation is required.

## 2. Typography system

Use only these two text font faces across the deck:

- Slide title and subtitle: `Pretendard ExtraBold`
- Body copy, section labels, tables, chart labels, callouts, captions, source notes, footnotes, page numbers, and every other text element: `Pretendard`

Do not use `Pretendard Bold`, `Pretendard SemiBold`, another weight variant, synthetic bold, or an application's built-in Bold control.

Build hierarchy through font size, color, spacing, alignment, and placement instead of additional font weights.

Use this default size system and adjust within the range only when content density or presentation distance requires it:

- Cover title: 34 to 44 pt
- Slide title: 26 to 32 pt
- Subtitle: 17 to 21 pt
- Key number: 28 to 40 pt
- Body copy: 14 to 18 pt
- Labels and table text: 12 to 15 pt
- Captions and source notes: 8 to 11 pt
- Page number: 9 to 12 pt

Keep equivalent elements at the same size throughout the deck. Do not shrink one page below the approved minimum to accommodate excessive copy; shorten or restructure the content instead.

For generated slide images, explicitly request the approved typeface appearance and reject synthetic-bold or mixed-weight results. Treat the editable PPTX typography as the exact implementation of the font rule.

## 3. Page anatomy

Preferred structure:

- Top: section label, title, and optional subtitle
- Center: one dominant visual relationship
- Support: two to five evidence blocks, labels, or callouts
- Bottom: implication, decision line, evidence caption, source note, and page number

Keep essential content at least 5 percent from every edge. Keep footer content at least 3 percent above the bottom and inside the horizontal safe margin.

Avoid repeating five equal rounded cards when the ideas have a different relationship.

## 4. Visualization selection

Choose by relationship:

- Sequence or operating model: process flow or layered architecture
- Before and after: two-column contrast with a visible transition
- Performance or market: one primary chart plus two or three takeaways
- Roadmap: phases, deliverables, gates, and outcomes
- Product or service: hero visual with callouts and benefit mapping
- Roles or governance: responsibility chain or RACI-like structure
- Evidence: real document, screenshot, certification, contract, customer signal, or quantified validation
- Decision request: limited options, required approvals, and the immediate next step
- System boundary: input → processing → output architecture
- Portfolio or multi-use value: hub-and-spoke map

Use exact charts for exact data. Do not use generative imagery for precise numeric charts or diagrams that must remain accurate.

## 5. Asset fidelity

- Preserve supplied brand marks without recoloring, redrawing, stretching, or adding effects
- Preserve real faces, body proportions, product forms, document evidence, seals, and screenshots when fidelity is requested
- Use high-resolution originals when available
- Keep logos and evidence assets as separate elements for later PPTX reconstruction
- Do not fabricate official proof
- Use labeled placeholders for missing evidence

## 6. Image-generation workflow

For every page:

1. Load the approved page specification
2. Reuse the deck-wide visual system
3. Confirm required exact assets
4. Generate one horizontal 16:9 slide image
5. Inspect the actual output
6. Correct defects
7. Reinspect before accepting the page

For corrections, modify only the requested elements unless broader rework is necessary to remove a defect.

## 7. Post-generation inspection

Check every generated page at practical presentation size and full resolution:

- Korean glyph corruption, nonsensical characters, missing syllables, duplicated letters, and typos
- Prohibited periods, narrative endings, and em dashes
- Titles, labels, numbers, units, names, dates, and source notes against the approved plan
- Text wrapping, alignment, hierarchy, contrast, and minimum legibility
- Cropping, edge collisions, overlap, distorted logos, altered faces, and changed product forms
- Horizontal 16:9 ratio and safe margins
- Header, footer, page number, source note, logo row, and typography consistency
- `Pretendard ExtraBold` appearance on titles and subtitles
- Regular `Pretendard` appearance on every other text element without synthetic bold
- Visual continuity with the adjacent pages

Correct every detected issue and inspect the corrected image again.
