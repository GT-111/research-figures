# Color and typography contract

These constraints are independent of project, institution and author identity. They express the selected visual language. Apply them to the generated master and to the editable reconstruction. Preserve an accepted layout when revising only color or type.

## Palette profiles

Use **earth-ink** for new figure sets: moss/olive, wheat/ochre and slate blue on a warm white field. Keep a previously accepted figure's resolved colors when only content changes. An explicit user request for vivid red/blue selects the alternative **red-blue-ink** profile. Resolve one profile for a set and propagate its semantic roles through diagrams, plots, tables and legends.

### Earth-ink — default

| Role | Hex | Preferred use |
|---|---|---|
| Ink | `#26261F` | Text, heavy contours, structural arrows, numerical baseline |
| Warm canvas | `#FCFAF4` | Default natural paper-like canvas |
| White | `#FFFFFF` | Tensor cells, photo backgrounds, plot interiors when useful |
| Focal olive | `#5F7348` | Main method curve/mark, focal route, compact emphasis |
| Sage body | `#B8C8A1` | Focal module body, repeated main-method carrier |
| Deep olive | `#3F5132` | Sparse dark header/footer, focal depth |
| Wheat body | `#E8D39B` | Preparation, data/interface or secondary stage when appropriate |
| Ochre accent | `#B8954C` | Third method, wheat route/header accent |
| Deep ochre | `#7A612E` | Wheat depth or compact dark detail |
| Slate blue | `#58788A` | Main comparator curve, supporting route |
| Slate body | `#BACDD4` | Context/reference or supporting module body |
| Deep slate | `#3B5563` | Sparse blue header/footer or depth |
| Clay | `#AD7459` | Fourth method or a small intervention/correction emphasis |
| Quiet sage region | `#EEF1E5` | Large supporting region with strong ink boundary |
| Quiet wheat region | `#F6EBCD` | Large preparation/interface region |
| Neutral note | `#696A60` | Secondary annotation, unavailable asset slots |
| Quiet grid | `#E3E1D8` | Supporting numeric grid or nonfocal divider |

Architecture bodies and plot marks use related roles, not the same light swatch: a sage body may contain black labels while the corresponding plot curve uses focal olive. The comparator similarly pairs slate body with a stronger slate curve. Default method comparisons: focal=olive, comparator=slate, then ochre and clay, with distinct marker/line/hatch identities. Do not make all routes or all modules green. Assign wheat to a meaningful supporting category rather than treating it as decorative confetti.

### Red-blue-ink — explicit alternative

Retain `#BA0C2F` focal red, `#0836BE` comparator blue, `#750C24`/`#08216D` depth, `#BE455E`/`#4969CD` supporting fills, `#171717` ink, white or `#FAF8F4` canvas, `#424A57` third series and `#C45212` fourth series. Optional `#F36C00` is a sparse accent. This profile preserves earlier accepted vivid figures; it is not automatically substituted into an earth-ink set.

These are designed figure palettes, not formal institutional or venue colors. Keep the exact resolved values across a set instead of choosing nearby colors independently in each exporter. Existing accepted method colors take precedence. Combine color with circle/square/triangle/diamond markers and solid/dashed/dash-dot/dotted lines. More than four methods may warrant grouping or another panel rather than near-identical shades.

## Lock the style before generation

Record one compact style specification in the figure brief: exact method-to-color/marker/line mapping; resolved font families/files/weights; final-size type hierarchy; structural ink weight; rough-contour treatment; uncertainty opacity; heading treatment; and canvas background. Pass these same choices to every generation prompt and project-local exporter. A master may vary composition, not silently replace the typography, resolved profile or contour language. If a user accepts one figure, use its resolved style for the rest of the set.

## Color distribution and contrast

In earth-ink, quiet warm regions and mid-tone natural bodies carry the scene; heavy black contours, short bold labels and meaningful internal mechanisms carry density. Reserve the strongest olive/slate/ochre for focal routes, compact header/footer bands and measured marks. A large dark colored slab can overpower the explanation. Natural colors do not require weak strokes, excessive empty space, rounded pill cards or uniformly pale cells. Preserve the accepted asymmetric layout and rough ink treatment.

Use ink labels on sage, wheat, slate-body, white and quiet-region fills. White/cream labels belong on deep olive/slate/ochre or a visibly dark selected body. Hatches and internal motifs need their own contrast decision: dark hatch strokes on light bodies, light motifs only against dark backing. Preserve black matrix edges and meaningful separators. Do not carry white text unchanged from a vivid dark profile into a light natural body.

In red-blue-ink, deeply filled focal modules and stronger middle-tone supporting bodies remain valid. Color distribution follows the selected profile, not an unconditional requirement to saturate every framework. A native recolor must update text, motif, hatch and depth contrast along with the fill, while preserving topology and geometry.

Color semantics are decided in the brief. The palette expresses hierarchy, not trainable/frozen status. Freeze, optionality, gradients and evidence status need explicit labels/line semantics. Keep the same object/method mapping across diagrams and results. Physical photos, model materials, official identities and measured values retain their actual meaning.

For heatmaps, use a perceptually ordered magnitude scale or an appropriate two-sided signed scale with a meaningful center. Earth-ink magnitude maps may progress from warm-white to slate; signed maps may use clay–warm-white–slate. Test the actual ordering/contrast and label the colorbar; natural hue matching does not justify misleading thresholds. Use about 0.16–0.22 alpha for uncertainty fill under an opaque matching curve. Bands may be light while means remain strong. Avoid translucent categorical bars when they weaken comparison; edges/baselines stay ink.

