# Native shape and ink vocabulary

This is a prepared drawing language, not a fixed layout or export API. The invoking agent authors geometry for the actual master using the current project's tools. Basic shapes, labels and relations remain editable. Preserve scientifically meaningful dimensions and numerical precision.

## Ink character

On a 1600×900 design canvas, start with about 3.2–4.0px structural contours and 3.5–4.5px major computation arrows. Secondary motifs use about 2–2.8px; light tensor separators can be thinner. Black should retain a strong role. Tiny raster-like jaggedness is not the goal: use visibly hand-directed, smooth, slightly bowed lines.

For a 200–350px module, mild contour displacement around 2–4px and waves spaced roughly 50–90px give a usable native approximation. Use stable irregularity across rebuilds so a label/asset revision does not redesign every contour. Different edges need not have identical sine waves. Corners may be slightly uneven or rounded. Avoid scalloped “cute” frames, exaggerated zigzags, torn-paper edges or scribbles that distract from the method. Do not skew text together with a rough contour.

Preserve visible pen strokes, shadows, hatches and depth using the [native effect recipes](native-style-reconstruction.md). Only fine stochastic paper/ink grain is routinely omittable with disclosure. This exception does not permit deleting shadow silhouettes, hatch lines or secondary contours. Match the chosen master rather than imposing the same effects everywhere.

## Boundary variants

| Boundary | Appearance | Use |
|---|---|---|
| Solid ink | Black, moderately irregular, continuous | Ordinary module or key mechanism |
| Colored solid | Resolved accent outline, white/natural interior or deep header band | Stage grouping or a scientifically distinct path |
| Dashed ink | Clearly separated short dashes following the contour | Visual grouping; optional/training meaning only when defined in the brief |
| Dashed color | Resolved accent dashes around a light/deep module | Stage grouping or qualified branch with an explicit label |
| Fine regular | Straight light grid with strong outside frame | Tensor, mask or data-table cells; preserve exact geometry |
| Blank slot | Neutral gray thin dashed frame, white inside | Missing screenshot/data/official asset in a draft |

A starting dash rhythm is roughly 8px on / 5px off at design size; adjust to the rendered line width. Dashes should remain separated at final paper size. Dashed lines must retain their shape at corners; avoid a dash pattern that makes a small module look solid. Text does not inherit dashing or sketch displacement. A boundary's meaning is labeled; never rely on color alone.

## Base shapes

| Shape | Geometry/style | Scientific role when appropriate |
|---|---|---|
| Rectangle | Slightly bowed sides, sturdy ink outline | Module, value carrier, region |
| Rounded rectangle | Small rounded corners with irregular sides; avoid huge pill corners | Learned mapping, memory, nested module |
| Dashed rectangle | Same proportions as its solid counterpart | Optional/frozen/training boundary with explicit meaning |
| Trapezoid | Two parallel faces; contour irregularity small relative to taper | Projection/compression/expansion when that interpretation applies |
| Encoder wedge | Left face taller, right face shorter | Compressing map, not every generic encoder by default |
| Decoder wedge | Left face shorter, right face taller | Expanding map |
| Parallelogram | Mild skew, text remains upright | Input/output carrier if the master uses this notation |
| Cylinder | Native body plus top ellipse and lower arc; compact top label | Dataset/memory store when useful |
| Circle/ellipse | Strong single outline; plus or short variable can be centered | Sum, graph node, compact operator |
| Diamond | Minimal native polygon, enough room for the symbol | Selection or gate when the method has one |
| Bracket/brace | Open contour around a repeated group | Temporal window, action chunk, shared weights |
| Zoom wedge/inset | Small focus boundary with short link to detail | Mechanism expansion, not a new computation path |
| Token square | Compact regular rounded square, precise row spacing | Discrete code/token; counted groups should reflect actual dimensions or an ellipsis |
| Mask cell | White/filled regular cell with 0/1 or active/inactive marker | Actual support/attention/control mask |
| Frame card | True image rectangle; optional offset stack | Temporal observation/reference samples |
| Matrix/tensor | Native regular cells/lines, strong exterior; short dimensions outside | Actual tensor/attention/relation structure |
| Network motif | Few editable nodes/edges inside a mapping | Generic learned mapping unless exact topology is specified |

Normalized trapezoid starting proportions: a symmetric trapezoid can use top corners near 20%/80% of width and bottom corners at 0%/100%. An encoder wedge can use the full left height and a right face inset about 15–20% at top/bottom; reverse for a decoder. Adapt to the master. The taper and boundary are native geometry; labels are native text, not baked into a picture.

Do not draw a robot hand, humanoid or simulator identity out of these primitives. Use genuine model renders, photographs or official assets. Generic network nodes and data tokens are appropriate; physical identities are not generic mechanism glyphs.

## Connector grammar

For relation endpoints, routing, junctions and native attachment, read [connector-design.md](connector-design.md). The rules here define appearance; a well-styled line does not establish a connected or meaningful relation.

Main computation has a clear reading direction. Use smooth native connectors with their own heads; rough module contours do not require rough or assembled arrows. Feedback gets a reserved local return channel, or a separate channel when a wider loop is needed to explain it. Keep arrowheads moderate and distinguish junctions from line crossings. Route around labels, not through a panel heading. Avoid arrows that stop short of a module without a reason. Use source/target attachment where available; retain native editable waypoints.

- Ordinary causal/data flow: strong black or the carrier's semantic color, solid arrow.
- Focal contribution route: the resolved focal accent with matching emphasis.
- Training-only objective route: explicit short-dash route and objective label where appropriate.
- Feedback: separate solid/dashed lane according to the brief, labeled with the actual observed quantity.
- Stop gradient: explicit short label and two oblique strokes crossing the relevant route; distinguish from a mere divider.
- Frozen mapping: clear FROZEN/read-only annotation. A snowflake may support the label but is not enough by itself.
- Shared parameters: bracket or labeled association, not an unlabeled computation arrow.
- Optional bypass: visible branch/rejoin and optionality label. Do not invent a residual sum or gate because it looks good.

## Internal density

A module may combine its short name with one meaningful micro-illustration: tokenization, a state vector, a mask row, a compact network, a frame strip, a spatial relation or a tensor operation. These motifs replace prose. Leave a few pixels of breathing room between the label and motif; they are separate visual levels.

Align repeated tokens, frame timestamps and matrices. An ellipsis means omitted continuation, not a fabricated dimension. Annotate tensor dimensions outside the grid. Rotate/skew conceptual cuboids mildly if the master uses them, but keep exact data cells unwarped. A network motif does not justify adding unimplemented layers or attention.

Large regions should contain aligned scientific objects rather than empty colored space. White gutters around 12–20px are a useful starting point between dense panels; arrow channels may need more. Asymmetric mosaics, a broad execution lane above compact learning/detail panels, or aligned expert lanes can all work. Choose according to the contribution and generated master.

## Result-figure adaptation

Use the same opaque resolved series colors, thick precise strokes, black bar/marker edges and handwriting. Add rough surrounding frames or handwritten stage headings as separate decoration. Bar baselines, point coordinates, error intervals, histogram bins, axes and heatmap cells are regular and accurate. Do not use global sketch transforms on numerical artists.

Task-photo boards can use strong stage bands and repeated native label groups. Photographs and numerical panels remain undistorted independent objects. A blank slot is truly blank evidence, not a zero-height bar or an imaginary task photo. Report the needed asset or data outside the final paper crop.
