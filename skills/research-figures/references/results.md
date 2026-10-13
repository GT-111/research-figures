# Quantitative and hybrid scientific figures

## Select by scientific question

| Question | Figure family | Dense ink adaptation |
|---|---|---|
| Method/task/metric comparison | Grouped bars, point contrasts, wide multi-metric panels | Resolved focal/comparator colors, ink edges, hatch/marker separation, compact common legend |
| Mechanism removal or addition | Ablation bars, paired differences | Align the variant naming with the exact changed component; short labels, zero baseline for bars |
| Learning/post-training trends | Curves, multiple panels, actual-step/time traces | Heavy precise strokes, handwritten axes, distinct markers; surrounding sketch frame only |
| Data/model/compute/rollout scaling | Linear/log curves, two-factor grids | Real coordinates and units; documented held-out cohort; separate independent variables |
| Relationships or transfer | Correlation, score, confusion, relation heatmap | Resolved two-sided signed scale or ordered magnitude map; precise grid and numeric annotations |
| Performance trade-offs | Scatter, Pareto scatter | Actual latency/quality coordinates; correct better-direction; highlight measured frontier only |
| Latent representations/manifolds | 2D/3D scatter, colored embeddings | Keep projections exact; record embedding algorithm/parameters and point labels; no causal interpretation |
| Motion/dynamics evolution | XY/XYZ trajectories, time-aligned curves | Equal spatial axes where appropriate; units and frame conventions; distinct reference/achieved lines |
| Multiple heterogeneous objectives | Radar/polar comparison | Document normalization and better-direction; consistent axis order; optional low-opacity fill |
| Data/method composition | Stacked counts/proportions, donut when justified | Thick black separators; explicit denominator and total; no false 3D volume |
| Distribution/reliability | Histogram, box/violin, empirical distribution | Raw samples, stated summary semantics; real outliers; no invented repeats |
| Conceptual geometry | Shaded sphere, vector field, manifold schematic | Distinguish explanatory geometry from observed data; no hand-drawn substitutes for physical hardware |
| Task performance with context | Task photos + bars/curves/table | Aligned task columns; matching cohorts; common legend; metrics and actual visuals in separate editable regions |

This is a capability specification for runtime authoring, not a shipped plotting library. Read the matching sections of [figure-families.md](figure-families.md) for concrete composition and ink treatment before generating the master. Tables, qualitative grids and hybrid figures use the same guide. Implement only the requested families in project-local code.

## Scientific data contract

Read the actual data and definitions: units, better-direction, run identity, seeds, evaluation cohorts, denominators and missing observations. Compare matched settings. Aggregate only real independent repetitions. A single run permits a curve, not a statistical band. Label illustrative data visibly. If sourced results and synthetic capability demonstrations share a board, separate their regions and use neutral synthetic method names; a real method identity must not silently carry into invented measurements. A raw count, success fraction, task progress and normalized throughput are different metrics.

Scaling requires actual positive numeric x for logarithmic axes; tick order or category index is not training exposure. Specify whether exposure means unique demonstrations, valid frames, hours, rollout steps or gradient updates. Record controls: model size, optimizer budget, task split and evaluation denominator. A fitted scaling law needs its formula, fit method, domain and uncertainty; do not silently smooth a few points into a claim.

Bars start at zero. Narrow curve ranges are allowed only when stated and no observations/bands are cut off. Use shared ranges for comparable panels. Missing values remain missing. No decorative jitter, hand-sketch transform or `xkcd()` on data paths, error artists, histogram bin positions, axes or heatmap cells. Color plus marker/hatch/line style must distinguish methods.

## Runtime plotting implementation

The skill does not ship a numerical helper API. During invocation, write minimal project-local Matplotlib code for the actual data, panels and master layout. Apply the palette and font specifications from palette-and-type.md and decorative contours from shape-vocabulary.md. Keep actual input paths, metric definitions, aggregation and redraw commands with the output. Do not import an assumed shared library or require a fixed JSON schema.

Construct grouped bars from a method × category matrix, curves from real numeric x and series vectors, and heatmaps from a row × column matrix with labels. Validate the dimensional relationships before plotting. For real independent runs, compute and label the requested statistic; use sample SD, standard error, bootstrap or confidence intervals only according to actual run structure and the requested interpretation. Never infer uncertainty from decorative shadows.

Use GridSpec/subfigures for unequal panels, shared axes for matched comparisons, and a dedicated legend axis or figure legend for crowded small multiples. Keep panel ordering and legend semantics stable. Use native polar axes only with documented normalization and direction; retain raw metrics in the source. Use 3D axes for real XYZ trajectories/surfaces, and retain projection/settings for embeddings.

