# From contribution to visual master to editable figure

## Input hierarchy

The project's method, implementation and evidence establish facts. The user's goal establishes emphasis and constraints. The installed style establishes typography, color and visual grammar. Named prior papers are visual references only when needed or requested. Start with the contribution, not a literature template.

Write the brief before prompting: what changes relative to the baseline, what evidence supports it, which mechanism causes the change, and which paths are causal/training-only. Select the figure's main job: introduce a capability, explain a framework, expose a mechanism, compare outcomes, inspect scaling, or show qualitative evidence. A contribution should get the largest or most visually salient region; baseline plumbing should be visually subordinate.

## Master prompt construction

Pass these concrete ingredients to image generation:

- Canvas and figure role; one main scientific message; exact required labels.
- Module/relationship list including inputs, outputs, feedback, freeze and stop-gradient meaning.
- The selected composition: e.g. a broad top execution lane and two compact lower mechanism/training panels. Preserve an earlier accepted composition unless the user changes it.
- Palette: the exact resolved profile, including natural body fills, stronger route/series colors, dark accents, warm canvas and ink contrast. Do not replace the selected profile with the generator's favorite bright primaries or cute pastel scheme.
- Font category, hierarchy, two-line label limit, variable/math handling and final-width legibility.
- Shape grammar: slightly bowed sketch outlines, sturdy black edges, short dashes for boundaries, trapezoidal mappings, token strips, stacked temporal carriers, genuine physical assets.
- Selected expressive effects: specify where offset ink shadows, secondary pen strokes, diagonal hatch accents, dark footer strips and dashed grouping boundaries belong. Match the requested intensity; do not turn all objects into uniformly clean flat cards. Preserve an accepted treatment instead of inventing extra effects everywhere.
- Local density: small scientific mechanisms within the module rather than prose; reserve channels for arrows and feedback.
- Actual supplied asset roles and exact places for missing assets/data. Missing physical inputs are empty reserved panels, not generated stand-ins.
- Quantitative panels: source data and exact plot references when available. Generated plot geometry is composition only; final data is reconstructed numerically. No invented results.

Use supplied reference images to condition visual appearance when appropriate; label their role in the prompt. Do not copy their science into a new method. Save the exact prompt, chosen master and factual correction notes in the output directory.

Inspect generated quantitative regions for added error caps/bands, invented sample counts, unlabeled series, fabricated log spacing and altered values—even in an explicitly illustrative master. Remove unsupported statistics during reconstruction. Restore the exact data and a method legend/direct labels. A generic loss or target branch added by the generator also needs confirmation from the method brief; visual plausibility is not authority. Record scientific repairs as removed/redirected edges as well as revised labels. An output must emerge from the operation that produces it: when correcting a solver/scheduler/update path, remove any old shortcut from the predictor to the final output. A correct caption does not repair an incorrect native arrow.

A targeted generated edit can preserve the appearance while correcting a local dependency. If it repeats incorrect routes, write the corrected producer/consumer map before authoring and apply that topology in native reconstruction. Retain the useful composition and expressive layers; another full image generation is unnecessary merely to force exact wiring. The master establishes visual decisions, while the project brief and corrected relation map establish scientific dependencies. Inspect the native result to ensure the old erroneous edges were actually removed, rather than leaving both versions of the route.

## Reconstruction map

Read the master as semantic objects. Write a project-local map of panel bounds, module bounds, labels, arrows, motifs, image slots and quantitative regions. Include each focal module's shape family, contour, fill, shadow, hatch, dash rhythm and type weight in the map. Read [native-style-reconstruction.md](native-style-reconstruction.md) and prototype a representative styled module in the actual renderer before repeating it. Work from this map rather than repositioning objects into the exporter's old template. Preserve wedges, rounded interiors, brackets and token arrangements that carry the master's visual grammar; if their implied scientific meaning is wrong, record that correction rather than silently normalizing every module to a rectangle. Relative master coordinates can be normalized into a 1600×900 slide; compact paper bounds should preserve the same composition.

Native object ownership:

| Master region | Reconstruction |
|---|---|
| Module/container/shape | Native rect/freeform/polygon; editable label or grouped label |
| Token/frame/mask carrier | Repeated native cells, meaningful group, short editable labels |
| Arrow/feedback/gradient boundary | Native connectors with explicit terminals/route; editable annotation |
| Tensor/network/relation motif | Native grid/nodes/edges or a documented vector source; no model-layer claim from generic decoration |
| Robot/task image/logo | Independent genuine picture object and source record |
| Quantitative panel | Exact Matplotlib/vector plot plus data/code; independently movable in deck |
| Missing material | Blank native slot with identifier; describe needed input outside final paper crop |