## Typography: one default, fixed across a figure set

Use **Comic Neue** throughout ordinary figure text: Bold for panel headings, module labels and axis titles; Regular for ticks, legends and secondary labels. This is the default handwritten identity for architecture and quantitative figures alike. Use a mathematical font only for actual math (DejaVu Serif with matching `dejavuserif` mathtext is the default). A monospace face is reserved for literal code. A serif-heading variant is available only when explicitly requested or already established by an accepted user figure; do not alternate serif and handwritten headings because different agents or exporters prefer different defaults.

Resolve the actual Regular and Bold font files before authoring. Match the same family and weights in image-generation instructions, plot runtime, native slides and draw.io. Resolve the math family in both the plotting runtime and the native renderer too: a font bundled privately with Matplotlib is not necessarily installed for PowerPoint/draw.io. Use the same available math family throughout the set; do not let each renderer silently choose one. Record family, file locations, weights and final-size roles in the project brief. Resolve fonts once for the figure set; reuse those decisions for later figures and revisions. A generated image suggests letterform character but cannot establish an exact font identity.

At a 180 mm wide paper plate, use this common starting specification: panel headings 12pt Bold; module/axis labels 9pt Bold; ticks/legends 8pt Regular; supporting notes 8pt Regular. Override a size only for a demonstrated layout or reading need and record it, rather than independently choosing a new hierarchy for each figure. These are final physical sizes: if authoring at a larger logical size, scale the font sizes accordingly so shrinking the export does not shrink 9pt to 5pt. For slides, scale the same hierarchy to the actual displayed figure bounds. Fit layout to the text; preserve the hierarchy across figure families.

If Comic Neue is unavailable, obtain it from a legitimate redistributable source when practical, or choose one available handwritten replacement for the whole set and disclose that choice. Do not silently mix fallback sans fonts into individual plots. Where a symbol is unsupported, use an explicit math/text fallback for that symbol and preserve the surrounding handwriting. Inspect actual labels such as units, minus signs, subscripts and mean ± SD in the renderer being used; OS font listings alone do not establish glyph coverage or actual rendering.

Before building a new figure set, render one small project-local specimen with the resolved heading, module label, axis title, ticks and legend. Take its required symbols from the actual label/equation inventory, including ellipses, operators and subscripts, rather than testing only a generic alphabet. Check the actual plot and native-slide render for substitutions, weight drift and wrapping. Inspect the final PDF font list as well as visible text when font consistency is being validated; unexpected fallback faces need an explanation or correction. For unsupported Unicode subscript characters, use supported ordinary characters with native baseline/size formatting or the resolved math renderer. Inline direction arrows and operators in handwritten headings need explicit covered font runs or native glyph geometry too. Apply that choice to the SVG/PDF/PNG path as well as native slides; a glyph that renders through an OS fallback in PPTX may still be missing in a paper export. An ellipsis can be three native dot objects. Reuse the resolved settings rather than making each figure rediscover them. This specimen and any authoring helpers live with the project's outputs, not in the installed skill. Do not bundle font files without redistribution rights. PDF should embed the resolved fonts; an editable text SVG/PPTX may still require those fonts on the recipient's machine, which belongs in the handoff.

## Paper figure versus presentation title

A paper plate normally starts with compact panel/stage headings; its caption supplies the full method title and explanatory claim. Add a full-width figure title only when it helps the requested composition. In a presentation, a separate native slide title may sit outside the figure crop. Keep the method name from consuming the mechanism or evidence region. Short synthetic/draft status labels remain visible when required, with detailed provenance in the caption/notes.

## Size and spacing

Use the final physical-size typography specification above as the source of truth. Convert it to the chosen authoring canvas instead of choosing an unrelated pixel range: `logical font px = final font pt × canvas width px / (final width mm × 72 / 25.4)`. For example, a full 1600px crop printed at 180mm needs about 38px for 12pt, 31.5px for 10pt and 25px for 8pt. Recompute for the actual exported crop, not a slide that includes margins outside the paper figure.

For a presentation, choose sizes for its viewing distance separately, retaining the same family, weights and relative hierarchy. Label line spacing around 1.0–1.15 and internal horizontal padding around half a label's font size are useful starting points. Inspect the actual exported crop at final width. If labels are too small, remove low-value detail or split a mechanism into another figure; shrinking everything is not density.

Use sentence/title capitalization consistently. Keep technical acronyms intact. Keep the variable count low and symbols consistent with the paper. Avoid extra words such as “Module”/“Process” when the functional term already identifies the object. No text paragraphs inside learned blocks. A caption explains the argument; the figure displays the mechanism and evidence.

## Quantitative visual weight at publication size

Scale chart styling for the final physical crop, rather than copying slide-pixel widths. At a full-width paper panel, 2.2pt focal curves, 1pt bar/marker edges, 0.9pt axes and 0.4pt supporting grids are the common starting values. Use readable markers and sparse measured-sample positions. Adjust after viewing the actual crop: thick strokes must not erase differences or obscure error caps. Small multiples may require less stroke weight but the same hierarchy.

A chart can feel forceful through full-strength resolved series colors, solid ink outlines and bold handwritten labels on white or warm-white. Deep colored heading bands are useful for a composite board, not mandatory on every tiny subplot. Preserve exact color/line/marker assignments across curves, tables and architecture legends. Record the chosen assignments once in the project brief, including how extra methods are distinguished. A large method count warrants another panel or a compact legend rather than many barely distinguishable neighboring shades.