Numerical artists remain precise. Add selective irregular group frames as separate decorative paths outside the full extent of ticks and labels. Strong headings and series can carry the style without a frame. Do not apply global sketch transformations. Use mathtext for short formulas by default; external TeX is optional when the environment has it. Select font files that the actual plotting runtime sees, not only names reported by the operating system. A stale font cache can otherwise silently replace handwriting with sans.

Determine each quantitative panel's final physical bounds inside the plate before plotting. Typography uses those panel bounds, not the width of the whole figure or an arbitrary standalone chart. Prefer authoring with `figsize` equal to the final panel size in inches and the documented physical font sizes; for a larger authoring canvas, multiply fonts/strokes by the same scale. A 7-inch plot later inserted at 2 inches reduces 12pt to about 3.4pt; increasing DPI does not restore legibility. Fit readable labels with sparse ticks, short category names, dedicated legends and appropriate panel area. Preserve image aspect ratio when placing the exact plot.

Export SVG with real text, PDF with appropriate embedded fonts, and PNG at 300dpi (600dpi for exceptionally dense final-size figures when useful). Keep an accurate data/spec copy or source reference, minimal redraw code, resolved fonts and uncertainty definitions. If a PDF font inspection reports a mismatch between font type and embedded file, repair the export route rather than dismissing it because one preview looks correct. A compatible SVG-to-PDF vector renderer can preserve the exact plot and embed OpenType/CFF fonts correctly when a plotting backend does not. A direct Cairo plotting backend is another option when SVG conversion introduces hatch seams. Inspect hatches and transparent bands after any backend change, as well as the actual text/font embedding and vector content; do not fix typography by rasterizing the whole figure. Shared styles may be project-local functions for that figure set; do not turn this documentation skill into a mandatory rendering framework.

For sphere/manifold/vector-field concept illustrations, state their mathematical construction and distinguish explanatory geometry from observations. A rendered mathematical sphere can be generated from a normal field and light direction; it is not a substitute for actual robot geometry. Domain computations such as diffusion paths, embeddings, frontiers, tests and fitted scaling laws belong in recorded analysis code rather than being guessed from a requested chart type.

Use the visual master to arrange exact numerical panels, not to supply their values. Quantitative compositions and task-photo pairings follow generation-and-reconstruction.md and assets-and-composition.md.

## Validation that changes the result

Use known coordinates and independent runs to catch wrong spacing or aggregation. Compare chart artists with expected data for added families; check zero bar baselines and explicit radar normalization. Resolve dimensional mismatches before export and omit unsupported one-run uncertainty. Inspect actual-size SVG/PDF/PNG for labels, legend placement, frame overlap and contrast. When pairing photos with results, confirm the cohort/condition mapping and source provenance. See assets-and-composition.md for combined teaser/task boards.

## Mean curves with standard-deviation bands

Build a run × x matrix from genuine repeated-run records, matching the same condition and actual x values. At each x, compute the arithmetic mean and sample standard deviation (`ddof=1`); draw mean ± 1 SD when the request says std without another definition. Label the band explicitly, including run count. SD is run-to-run spread, not standard error or a confidence interval. Use opaque method-colored mean lines and low-opacity matching fills behind them, with shared color/marker identity in other panels. Do not let the generated master choose the band widths.

An individual run must contribute once at a given x. For unaligned or missing checkpoints, state the alignment and available run counts; do not invent observations or silently interpolate runs to create a band. If fewer than two independent runs support a point, omit its SD band. Interpolation/smoothing, when scientifically justified and requested, belongs to documented analysis. Keep the numerical mean and bounds available with redraw data. Verify a representative mean/SD against the raw rows and inspect whether both curves and bands remain legible when overlapping.

## Bar and line overlays

Honor an explicit request for an overlay. Establish what the bars and line each measure, their units, the shared x variable and the data association. When both encode the same unit, use one y scale. For different units, a labeled secondary y axis is appropriate: label both axes and put metric + unit in the legend or direct labels. Keep bars behind the line, with black edges and a less dominant fill; give the line an opaque contrasting semantic color and visible sample markers. Bind each series to its intended axis explicitly.

Bars start at zero; secondary ranges are set from the actual metric and explained rather than adjusted to manufacture matching peaks or crossings. Both layers use the same true x coordinates and category order. Combine legend entries from both axes. Numeric x values with unequal spacing remain unequal, including bar centers; choose widths that do not imply categorical equal spacing. Categorical overlays show separate category comparisons, not a continuous causal relationship. A dual-axis intersection is not an equality of values. Preserve method colors when already assigned; distinguish metric roles with fill, stroke and marker rather than silently recoloring a method.
