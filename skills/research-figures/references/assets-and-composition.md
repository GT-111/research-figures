# Visual assets and hybrid composition

For reusable native motif recipes and an optional prepared material kit, read [asset-vocabulary.md](asset-vocabulary.md). This document owns genuine-media provenance and its pairing with evidence.

## Real entities have real visual sources

Render physical entities from project-owned geometry or use genuine photographs/simulation frames. Inspect the visual result: a successful renderer exit does not establish a useful image. A transparent static render demonstrates morphology only, not successful execution. Preserve mesh scale, joints, source path, camera, material and pose. Write project-local visualization code using the project's native renderer or an available mesh renderer; geometry preparation for its model format belongs to that project. Use original asset materials unless a neutral illustration is intentionally selected. Camera roll and view direction are explicit parameters. Check silhouettes at the actual figure size.

Use official project/repository media for benchmark or backend identities. Preserve aspect ratio and record provenance/license. If there is no published mark, use a native typographic name; do not invent a logo. A parent-company mark plus product text should be described as such. Native geometry is for mechanisms, not for approximating recognizable robot hardware. Existing screenshots, renders, photos and logos stay independent image objects.

## Source galleries and image-backed identities

When input diversity or benchmark/task breadth matters, collect representative original media for each displayed source from its official page or repository before reducing the input area to a list of names. Favor a real scene/frame/render over a screenshot of its framework, result chart or website chrome. Retain the original media and record crop/frame time. A dataset with both human and robot views can occupy both scientifically valid roles; its project identity alone does not determine the input representation.

A useful compact card is one genuine background image plus an independent editable typographic project name. Put the name on a small opaque ink/warm backing where it remains readable, clear of the hand/object/contact region. Use an original published logo separately when available. Repeated cards share caption baselines and frame dimensions; their crops preserve useful silhouettes rather than stretching or normalizing hardware into fictitious sizes. This composition is an option for a diversity argument, not a compulsory card grid for every figure.

Fit the photo region to its useful source aspect or choose an explicit scene-preserving cover crop; a tall shell around a centered landscape thumbnail creates empty space rather than a background visualization. Alpha-bounded hardware and off-center source crops need inspection in each exported renderer. A native picture crop and a nested SVG viewBox can produce different visible content; confirm that the complete intended silhouette/contact region appears, and baked source-title margins are absent where the recorded crop removes them. If a nonzero nested viewBox renders the wrong fragment, use a zero-origin viewport, explicit crop-sized clip and the original image translated by the negative crop origin. Preserve original media separately and correct the viewport/clip rather than filling the missing image with generated content.

Place source examples in their correct roles: a data-reference gallery, backend-context illustration and evaluated rollout are different things. Mark upstream examples as such in the figure/caption, and show project performance only from actual project evidence. A missing source image gets a named blank slot and an entry in the missing-input record; an attractive scene from another dataset is not a replacement.

When a source photograph provides context while the model consumes a different quantity, name that quantity at its inlet with a compact carrier (for example a pose window or native state). A recognizable background photo must not silently imply a new RGB/model-input modality. When imagery is the actual input, show its corresponding image/features route.

## Contribution-led generated composition

Use [generation-and-reconstruction.md](generation-and-reconstruction.md) for the default master workflow, including hybrid figures. Read project facts before composing. Genuine images are evidence-bearing inserts; a generated composition never creates that evidence. Preserve each actual asset as an independent picture during reconstruction.

## Task visual + measured result

Choose a composition from the actual argument:

- Repeated task columns: one task title; aligned success/throughput axes above; the corresponding task frame below. Put the shared method legend in a dedicated strip. Match cohorts and units, use consistent ranges for comparable metrics, and keep progress distinct from binary success.
- Sequence plus trace: horizontally aligned frames with real timestamps; observed/reference trajectories or contact/error traces directly below on the same time support. Mark actual events with aligned guides.
- Teaser plus evidence: larger real visual collage and one compact main metric/scaling panel. Use a short central claim only when it is backed by the displayed result. Avoid turning a teaser into a methods appendix.
- Failure analysis: paired success/failure frames with the same setup, a quantitative distribution or case matrix and a short failure category. Do not cherry-pick a qualitative comparison to imply a population effect.
- Scaling board: top row shows actual data/embodiment/task diversity; bottom row shows data, model, compute or rollout scaling on accurate measured coordinates. Control variables and held-out cohorts belong to the caption.

A figure can mix native architecture with rendered quantitative panels. Export each quantitative panel as SVG/PDF/PNG with its data and redraw code. Insert previews as independently movable images, alongside editable titles, legends and task imagery. Keep source attribution/evidence notes in speaker notes and the project brief. Illustrative data must be visibly labeled; source-paper task imagery is an example from that source, not project execution evidence.
