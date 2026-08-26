---
name: build-strategic-ppt-decks
description: "Create Korean strategic proposals, IR decks, business plans, government-support presentations, consulting proposals, product introductions, and pitch materials through a fixed end-to-end workflow: source analysis, full-deck planning, pagination, page-level planning, user approval checkpoints, consistent 16:9 slide-image generation, editable PPTX reconstruction, and rendered quality assurance. Use when the user requests a complete presentation workflow, asks to proceed in the established strategic PPT style, wants generated slide images converted into a highly editable PPTX, or refers to the previous proposal, IR, image-first, review-gated, or editable-deck production method."
---

# Build Strategic PPT Decks

Create one coherent strategic deck from source analysis through slide images and an editable PPTX. Treat image generation as the approved visual design stage and reconstruct the final deck with native PowerPoint objects wherever practical.

## Required references

Read only the references needed for the current stage, but read each selected file completely before acting:

- Stages 1 to 3: [references/planning-workflow.md](references/planning-workflow.md)
- Stages 4 to 5: [references/visual-guidelines.md](references/visual-guidelines.md)
- Stage 6: [references/editable-pptx-rules.md](references/editable-pptx-rules.md)
- Final delivery: [references/quality-checklist.md](references/quality-checklist.md)

When available, also use the established `build-strategic-ppt-images` skill for image-production details and the `Presentations` skill for PPTX authoring and verification. Follow their file-format and tool rules without weakening this skill's workflow.

## Default operating mode

Use review-gated mode by default and complete the workflow in approved increments unless the user explicitly requests autonomous completion:

1. Analyze and enhance the full content
2. Establish pagination and narrative sequence
3. Specify every page in image-ready detail
4. Propose visual styles and generate approved pilot slides
5. Generate the full slide-image deck
6. Reconstruct and verify an editable PPTX

If the user says not to start production yet, complete only the requested planning stages. If the user requests images only, stop after stage 5. If the user requests an editable PPTX from completed images, begin at stage 6 after confirming all source images and brand assets are available.

## Review-gated mode

Pause at the following approval gates unless the user explicitly selects autonomous mode:

1. Strategic direction approval
   - Present the purpose, audience, decision objective, core problem, proposed value, persuasion logic, storyline, missing proof, and major assumptions
   - Ask whether to approve, partially revise, or restructure the strategy
2. Pagination approval
   - Present the complete page map with page role, main message, evidence, visualization, required source, and speaking time
   - Ask whether to approve, add or remove pages, or reorder the narrative
3. Visual-style approval
   - Propose three to four distinct but professionally viable style directions before full image generation
   - Show a cover and one representative content page together for each direction when image generation is available
   - Explain the palette, typography, grid, diagram language, logo treatment, and intended audience impression
   - Ask the user to select one direction or request a partial adjustment
4. Pilot-slide approval
   - Generate two to three representative slides using the selected style, including a cover, an infographic page, and a complex diagram or architecture page when applicable
   - Ask whether to expand the style, adjust it, or replace it
5. Full-image approval
   - Present the checked full slide-image deck and summarize corrected defects
   - Ask whether to approve all images, revise specified pages, or perform a deck-wide refinement
   - Start editable PPTX reconstruction only after this approval

At every gate:

- Ask one compact decision question at a time
- Offer two to three clear choices plus free-form revision when the interface supports it
- Treat `진행`, `승인`, or an equivalent response as approval of the current gate only
- Continue only to the next approval gate after current-gate approval
- Resolve minor details autonomously and ask only about choices that materially affect strategy, pagination, style, fidelity, or evidence
- Preserve approved decisions unless the user explicitly reopens them
- Summarize material changes before requesting approval again

## Autonomy rule

Switch from review-gated mode to autonomous mode only when the user explicitly approves the entire remaining workflow or says phrases such as `전체 진행`, `중간 확인 없이 진행`, `마지막까지 자율 진행`, or `전체 장표 일괄 제작`:

- Continue through the final requested stage without page-by-page confirmation
- Preserve the sequence internally even when intermediate plans are not shown
- Make sensible assumptions for non-critical gaps
- Use labeled placeholders for missing non-critical evidence
- Pause only when a missing choice or asset materially changes the entire deck or makes exact fidelity impossible
- Keep progress updates brief

Do not interpret a standalone `진행` response at an approval gate as authorization to skip all remaining gates.

## Stage 1: Full-content planning

Analyze all supplied documents, images, tables, logos, prior plans, and conversation constraints before designing pages.

- Define audience, decision objective, presentation time, desired action, and evaluation context
- Extract verified facts, numbers, names, dates, claims, sources, and required evidence
- Separate supplied facts, verified external facts, assumptions, and proposals
- Identify contradictions, duplication, weak claims, missing proof, and unnecessary detail
- Build the persuasion logic around context → problem → implication → solution → proof → execution → decision
- Preserve the user's original intent while improving clarity and order
- Do not invent official proof, contracts, certifications, customer results, or exact financial values

Produce a concise strategic brief before pagination and request strategic-direction approval in review-gated mode.

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

Present the completed page map and request pagination approval in review-gated mode.

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

After page-level planning, proceed to visual-style selection and pilot slides according to the review gates before creating the full image deck.

## Stage 4: Visual-style selection and pilot slides

Propose the deck-wide visual system before full slide-image generation.

- Create three to four distinct professional style directions
- Pair one cover and one representative content-page concept for each direction when possible
- Keep each direction feasible for consistent full-deck generation and editable PPTX reconstruction
- Explain the palette, typography, grid, header, footer, logo treatment, diagram language, and audience impression
- Generate two to three representative pilot slides after the user selects a direction
- Inspect the pilots for text legibility, information density, brand fidelity, visual continuity, and reconstruction feasibility
- Request visual-style and pilot-slide approval in review-gated mode

## Stage 5: Slide-image generation

Generate horizontal 16:9 slide images only after the page specifications are sufficiently concrete and the style and pilot gates are approved, or after the user has explicitly selected autonomous mode.

- Use image generation for the raster slide pages
- Carry forward one deck-wide visual system across every page
- Keep header, subtitle, footer, source note, page number, margins, typography scale, and logo placement consistent
- Use supplied logos, faces, products, screenshots, documents, seals, and evidence without unauthorized alteration
- Match visualization type to the information relationship
- Prefer diagrams, charts, process flows, matrices, timelines, architecture, and annotated product scenes over paragraph-heavy layouts
- Inspect every generated image for Korean text corruption, numbers, units, names, cropping, overlap, logo fidelity, alignment, and 16:9 ratio
- Correct defects before accepting a page as final

Do not present unchecked images as verified.

Request full-image approval after correction and before editable PPTX reconstruction in review-gated mode.

## Stage 6: Editable PPTX reconstruction

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
- `중간 검토 방식으로 진행`
- `전략·페이지·스타일 승인 후 진행`

If the user says `기획 고도화`, provide planning only unless production is also requested. If the user says `진행` in review-gated mode, approve the current gate and continue only to the next gate without restarting. If the user explicitly requests autonomous completion, continue through the final requested stage.
