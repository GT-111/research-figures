# Art direction by figure family

Read the sections matching the requested figures. This document owns composition and visual treatment per family. The exact palette/type and base geometry live in [palette-and-type.md](palette-and-type.md) and [shape-vocabulary.md](shape-vocabulary.md); numerical semantics live in [results.md](results.md). Every family uses a generated composition master followed by reconstruction. A numerical master proposes arrangement, never measurements.

## Shared character across different families

Use a compact scientific plate: bold short panel headings, clear focal hierarchy in the resolved palette, forceful black contours, legible handwriting, and closely arranged meaningful objects. The blank canvas and arrow/label gutters provide contrast. Make the contribution visually heavier than its context. Density means an efficient relationship between objects; it does not mean filling every gap or enclosing everything in a box.

Carry the same method color, marker and naming across the figure set. A curve cannot adopt a different method color simply to balance a neighboring photograph. Keep evidence plots on white interiors; put stronger ink in series, outlines, headings and selected group bands. Architecture can sustain deep filled modules; quantitative figures need space to read values. This difference preserves a common style without making every family the same composition.

Use slightly bowed, uneven contours around semantic groups and conceptual objects. A heading may have a short heavy underline or colored band. Use a second offset stroke selectively on a focal boundary. Outer frames are optional: a strong heading and repeated black-edged marks can carry the style without frames. When framing plots, enclose the whole group including tick labels and axis titles; do not trace the axes rectangle with a wavy line. Shared gutters and aligned axes matter more than decorative enclosure.

## Teaser: capability plus evidence

Give one genuine scene, montage or morphology grouping the largest region. Link it to a compact representation of the contribution and a small evidence panel. The eye should find capability, mechanism and evidence in that order when that matches the argument. An asymmetric collage can use a broad scene strip above a compact mechanism and result pair; it need not resemble a framework figure.

Use strong resolved-accent labels or brackets to identify actual demonstrated capabilities. Keep scene silhouettes and contact regions visible. Use one short contribution phrase and a few concrete labels, rather than a paragraph of claims. A tiny quantitative panel still needs units, a readable baseline and cohort identity. A blank evidence slot is appropriate when measurements are pending; never promote an illustrative trend to the teaser's claimed gain.

When an overview and teaser accompany the same method, give them different jobs. The teaser connects recognizable input/task diversity to one visual contribution cue; the framework explains the necessary computation and learning relations. Remove decoder internals, ABI labels and repeated training plumbing from the teaser. If qualified results are absent, frame it as a method/concept teaser with attributed source scenes and an explicit evidence-status note, rather than inventing a performance panel or an achieved capability claim.

## Framework: overview with internal mechanisms

Allocate a broad region to the main causal path; fit preparation, training or optional adaptation into smaller adjacent regions according to dependencies. A top execution lane with compact lower mechanism panels or an asymmetric interface/training mosaic are starting points. Stage boundaries are heavier than interior separators. Deep headers and focal cores should anchor an otherwise readable white/middle-tone field.

Replace descriptive bullet lists with real carriers: frames entering an encoder, a vector entering a policy, a support mask controlling dimensions, a token strip entering shared attention. Include only motifs justified by the project. Use black arrows for ordinary computation and a consistent accent for the focal route. Training supervision and feedback get dedicated paths and explicit labels. If a detail cannot fit at final size, put it in a companion mechanism figure instead of shrinking it.

## Mechanism: expose the operation

Center the actual operation, with inputs on one side and resulting representation/objective on the other. Use token grids, matrix products, masks, before/after geometry or a small state transition when these explain the contribution. A magnified inset should refer to a specific part of the overview. Keep the same carrier geometry and color as the main figure.

For teacher/student or target/context designs, align the branches so shared and differing operations are visible. Freeze, stop gradient and parameter averaging are distinct annotations. Strong filled mappings contrast with regular white tensor cells. Put dimensions outside matrices; put short operation labels beside arrows. Keep multiplication, normalization and aggregation symbols separate editable objects. A decorative network is not an explanation of the mechanism.

## Grouped comparisons and ablations

Use compact matched small multiples with one shared legend, or one broad chart when categories are short. Resolved focal/comparator bars have ink edges; extra methods use a restrained neutral plus hatch/marker distinction. A short handwritten panel heading and a strong local underline can supply the sketch character without surrounding every axis. Leave space for category labels below the axis.

