# Editable PPTX reconstruction rules

## Contents

1. Reconstruction objective
2. Object mapping
3. Common slide system
4. Typography implementation
5. Hybrid-image rules
6. Authoring workflow
7. Verification and handoff

## 1. Reconstruction objective

Recreate the approved slide images as a highly editable PPTX while preserving visual fidelity, hierarchy, and presentation legibility.

Use the slide images as visual references. Do not place each full slide image as the only object unless the user explicitly requests a flattened deck.

## 2. Object mapping

Rebuild as native editable objects:

- Titles, subtitles, body copy, labels, footnotes, sources, and page numbers
- Cards, backgrounds, dividers, badges, emphasis bands, and callout boxes
- Tables, comparison structures, timelines, roadmaps, matrices, and decision rows
- Simple process flows, connectors, arrows, circles, icons, and layered architectures
- Charts when the exact data is available

Keep as separate image objects when native reconstruction would materially reduce fidelity or require excessive manual redrawing:

- Photographs
- Generated product or equipment scenes
- Complex illustrations
- Detailed screenshots and document evidence
- Highly detailed infographic artwork without source vectors

Keep supplied logos as separate high-resolution image objects. Never merge them into the slide background.

## 3. Common slide system

Define and reuse:

- Slide size and 16:9 coordinate system
- Horizontal and vertical safe margins
- Header line and logo row
- Title, subtitle, body, caption, source, and page-number coordinates
- Font family and scale
- Color tokens
- Corner radii, strokes, arrow styles, connector styles, and shadow policy
- Footer and source-note rule

Use the same coordinates for equivalent elements on every page.

Create all pages from one shared set of helper functions or master-like constants when programmatic authoring is used.

## 4. Typography implementation

Use exactly these font faces:

- Slide title and subtitle: `Pretendard ExtraBold`
- Body copy, labels, tables, charts, captions, sources, footnotes, page numbers, and all other text: `Pretendard`

Never use PowerPoint's built-in Bold property.

- Set every text shape and every rich-text run to `bold: false`, or omit the bold property only when the runtime guarantees that no master, placeholder, or inherited style applies bold
- Never set `bold: true`
- Do not use `Pretendard Bold`, `Pretendard SemiBold`, another weight face, font-weight simulation, or synthetic emphasis
- Create emphasis through font size, color, spacing, alignment, placement, or a separate shape
- Keep the font face constant inside each text role and do not mix regular and ExtraBold runs inside body paragraphs
- Use `fontFace: "Pretendard ExtraBold"` with `bold: false` for titles and subtitles in programmatic authoring
- Use `fontFace: "Pretendard"` with `bold: false` for every other text object in programmatic authoring

Use the approved deck-wide font-size scale. Adjust size rather than weight, but do not reduce body, label, caption, or source text below the approved legibility minimum to fit excessive copy.

Before authoring, verify that both exact font faces are available in the runtime. If either font is unavailable, do not substitute silently; pause and resolve the font installation or obtain the required font asset.

After PPTX export, inspect the OOXML package and reject the file if any text property in slides, layouts, or masters contains built-in bold such as `b="1"` or `b="true"`. Correct the source objects, export again, and repeat the scan.

## 5. Hybrid-image rules

- Crop source slide images outside the PPTX when exact image-crop behavior is unreliable
- Use tight transparent crops for logos and cutout visuals
- Keep raster text out of image objects whenever practical
- Avoid duplicated titles or subtitles inside cropped infographic regions
- Ensure cropped images do not contain partial labels, borders, callouts, or footer fragments
- Place complex image objects behind native labels and callouts when editability benefits from separation
- State the rasterized elements in the final handoff

## 6. Authoring workflow

Use the applicable `Presentations` skill and its supported authoring runtime.

1. Read the presentation-authoring instructions completely
2. Create the required artifact-operation marker once when instructed
3. Load all source slide images and original brand assets
4. Establish the common slide system
5. Build each slide with native objects and separate images
6. Add compact source notes or speaker-note sources when required
7. Export the PPTX
8. Render every exported slide
9. Compare the rendered PPTX with the approved slide image
10. Correct layout, font, crop, overlap, and fidelity issues
11. Scan the PPTX text properties for prohibited built-in bold attributes
12. Run the available overflow or presentation tests
13. Deliver only after all tests pass

Do not use unsupported presentation libraries when the applicable presentation skill mandates a specific toolchain.

## 7. Verification and handoff

Inspect every slide, not only a montage:

- Text presence, Korean font rendering, wrapping, and overflow
- `Pretendard ExtraBold` applied to every title and subtitle with built-in Bold disabled
- Regular `Pretendard` applied to every other text element with built-in Bold disabled
- No prohibited built-in bold attribute in slide, layout, or master text properties
- Object boundaries, alignment, spacing, and safe margins
- Logo fidelity and proportions
- Crop boundaries and unintended duplicate content
- Connector direction and arrow placement
- Page numbering and footer consistency
- Slide count and order
- File integrity and successful rendering

At delivery, state concisely:

- Total page count
- Native editable element types
- Raster image-object element types
- Verification performed

Do not claim complete editability when complex visuals remain raster images.
