---
name: research-figures
description: Design and revise paper teasers, framework and module figures, quantitative plots, and task-visualization result boards. Read project contributions and user requirements, generate a visual composition master, then reconstruct editable PPTX/draw.io and reproducible vector plots in a dense ink sketch style. Can assemble all figures in one PPTX.
---

# Research figures

Create figures that communicate a project's contribution in a dense, expressive scientific sketch language. The project determines the scientific content; the established style determines its visual expression. Default to English figure labels and communication in the user's language.

## Workflow: project → visual master → editable reconstruction

1. **Understand the project and request.** Read supplied instructions, method/design documentation, relevant code/configuration, existing evidence and the user's constraints. Identify the core contribution, the comparison it changes, and the scientific message each figure must support. A repository's model variants, planned mechanisms and validated capabilities are different things.
2. **Write the project-local figure brief.** Record the figure's role, one main claim, contribution hierarchy, inputs/outputs, causal/training paths, source pointers, exact labels and evidence status. Inventory actual models/images/logos/data and missing material. Project facts and named reference provenance stay here, not in the installed skill.
3. **Plan the explanation and resolve the style.** Read [illustration-design.md](references/illustration-design.md) for contribution-led arrangement and original-paper learning. Read the relevant figure-family section, then [visual-style.md](references/visual-style.md), [palette-and-type.md](references/palette-and-type.md) and [shape-vocabulary.md](references/shape-vocabulary.md). Record one figure-set specification for fonts, colors, marks and stroke hierarchy. For connected mechanisms, read [connector-design.md](references/connector-design.md) before assigning coordinates. Reuse applicable studies and the accepted layout for later revisions; browse further only when the new explanation or requested style requires it. Sources inform arrangement, while the project remains the authority for content.
4. **Generate the visual master.** Generate the full figure's designed composition from the brief and style constraints, using genuine asset inserts where available. This is the default design route, including architecture, teaser, standalone quantitative plots and result-board composition. Retain an accepted earlier layout when the user requests a color/style change. Do not replace it with a canned diagram template. Read [generation-and-reconstruction.md](references/generation-and-reconstruction.md).
5. **Read and correct the master.** Inspect the generated image. Check scientific topology, labels, dimensions, frozen/gradient boundaries and evidence against the project brief. Generated numbers, physical identities and model mechanisms are not authority. Keep the expressive composition; correct factual errors before reconstruction.
6. **Reconstruct and deliver.** Map meaningful regions to native editable shapes, labels and connectors; use independent genuine image assets for physical entities, and exact data-driven rendering for numerical plots. Read [native-style-reconstruction.md](references/native-style-reconstruction.md) before native authoring. Reproduce the master's hierarchy, geometry, typography, density, color distribution and designed effects: shadows, rough contours, dashes and hatching where present. Leave deliberate blank regions for missing inputs, and tell the user exactly what is needed. Render the actual editable files and inspect their visual/scientific correspondence.

Choose supporting references by the requested deliverable; the route list below is an index, not an instruction to load every document. Resolve available image generation, font files, authoring tools and native renderers in the current environment before promising exports. Tool names, runtime paths and material caches from another project are not prerequisites. Keep progressing on available outputs and report any unavailable generation/rendering step accurately.

When editing an existing user-modified artifact, read it first and preserve the user's changes. Generate a revised visual proposal when redesign is requested, then apply it to the latest artifact. Do not overwrite manual edits from an obsolete scene file. PPTX and draw.io do not automatically synchronize later edits.

## Route detail