For ablations, pair a compact component-presence table with aligned results, or align incremental variants in a horizontal chart. Define a component's presence with a native check/cross or filled/empty cell; do not turn an ablation into a paragraph. Keep reference and ablated colors consistent and show exact deltas only when supported. Bar heights and zero baselines remain exact; a requested narrow hard shadow may follow the native-effect recipe, sharing the baseline and no higher than the data top. Avoid shadows resembling an extra series or altering perceived height.

## Learning curves and post-training

Give time or actual training exposure a continuous broad axis. Use opaque, decisive lines in the resolved series colors with sparse markers at measured samples; separate methods with line pattern as well as color. A narrow pale uncertainty band is subordinate to its precise curve. Put the shared legend in a free strip or direct-label unambiguous endpoints with sufficient clearance.

If phases or interventions matter, use a small stage band above the plot and thin aligned event guides. Stage boundaries come from logs. A surrounding handwritten arrow can highlight a real event but ends outside the trace and its uncertainty. Use matched panels for different metrics rather than mixing unrelated units on a decorative second axis. Smoothing, when used, must be stated and the raw behavior recoverable.

## Mean ± SD curves and bar–line composites

For repeated-run curves, make the opaque mean and its sample markers the visual foreground. Use a restrained matching SD envelope behind it; label “Mean ± 1 SD, n = … runs”. The band can be light while the mean remains deep and forceful. Use the figure-set handwriting and ink weights unchanged. Keep grids quieter than the band boundaries, and shared panel ranges when comparing the same metric. Numerical aggregation follows [results.md](results.md).

For a bar–line overlay, use a broad shared plotting region with black-edged bars behind an opaque contrasting line. Keep axis titles close to their corresponding side and include both metrics in a common legend. Prefer a compact handwritten heading and one slightly bowed underline over a large colored header that competes with the data. A second y axis has an explicit unit; its scale is an analytical choice, not a visual alignment trick. Exact values, error marks and zero bar baselines retain precise geometry. If several methods/metrics make the overlay unreadable, separate secondary comparisons into a companion panel while preserving the requested main overlay.

## Data, model, compute and task scaling

Make the scientific independent variable visually explicit: actual demonstrations, unique tasks, frames, parameters or compute. A narrow genuine data/task strip can sit above a wide scaling plot. If quantity and diversity vary independently, use two aligned plots or a two-factor heatmap rather than merging them into a generic 'Scale' axis.

Use accurate linear/log coordinates and substantial resolved-color curves. Keep annotation callouts short: evaluation split, actual knee, observed saturation or measured comparison. Distinguish interpolation from extrapolation with labeled line treatment. A power-law fit is a separate analyzed series with its domain, not a decorative curved arrow. A data pyramid is conceptual unless its dimensions are explicitly quantitative. Pair success scaling with error/compute only when the data supports the pairing.

## Heatmaps, correlation and transfer

A crisp rectangular matrix is the focal visual mass. Use short handwritten row/column group labels and a bold regular outer boundary; put rough brackets outside for task families or transfer groups. Select an ordered magnitude or centered signed scale from palette-and-type.md according to the quantity, with a labeled colorbar and meaningful center. The darkest cells may be visually strong without changing the numeric normalization.

Shared-scale matrices enable comparisons. Keep cell geometry exact, represent missing cells distinctly from zero and choose annotation text for contrast. Confusion probabilities, correlations and raw counts need different normalization labels. A dense matrix can omit per-cell text when a readable colorbar conveys it; do not shrink all numbers to fit. Use a native inset for a meaningful submatrix only when the selected region is identified.

## Scatter, trade-offs and Pareto fronts

Use sturdy black-edged markers, resolved focal/comparator accents and restrained neutral context. Direct-label a few important methods with short leaders; move dense naming to the caption or legend. Reserve a clear corner for better-direction annotation rather than adding an unmeasured ideal curve.

A measured Pareto frontier links only nondominated observations under the stated directions. If lines between points imply unmeasured interpolation, distinguish that from measured samples. Bubble area must encode a named positive quantity with a size legend. Sketch accents belong to callouts and grouping, never point displacement. Use an inset with stated bounds when crowded observations need more space.

## Distributions, reliability and uncertainty

Use deep outlined box/violin silhouettes, precise median/quartile marks and consistent method colors. A white interior or restrained tint can preserve density cues; large solid dark violins can hide them. ECDFs and histograms use the same strong lines/edges as other results. Give an ECDF a little horizontal room beyond its largest observation and show the terminal probability-one plateau; a dashed final jump clipped at the axis edge can otherwise look like missing probability mass. This extension is the same empirical function, not extra observations. Put units and the meaning of spread in a short caption/legend, not dense chart prose.