The final output should resemble the master in hierarchy, local spacing, contour weight, color areas and internal visual rhythm. Matching only colors/fonts while reverting to generic rectangles is insufficient. Do not use the full master as a background and overlay a few text boxes, or describe traced raster artwork as semantic editability.

If a specific effect cannot be represented natively, keep the semantic structure editable, approximate only that effect deliberately, and report the difference. Use a hybrid image region only for the actual visually complex region, not a whole panel containing scientific labels and connections.

## Missing-input handoff

Keep one missing-input record in the project brief: slot identifier, intended role, exact required item, and practical form. Examples: task name + evaluation condition + one screenshot; robot model or chosen view; official logo URL/asset; CSV with training exposure, seed, success numerator/denominator and cohort. Avoid asking for material already accessible in the project. Keep working on independent regions.

A blank results region means data is absent, not zero performance. A diagram can show a designed interface if its evidence status is stated; it cannot show a validated outcome without data. Leave clean whitespace or an unobtrusive native draft label; remove draft placeholders when inputs arrive.

## Visual verification

Open the native PPTX and draw.io renders; compare them with the master side by side. Correct observed clipping, arrow-label collisions, wrong asset aspect, font substitution and unexpected spacing. Check labels and relationships against the brief, and data against the input. Moving a module/editing a label should preserve meaningful editable content. Preserve this verification as real previews and a short limitations note, not a numerical aesthetic gate.

## Carry the style through the prompt

Compose the prompt from the actual brief and the relevant [figure family](figure-families.md), then resolve the exact color and font choices from their owning document. Write concrete visual instructions rather than only 'beautiful scientific figure' or a paper's name. A useful prompt structure is:

> Purpose: [one scientific message and intended final size]. Content authority: [project facts, exact labels and evidence status]. Reading order: [main path or comparison, then supporting detail]. Composition: [region hierarchy and placement, preserve accepted layout if present]. Visual treatment: dense expressive scientific ink drawing; compact bold headings, rounded handwritten short technical labels, resolved focal/body contrast, substantial ink outlines and controlled bowed contours; white gutters; meaningful internal mechanisms. Palette and typography: [resolved exact values/families]. Quantitative regions: [data/plot references, axis meaning, what must remain precise]. Actual image inserts: [asset and role]. Missing regions: [blank slot and required input]. Reconstruction targets: [native modules/carriers/labels/connections, independent pictures and exact plots].

For result-only figures, concentrate ink in strong precise marks, handwritten headings, black edges and selective surrounding annotations. Do not ask the generator to make numerical axes or observations wobbly. For frameworks, carry the local row/column guides and port choices from connector-design.md into the prompt: horizontal/vertical conceptual shafts, purposeful orthogonal returns, no diagonal shortcuts or tiny alignment jogs. Specify which modules contain actual masks, frames, vectors or operations; a request for density alone often produces filler. For mixed figures, describe the alignment between each task view and its measured outcome. Spell out a short exact label list; put explanatory prose in the caption/brief. Separate verbatim figure text from layout instructions in the prompt. Region proportions, editing instructions and reconstruction notes are not display labels. Specify whether a full-width title is wanted; a paper plate usually needs compact panel headings instead. Scientific variable types remain literal: a scalar prediction is represented by variables/samples, not a semantically different pictogram. Match masks to the actual entity they index, such as modalities, tokens or dimensions.

Generate one coherent composition per intended figure. A style-contact sheet is only a style test, not a reason to shrink a full method into one miniature panel. If generation is unavailable, report that limitation and preserve the brief; do not silently call a direct code layout a generated master.

## Reconstruction without aesthetic drift

Before authoring, identify the visible decisions that make this master work: focal region, unequal panel sizes, dark color masses, contour character, label hierarchy, recurring internal carriers and open arrow channels. Record these briefly with the reconstruction map. Retain them as the content is corrected. A deeply colored block may contain white internal motifs and a short title; flattening it into an empty rectangle loses both mechanism and style.

Fit native text using the resolved font and actual wrapping. Scientific equation lines have the same spatial obligation as labels: display a compact exact operation, split it at a meaningful step, or place the complete derivation in the caption when the panel cannot support it. Dense mechanisms gain detail from carriers and operations, not from full-width formulas running across neighboring blocks. Adjust the local geometry or shorten redundant labels rather than shrinking every label. Place image crops without stretching. Group a module's contour, label and motif while keeping them independently editable. Preserve exact plots as independent assets; a separate rough outline around their group is optional. On charts, the decorative boundary must clear the rendered labels and legend as well as the plotting area.

Compare actual render and master at the intended publication size. Correct the discrepancy you can see: weak core fill, lost asymmetry, missing internal mechanism, handwriting substitution, crowded labels or a rough frame touching ticks. Check science against the brief separately from appearance against the master. Completion requires reporting any remaining mismatch; a correct file format alone does not demonstrate style fidelity.
