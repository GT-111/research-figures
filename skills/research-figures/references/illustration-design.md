# Design an illustration that explains the contribution

Read for a new paper teaser, framework, mechanism or evidence board, and when a user says a figure is attractive but unclear. This document owns explanatory reasoning and learning from relevant paper figures. Scientific topology belongs to the current project; typography, palette and rendering belong to their existing references.

## Start with the reader's question

Write one concrete question the figure answers and one sentence the reader should be able to explain after seeing it. A framework might explain how the new mechanism changes the path from input to output; a mechanism might explain which information an update consumes and what it changes; a teaser might connect a new capability to visible evidence. The name of a model or a list of components is not that explanation.

Extract the contribution from project text and implementation before looking for a layout. Identify the limiting behavior, the actual change, the intermediate operation causing the change, and the output/evidence it affects. Distinguish a new mechanism from standard infrastructure. Do not declare novelty based on a visually prominent module. If the scientific change cannot be named, narrow the figure's job rather than decorating the whole repository.

## Figure job determines the explanation

| Figure job | What it must let the reader understand | Content emphasis |
|---|---|---|
| Teaser | The capability/problem and its concrete consequence | Genuine representative scenes, a compact contribution cue and justified evidence |
| Main framework | How the contribution fits the method and changes the input-to-output path | Essential interfaces, the focal mechanism and distinct execution/training lanes |
| Mechanism detail | How the new operation works on its inputs | A worked representation/state/geometry example plus its actual transformation |
| Training/adaptation | Where learning evidence comes from and which parameters/state change | Sampling/supervision, objective/update recipients and time/evidence boundaries |
| Results/ablation | What comparison answers the scientific question under which conditions | Accurate metric/cohort/axes, supported variants and uncertainty |
| Failure/diagnostic | What observed behavior supports the proposed explanation | Matched cases/traces, actual event alignment and stated scope |
| Scaling | Which independent variable changes the outcome | Actual exposure and controls, held-out evaluation and measured trend |

Choose the figure job before considering application-specific examples. Optional [robotics-layouts.md](robotics-layouts.md) supplies worked patterns learned from robotics. Use a relevant pattern after identifying the actual relations; unfamiliar methods use the same general reasoning and can draw references from any appropriate domain. Several jobs usually require several figures rather than a single plate that tries to explain the whole repository.

## Read relevant original figures for explanatory moves

For a new paper-grade design, inspect a small set of relevant original figures, normally two to four. Select by the explanatory relation needed: a comparable transformation/conditioning/update, a compatible interface or time structure, and an evidence composition when results are involved. Useful references may come from another application domain. The project's related-work citations are a useful starting point; supplied references take precedence for visual appearance. Read the paper's figure and caption plus the method passage needed to understand its arrows. A similar topic or venue alone does not make a layout suitable.

Keep source/version/figure/page pointers in the project-local brief. For each useful reference, record the reader question it answers, how it allocates the focal region, what its arrows and visual carriers mean, and the explanatory move worth adapting. Examples: a shared model surrounded by several conditioning cases; matching before/after representations; an expanded update inset; a split control-command versus training-target route; aligned task images and metric columns. Read pixels, not just captions. Interpret repeated blocks carefully: they may denote time, shared parameters, alternative modes or genuinely separate modules.

Choose the explanatory move because it matches the project. Style references inform color/ink/type; mechanism references inform how to expose the project facts. Neither supplies a missing module, loss, gradient, tensor dimension or validated result. A paper's fictionalized schematic robot is not a substitute for a current project's genuine hardware asset.

Reuse a still-relevant prior figure study for later figures or a pure color revision. Targeted reading ends when a useful explanatory arrangement is justified; a new bibliography is not a prerequisite to editing a label. If source access is unavailable, use supplied/readable references and disclose that limit while continuing the grounded figure.

## Transferable scientific relations

Reduce the project to the relations the reader needs to understand. These relations transfer across domains; a method name or application category does not select the diagram.

| Relation | What to expose | Useful representation/arrangement |
|---|---|---|
| Transformation | How one representation becomes another | Before/after carriers around the actual operator, with important units/frames |
| Conditioning | Which information controls an operation without becoming its output | Distinct condition entry and output route; small interaction/selection example |
| Selection / constraints | What can change and which constraints determine the choice | A meaningful mask/set/feasible-region example, exact selection or solve step |
| Shared structure | What is reused across cases and what differs | One shared core plus aligned settings/instances; explicit shared-parameter association |
| Iteration / feedback | What is carried to the next step and what exits | Update operation, state carrier and labeled loop; separate different clocks |
| Learning / adaptation | Which evidence modifies which parameters/state | Evidence → objective/update → recipient, with availability and phase boundaries |
| Hierarchy / interfaces | Which level delegates what to which execution component | Named interface carriers and unequal levels, rather than uniform process cards |
| Comparison / intervention | Which controlled change leads to which observation | Matched branches, before/after or supported ablation, aligned measurement |
| Evidence / uncertainty | What population or samples support the claim | Genuine qualitative context paired with exact data/cohort/statistic definitions |