Show real samples when useful. Any beeswarm displacement is confined to a categorical, non-measured direction and explicitly described; never jitter the measured coordinate. State histogram bins and KDE bandwidth when they affect interpretation. Keep outliers and sample counts recoverable. A single aggregate observation supports a point, not an invented distribution. Reliability curves require the actual binning and observation counts.

## Radar, polar and composition

For radar, use a precise regular grid with minimal neutral spokes, bold resolved-color method lines and visible vertices. Put short labels beyond the perimeter; provide room at the left/right extremes. A low-opacity fill may aid grouping, but opaque overlapping polygons conceal comparisons. State normalization, axis direction and order; provide raw values alongside the analysis. Choose aligned bars instead when the radar obscures the claim.

For stacked bars, align totals and label important segments directly. Use a compact common legend and black separators. For a justified donut, keep true angular proportions and use the center for the total/denominator; handwritten callouts stay outside with clear leaders. Use hatches or related tones for additional categories. Decorative extrusion, tilted ellipses and rough slice geometry distort values and are excluded.

## Embeddings, manifolds and conceptual geometry

Separate observed projections from explanatory constructions in both labeling and source records. A measured embedding uses exact projected coordinates, clear category encoding and recorded projection settings. A conceptual manifold can have an expressive boundary, short vector arrows and native sample markers; label it schematic. Use a deep colored surface with careful contrast if surface shading conveys geometry.

For spheres, vector fields and 3D geometry, use a clean rendered/vector mathematical construction within a compact ink-framed explanatory composition. Keep depth cues, occlusion and projection consistent. Rough arrows may explain a conceptual path, but measured trajectories/vectors remain exact. A mathematical body is not a surrogate for an actual robot mesh. If a scatter is visually dense, use appropriate aggregation or opacity rather than inventing category separation.

## Trajectories, temporal strips and contact diagrams

Align reference/achieved traces with genuine timestamped frames or poses. Match reference and achieved color across paths and error panels. A broad spatial view can sit beside a narrow error plot, or a frame sequence can sit above a time-aligned trace. Use black-edged event symbols for actual contacts and a compact legend for frame/units.

Equal spatial aspect and stated coordinate frames preserve geometry. Time arrows, sample markers and event guides reflect actual order. For many trajectories, use a documented subset or density view and label the selection. For 3D plots, choose a camera that exposes the meaningful deviation and preserve the projection. A static pose strip conveys poses, not a verified rollout. Keep real robot images distinct from conceptual path diagrams.

## Task photographs, result boards and tables

For spatial perception and navigation panels, distinguish an observed map, a predicted field and a schematic layout. Preserve map aspect, frame, scale and the alignment of overlays; show unknown/occluded areas separately from zero-valued or free regions. Use a common scene and view for comparable conditions. Graph edges inside a representation retain their stated semantic or geometric meaning, while external computation arrows use the framework connector language. Hatching, rough borders and handwritten annotations belong around the evidence and must not alter occupied regions, contact boundaries or measured paths.

Build repeated task columns with a short task label, precise result panel and corresponding genuine scene. Share metric ranges and legends across matched tasks. A stronger visual example may span two columns when it carries the contribution; uniform cards are not required. Deep colored headers and heavy picture boundaries can bind the board while the photos retain original colors.

For visual-plus-table boards, align each scene/condition with its row and metric columns. Use white cells, strong column headings, sparse separators and selective resolved-accent emphasis. Keep numeric precision and units consistent; use an explicit missing-data mark. Bold the best value only under the stated metric direction and comparison scope. Highlight practical differences without implying statistical significance.

For before/after, success/failure or qualitative grids, keep camera, crop and timing comparable or disclose the difference. Meaningful callouts identify actual contact, error or behavior. Pair selected examples with population evidence when making a general claim. Missing images remain clean independent slots; report task, camera, condition and needed metric data outside the final figure crop.

## Combined figure sets

Let panels differ by scientific role while repeating type, ink, palette semantics and carrier notation. Use one deck-level figure order and short figure-specific titles. Preserve each accepted layout, including its intentional asymmetry; assembling a deck does not mean converting every figure to a common card grid. Keep chart source/code, native architecture objects and image provenance accessible. Inspect paper crops and slides separately: a dense two-column paper plate may need a full slide or additional detail slide rather than automatic stretching.
