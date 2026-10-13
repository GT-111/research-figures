# Preserve designed effects in editable reconstruction

Read before reconstructing a visual master into PPTX or draw.io. Editable figures retain their visual treatment, not merely labels and colors. Clean generic redraws do not reproduce sketch designs.

## Read and prototype the treatment

Alongside the semantic map, record each important region's contour width/irregularity, second pen strokes, fill/gradient, hatch placement, shadow displacement, dash rhythm, depth layers, type weight and motifs. Describe what is actually present; do not add every effect everywhere. A requested stronger sketch treatment is a deliberate style revision, distinct from faithful reproduction. Preserve the accepted layout.

Render one representative focal module with its actual title, longest nearby caption, connector label, token/frame carrier and effects before propagating that native style. Include child primitives whose theme defaults may differ from the body; a clean main block does not establish that small cells or text boxes are free of unintended effects. Compare at the intended figure size. Repair visible losses of ink, depth or weight here so they are not repeated throughout the deck. This small prototype does not require an extra user approval.

## Native layer recipes

Group editable layers: shadow/back layers → body → pattern → header/footer → contour/second stroke → motif/text. Give layers useful names. Attach connectors to the semantic body where supported.

**Shadow:** duplicate the silhouette behind the body, translate down/right and fill with ink or a dark related color. Start with 4–7px displacement on a 1600px canvas and match the master. Leave arrow/label channels clear. This is an editable freeform. Soft shadows may use explicit native effects if the renderer preserves them. Remove accidental inherited theme shadows only; never clear the designed shadow as blanket cleanup.

**Sketch and second stroke:** use smooth bowed native paths with stable edge-specific irregularity and substantial apparent ink weight. A partial secondary path 1–3px away can follow selected edges like a second pen pass. Avoid procedural repeating waves and polygonal stair steps. Text/data stay upright and exact. Native sketch presets are optional implementations, not evidence of visual fidelity.

**Dashes:** follow the bowed contour with visibly separated dashes; start around 8px on/5px off and match the source. Grouping boundaries may be aesthetically dashed. Computational paths have optional/training semantics only when defined by the brief. For a decorative boundary whose freeform API lacks dash control, editable contour dash segments can preserve its appearance. For a relation, use the single connector's native dash style and head; do not apply the segmented-boundary recipe to arrows. See [connector-design.md](connector-design.md).

**Diagonal hatch:** clip parallel native line segments to the body or a narrow side/footer band using line–polygon intersections. Start near 35–55 degrees, 7–12px spacing and 1–1.6px stroke at 1600px width; match the master. Keep solid backing under text and clear matrix values. Group the hatch lines with the body. Disabling automatic fill selection must not delete intended patterns: draw.io solid fill plus a separate native hatch layer is valid. If direction distinguishes categories, include it in the legend.

**Depth and tone:** preserve dark footer strips, stacked sheets, internal separators and side faces as independently editable shapes. Explicit native gradients are appropriate when present in the master and supported by actual rendering. Do not flatten every gradient into one light swatch. Inspect any tonal-layer approximation for distracting banding. Stacks do not imply extra model layers unless the brief says so.

**Type:** match apparent size, weight, spacing and title/body contrast, not only family. Bold generated labels reconstructed in thin regular text change the style. Use installed bold faces and the figure-set font contract, preserving literal math semantics.

Match line height and internal text padding as well as the text-box center. Native HTML labels and slide paragraphs can place identical multiline text differently despite the same font and bounds. Inspect the first and last visible lines against sloped or bowed module contours, and resolve the renderer's paragraph/HTML spacing explicitly when it causes drift.

## Exact numerical geometry

Keep data coordinates, SD envelopes, errors, axes and cells exact. Sketch effects belong in headings, framing, annotations, panel bands and intentional fill patterns. A requested narrow hard bar shadow is allowed: its top must not exceed the data top, it shares the zero baseline, and foreground edges/error caps remain unambiguous. Avoid apparent extra series or height and 3D perspective. Shadows never mean uncertainty. Precise hatches can distinguish series with a matching legend.

## Render and edit evidence

Compare master and actual native render at equal size and at publication size. Inspect the specific effects present: lost shadow, dash gaps, second strokes, hatch or dark strips require repairing those layers. Color/font agreement alone is insufficient. Compare focal type weight and mechanism density too; check science separately.

Move one styled module and change its label, then render. Its shadow, pattern and contour must remain with it; disclose manual connector rerouting. Inspect PPTX and draw.io independently when delivering both.

Only fine stochastic paper/ink grain is routinely omittable with disclosure. This exception does not cover visible shadows, hatching, dashes, rough contour geometry, header/footer depth or second strokes. If an effect cannot be represented, identify the exact region and approximation. Do not claim faithful reconstruction while defining effects are absent.