Identify roles such as observation, representation, operation, stored state, condition, target, output and evidence, then distinguish the applicable relations. A single arrow style cannot silently mean computation, shared weights, gradients and time order. Separate carrier properties from operational roles: a clean value can be an observed condition or a generated output, so a clean/noisy glyph legend must not identify both as conditioning/marginalization. One module may participate in several relations; use a local detail figure if the overview cannot explain that cleanly.

When the representation is itself a graph, separate its internal edges from the framework's computation arrows. Containment, spatial adjacency, association and navigable connectivity describe different relationships. Show a small labeled example of the relevant edge type, then connect the whole representation to its consumer. An object hierarchy can answer a semantic query without specifying a collision-free route; expose the separate geometric operation when execution depends on it. Keep map/graph construction distinct from later query or planning, and show an online update only when the method performs one.

Choose a minimal worked example when an operation is otherwise hidden in a label. It may be a matrix update, a selected subset, a changed spatial relation, a conditioned prediction or a state transition. Its entities/operation must reflect the method; illustrative values are explicitly schematic. The example explains an operation, not an invented experimental gain.

## Make a content hierarchy before coordinates

Place the contribution-defining operation in the focal region. Keep enough input context to understand it, enough output to show its consequence, and subordinate standard preparation. Separate overview and local detail: a broad framework shows interfaces; a zoomed mechanism shows the operation that would otherwise remain a named box. Move exhaustive derivations/configuration to the caption or appendix.

Use reader-facing role names before implementation symbols: “Motion reconstruction” or “Closed-loop controller,” with a compact symbol only if the caption needs it. A repository class name, decoder index or adapter ABI rarely explains an operation to a new reader. Keep exact dimensions, serializers, dispatch/bounds details and engine plumbing in notes unless that interface is the contribution. Show the unchanged supported component inventory there when the overview selects fewer examples.

When several representations become compatible, expose the relationship that makes them compatible. Distinguish correspondence/alignment, reconstruction and control learning. Show the actual paired carriers or supported common frame, the alignment objective and its learning recipient in a compact training inset; matched colors or arrows converging into a box do not establish alignment. Resolve temporal support, geometric frame and semantic pairing from the project, rather than treating these different meanings of “alignment” as interchangeable. Preserve the continuous/discrete level at which the actual comparison occurs.

Give every visible object a job: physical entity, observation, representation, operation, stored state, condition, supervision, result or annotation. Select a faithful carrier: time-aligned frames for temporal evidence, regular cells for a mask, matrix/operator for an actual update, spatial relation for geometry, sequence bracket for a command chunk. Use real assets for physical identities. Generic neural nodes only indicate a learned map; they cannot explain an unknown mechanism.

Use verbs on a few important transformations (encode, select, condition, solve, update, execute) and short nouns on representations. Preserve important representation changes: poses becoming constraints, observations becoming latents, predictions being combined with measured values, or commands entering a simulator. One repeated box family for every object hides these differences.

## Arrange according to dependencies

Choose a main reading route, then reserve space for feedback, training and alternatives. Unequal regions should reflect explanatory importance. Align comparable branches at the points where their inputs/operations differ; do not force every stage into equal cards. Draw junctions and crossings distinctly and keep captions in free corridors.

Let serial/parallel computation read as one connected composition when that is the method's structure. Region headings, spacing and restrained color can organize inputs, shared operations and outputs without enclosing every stage in a separate panel. Use an enclosing boundary when it communicates shared parameters, ownership, an optional/frozen subsystem, a training-only scope, or an independent comparison. A panel division that merely mirrors the repository folders can conceal a continuous method path. Independent experiments, distinct clocks and genuinely separate explanations can still deserve panels; choose from the actual dependency structure.

If an open composition leaves the focal mechanism hard to locate, emphasize one coherent core with a restrained background and a labeled irregular boundary, keeping its serial/parallel operations continuous inside. Leave input context, external execution and genuinely optional components outside when those are their roles. Give the boundary clearance from node contours, captions and route shafts; it must not cut a carrier or resemble an extra feedback path. An outline expresses the named scope, so distinguish emphasis from training/frozen meaning with a short label and fill hierarchy. Use the boundary needed for comprehension rather than boxing every stage.

Select visible relations by the reader question rather than by the number of dependencies in code. A main figure can abbreviate standard preparation and repeated calls in its caption, while a local inset exposes the operation that matters. When routing becomes tangled, reconsider which relations belong at this level before adding bends or expanding the canvas. Dense mechanisms and sparse connecting paths can coexist; density is not a target edge count. For endpoint ownership and native arrows, use [connector-design.md](connector-design.md).