- Contribution-led explanation and relevant original-paper figure learning: [illustration-design.md](references/illustration-design.md).
- Architecture, teaser, module figures and all-in-one slide assembly: [architecture.md](references/architecture.md).
- Family-specific composition and heavy-ink treatment, including tables and qualitative grids: [figure-families.md](references/figure-families.md). Read the relevant family sections before master generation.
- All quantitative families, scaling and custom Python plots: [results.md](references/results.md).
- Optional examples of transferable explanations learned from robotics: [robotics-layouts.md](references/robotics-layouts.md). Select relevant examples after mapping the actual relations; method families do not prescribe a template.
- Genuine rendered assets, official identities and task-image/result pairings: [assets-and-composition.md](references/assets-and-composition.md).
- Prepared native ingredients, operation-first module illustrations and optional reusable material kits: [asset-vocabulary.md](references/asset-vocabulary.md).
- Relation endpoints, module/port alignment, loop ownership, routing and attachment behavior: [connector-design.md](references/connector-design.md). Read before assigning coordinates to connected mechanisms, then retain the resolved guides in generation and reconstruction.
- Color, typography, native shape vocabulary and matching the visual master: [visual-style.md](references/visual-style.md).

## Visual invariants

New figures default to the earth-ink profile: moss/olive, wheat/ochre and slate blue on warm white, with strong ink contours. The vivid red/blue profile remains available for an explicit request or an already accepted figure set. Handwritten short labels and thick irregular module contours create the sketch character. Density comes from visual mechanisms, real examples and compact hierarchy; long text inside boxes is not a substitute. Use the documented shape vocabulary as a drawing language, not a fixed layout.

All figure families share this language: grouped bars, trend/scaling curves, scatter, heatmaps, radar, composition, trajectories, distributions, geometric illustrations, task boards and mixed teaser/results. Conceptual module connections default to aligned horizontal/vertical shafts and deliberate orthogonal routes; resolve local guides before generation. Data positions, axes, error bands and matrix cells stay mathematically precise. Heavy hand-drawn treatment belongs to framing, surrounding annotations and conceptual shapes.

Missing assets/data: reserve the intended space, identify it in the editable draft or an external missing-input note, and report what must be supplied. Do not fabricate measurements, successful robot execution, branded identities or statistical uncertainty. Explicit illustrative data is appropriate only for a requested capability demo, visibly labeled and separate from project evidence.

## Outputs

Architecture defaults: native `.pptx`, `.drawio`, paper `.svg`/`.pdf`, and PNG previews. Plots: input data/reference, minimal redraw code/spec, SVG/PDF/PNG. Hybrid figures retain each photo/render/plot as an independent image alongside native editable layout and labels. Do not claim inserted plots are native PowerPoint charts.

“把所有图放进一个pptx” or equivalent: collect requested figures in their intended order, reuse editable architecture slides, include result panels with their vector/data sources, and assemble one deck. No extra confirmation is required.

Keep generated images, figures, results and renderer outputs in a project-local ignored or explicitly external directory. Keep the installed skill independent of any project paths, school names, paper identities, robot lists or model assumptions. Sources/licenses for actual copied assets belong to the project-local record and deliverable.

## Documentation-only implementation

The installed skill contains instructions and reference documents, not export scripts or a plotting library. When invoked, the agent generates a visual master and writes task-specific authoring/redraw code in the current project's figure output directory using available tools. The documents constrain color, typography, shapes, scientific correctness, master correspondence and editability; they do not force a fixed code API or diagram schema.

For local implementation choices and renderer pitfalls, read architecture.md and results.md. Missing generation or native rendering capability is a concrete limitation to report, not permission to claim an ungenerated master or verified export.

Validate metadata after skill edits. Behavioral acceptance uses unrelated methods, known numerical inputs, a combined deck and a native-object edit. Inspect actual renders for clipping, collisions, font/palette drift and master correspondence. Keep sample artifacts outside the installed skill and outside tracked project source.

## Improving the skill through trials

When asked to improve the reusable skill, treat a sample figure as evidence for a transferable authoring decision. Identify whether its failure comes from explanation hierarchy, visible relation selection, asset choice, style reconstruction or the export primitive. Change that rule in its owning reference, keeping project-specific facts and the trial's comparison outside the skill. A repaired sample alone does not establish a general improvement.

Use a small independent trial targeted at the changed decision. An exporter/arrow failure can be tested with a few native connectors before rebuilding a whole framework; an explanatory failure needs another method or original-paper structural comparison. Once the observed failure is understood, the guidance updated and the relevant trial inspected, end that iteration. Continue revising the sample only when the user requests its final figure or a remaining failure changes the reusable guidance.
