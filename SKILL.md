---
name: build-strategic-ppt-decks
description: "Create Korean strategic proposals, IR decks, business plans, government-support presentations, consulting proposals, product introductions, and pitch materials through a fixed end-to-end workflow: source analysis, full-deck planning, pagination, page-level planning, consistent 16:9 slide-image generation, editable PPTX reconstruction, and rendered quality assurance. Use when the user requests a complete presentation workflow, asks to proceed in the established strategic PPT style, wants generated slide images converted into a highly editable PPTX, or refers to the previous proposal, IR, image-first, or editable-deck production method."
---

# Build Strategic PPT Decks

Create one coherent strategic deck from source analysis through slide images and an editable PPTX. Treat image generation as the approved visual design stage and reconstruct the final deck with native PowerPoint objects wherever practical.

## Required references

Read only the references needed for the current stage, but read each selected file completely before acting:

- Stages 1 to 3: [references/planning-workflow.md](references/planning-workflow.md)
- Stage 4: [references/visual-guidelines.md](references/visual-guidelines.md)
- Stage 5: [references/editable-pptx-rules.md](references/editable-pptx-rules.md)
- Final delivery: [references/quality-checklist.md](references/quality-checklist.md)

When available, also use the established `build-strategic-ppt-images` skill for image-production details and the `Presentations` skill for PPTX authoring and verification. Follow their file-format and tool rules without weakening this skill's workflow.

## Default operating mode

Use the complete workflow unless the user explicitly limits the scope:

1. Analyze and enhance the full content
2. Establish pagination and narrative sequence
3. Specify every page in image-ready detail
4. Generate the full slide-image deck
5. Reconstruct and verify an editable PPTX

If the user says not to start production yet, complete only the requested planning stages. If the user requests images only, stop after stage 4. If the user requests an editable PPTX from completed images, begin at stage 5 after confirming all source images and brand assets are available.

## Autonomy rule

When the user approves the entire deck, says `진행`, requests all pages, or asks for autonomous completion:

- Continue through the final requested stage without page-by-page confirmation
- Preserve the sequence internally even when intermediate plans are not shown
- Make sensible assumptions for non-critical gaps
- Use labeled placeholders for missing non-critical evidence
- Pause only when a missing choice or asset materially changes the entire deck or makes exact fidelity impossible
- Keep progress updates brief

## Stage 1: Full-content planning

Analyze all supplied documents, images, tables, logos, prior plans, and conversation constraints before designing pages.

- Define audience, decision objective, presentation time, desired action, and evaluation context
- Extract verified facts, numbers, names, dates, claims, sources, and required evidence
- Separate supplied facts, verified external facts, assumptions, and proposals
- Identify contradictions, duplication, weak claims, missing proof, and unnecessary detail
- Build the persuasion logic around context → problem → implication → solution → proof → execution → decision
- Preserve the user's original intent while improving clarity and order
- Do not invent official proof, contracts, certifications, customer results, or exact financial values

Produce a concise strategic brief before pagination when the user requests planning review.

## Stage 2: Pagination

Assign one strategic job and one takeaway to every page.

- Determine the page count from the audience, purpose, and speaking-time budget
- Prefer fewer stronger pages over repetitive pages
- Allocate realistic explanation time to every page
- Separate context, problem, solution, proof, implementation, economics, roles, roadmap, and decision pages when each has a distinct job
- Merge pages that repeat the same conclusion
- Reorder pages when the evidence should precede the proposal
- Define page number, role, main message, key evidence, visualization, and required source

Do not finalize visual design before the page map is logically complete.

## Stage 3: Page-level planning

Convert every page into an image-ready production specification.

- Define page role and the single conclusion the audience must retain
- Finalize headline, subtitle, short body copy, labels, numbers, source note, and decision line
- Choose the correct visual relationship instead of defaulting to equal cards
- Specify grid, visual focal point, data hierarchy, diagram structure, and asset placement
- Keep each page explainable within its time allocation
- Keep essential content inside the editable-PPTX-safe area
- Plan separable layers for later PPTX reconstruction
- Request only sources that materially affect fidelity or evidence

Use the page-plan format in `planning-workflow.md`.

## Stage 4: Slide-image generation

Generate horizontal 16:9 slide images only after the page specifications are sufficiently concrete or the user has approved autonomous production.