- **Joint/shared models:** one shared core with clearly labeled inputs/outputs; compact use cases show the actual changed conditions. Repeated simplified operators can clarify different paths when an explicit shared-parameter label prevents implying separate weights.
- **Conditioning or attention:** attach conditioning to the operation that consumes it. A compact interaction/mask diagram can expose structure that an unexplained “attention” box conceals. A structural association is not automatically a causal computation arrow.
- **Updates and memory:** show what is read, when new evidence becomes available, the local update, and what the next decision reads. A temporal strip or state transition is more explanatory than a large cylinder labeled memory.
- **Nested loops:** show their different clocks and quantities. Iterative solver/denoising updates are distinct from execute → observe → replan; their exits come from the actual producer of the final output.
- **Training versus execution:** future targets, teachers and losses occupy a separate lane/inset with explicit boundaries. When learning is part of the figure's question, connect predicted quantities and actual targets/evidence to the objective and its parameter/state recipient; dataset names or sampling rules alone do not explain learning. Parameter freezing, stop-gradient and inference absence are distinct facts.
- **Execution supplies learning evidence:** place the environment/executor beside the command and observed consequences it actually produces. Keep command → execution → observation/rollout → objective/update → parameter recipient visibly connected when that loop explains the method. Training annotations can occupy a quieter adjacent lane while remaining part of the dependency structure. A detached inventory of simulator/backend names cannot explain execution or learning; selected and alternative executors need explicit status.
- **Multiple embodiments/backends:** shared representation and per-system adapters have distinct roles. Depict the common interface before parallel native execution lanes; mark planned/validated scope explicitly.
- **Evidence boards:** align actual task/condition images to the measured cohort. Temporal traces share frame support; comparison panels share metric definitions and scales. A selected example is not population evidence.

These are layout decisions, not model assumptions. Use only the structures the project actually contains.

## Show structural alternatives as visual comparisons

When the reader must understand how modes, conditions or variants change computation, use aligned miniature diagrams with consistent carrier positions. Expose the changed input availability, connection, operation or output directly. For example, held-clean, excluded/noisy and generated variables need visually distinct carriers and an operation/route that shows what happens; a row of parameter settings makes the reader reconstruct that behavior mentally. A large shared mechanism can supply the detail once, while the small cases show only the meaningful differences. Label shared parameters where needed. Do not reproduce the whole implementation in every case.

A table is useful when its job is precise lookup of configuration, dimensions or results. It does not replace the contribution's operation or dataflow. A comparison inset earns its space only if it exposes a relevant difference; a roster of named capabilities does not. The shared mechanism must honor the settings shown in its cases: distinguish active and held paths, and attach termination/output to the actual active operation. A case inset cannot repair a contradictory unconditional route in the main mechanism. Controlled architecture variants, alternate sampling settings and measured ablations have different scientific meanings. Keep them distinct, and do not add a baseline or an experimental claim merely to create a contrast.

## A compact scene plan

The project-local brief should now explain: the reader question, contribution-defining operation, chosen reference-derived explanatory move, main route and supporting lanes, exact representations/relations, one meaningful internal mechanism, required genuine assets/evidence, and what belongs in the caption. A brief can use a short paragraph and a sketch; no universal diagram schema is required.

Only then choose region bounds and generate the visual master. Tell the generator which fact must be visually legible, which operation is enlarged, and which paths must remain distinct. Specify exact displayed labels separately from explanation/layout instructions. Strong colors and rough ink emphasize this hierarchy; they do not supply it.

## Judge explanation on the actual render

Read the delivered figure as a reviewer unfamiliar with the repository. Trace the core input through the new operation to the output; identify where conditioning and supervision enter; distinguish execution from training and each feedback clock. State the contribution using only the visible content and its caption. If that requires knowledge hidden in the repository, revise the missing representation or operation rather than adding more decorative nodes.

Inspect whether the prominent region actually explains the change. A figure with all method boxes and correct arrows can still hide the contribution if the crucial operation remains an empty label. Conversely, a simple well-chosen state/mask example can explain more than a complete implementation graph. Compare a single intervention/baseline only when the project supports it; explain what changes, without inventing an ablation result.

Use direct judgment, not an aesthetic score or a ritual checklist. Fix the observed ambiguity, misleading path or missing explanatory step. Technical captions complement the illustration; they cannot repair a contradictory arrow or an unsupported evidence claim. Preserve useful density, editable effects and exact numerical geometry while making that correction.

For an original-paper reproduction trial, compare explanatory structure with the selected source figure after native rendering. Trace the same question in each: where inputs enter, how the focal operation is exposed, what remains fixed versus changes, and which operation actually produces the output. Record concrete information preserved, lost or made clearer, with source figure/page and the inspected artifact version. This comparison concerns explanation, not matching colors or copying coordinates. Preserve the earlier render when repairing an observed structural failure so the before/after can be assessed. Apply the resulting lesson to the relevant relation, not as a compulsory layout for unrelated methods.