- Use image generation for the raster slide pages
- Carry forward one deck-wide visual system across every page
- Keep header, subtitle, footer, source note, page number, margins, typography scale, and logo placement consistent
- Use supplied logos, faces, products, screenshots, documents, seals, and evidence without unauthorized alteration
- Match visualization type to the information relationship
- Prefer diagrams, charts, process flows, matrices, timelines, architecture, and annotated product scenes over paragraph-heavy layouts
- Inspect every generated image for Korean text corruption, numbers, units, names, cropping, overlap, logo fidelity, alignment, and 16:9 ratio
- Correct defects before accepting a page as final

Do not present unchecked images as verified.

## Stage 5: Editable PPTX reconstruction

Use the approved slide images as visual references, not as full-slide flattened backgrounds by default.

- Recreate titles, subtitles, body copy, labels, source notes, and page numbers as native editable text
- Recreate cards, tables, comparisons, timelines, roadmaps, flows, connectors, and simple diagrams as native editable objects
- Insert supplied logos as separate image objects
- Rebuild charts natively when the source data is known and exact
- Keep complex generated scenes, equipment renders, photographs, screenshots, and highly detailed illustrations as separate movable image objects
- Use a common coordinate system, typography scale, colors, spacing, stroke weights, corner radii, footer rules, and logo row across the entire deck
- Keep reconstruction fidelity as high as practical without sacrificing editability or legibility
- State which elements remain raster images at delivery

Use the applicable presentation-authoring capability and follow `editable-pptx-rules.md` exactly.

## Copy rules

Apply these rules to plans, slide images, and PPTX copy:

- Write primarily in Korean
- Use compressed bullets, noun phrases, and strategic-report language
- Do not end slide lines with periods
- Never use an em dash
- Avoid narrative endings such as `~합니다`, `~입니다`, `~원합니다`, `~해야 합니다`, `~필요합니다`, `~가능합니다`
- Prefer `A → B`, `A 기반 B`, `A 중심 B`, `A에서 B로 전환`, and `A·B·C 통합`
- Use headline → evidence → implication
- Keep one page focused on one message
- Use precise figures only when supplied or verified
- Label estimates and assumptions clearly
- Avoid dense paragraphs and decorative copy

## Default visual system

Unless the user provides another direction:

- Use a horizontal 16:9 canvas
- Use a white background with restrained professional colors
- Use navy or charcoal for primary text
- Use teal or blue for structure and one limited warm accent for decisions or risks
- Keep strong grid alignment and generous whitespace
- Maintain high-contrast Korean typography
- Use consistent headers, footers, page numbers, source notes, logo positions, corner radii, strokes, and icon families
- Avoid arbitrary gradients, excessive shadows, floating decoration, fake dashboards, and repetitive card walls

The user's supplied template, reference style, or approved sample overrides these defaults.

## Source and evidence handling

- Put a compact source note at the bottom of each evidence-bearing page
- Preserve exact source wording when legal, financial, scientific, or official accuracy depends on it
- Distinguish company-wide data from site-specific data
- Distinguish actual results from targets, scenarios, and estimates
- Leave a visible placeholder when required evidence is missing
- Keep missing-source requests outside generated slide images unless the user asks otherwise

Use this format in planning:

`! 필요 소스: [자료명] | 용도: [배치 위치·전달 목적] | 조건: [원본 유지·비율·해상도]`

## Five-pass final improvement

After the final requested artifact is produced, complete five corrective passes:

1. Narrative sequence, page roles, transitions, and duplication
2. Copy clarity, factual consistency, names, numbers, units, and sources
3. Speaking-time fit and page-level information density
4. Visual continuity, hierarchy, fidelity, and editability
5. Final image and PPTX render inspection across every page

Treat every pass as review → correction → recheck. Do not merely list defects.

## Delivery rules

Deliver only artifacts that passed the applicable quality gates.

- Slide images: provide the final ordered images or requested combined PDF
- Editable deck: provide the final PPTX and briefly state the editable and rasterized element types
- Combined request: provide the PPTX and PDF when requested
- Keep the handoff concise
- Do not claim complete editability when complex visuals remain raster objects
- Do not claim fidelity that was not visually verified

## Interaction shortcuts

Interpret these phrases as triggers for the complete established workflow:

- `이전 방식 그대로`
- `전략형 PPT 방식으로 진행`
- `제안서 전체 제작`
- `IR 자료 이미지부터 PPTX까지 제작`
- `이미지 생성 후 편집 가능한 PPT로 전환`
- `방금 작업 방식으로 진행`

If the user says `기획 고도화`, provide planning only unless production is also requested. If the user says `진행`, continue from the latest approved stage without restarting.
