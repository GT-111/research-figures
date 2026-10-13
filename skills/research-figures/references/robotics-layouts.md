# Robotics-derived explanatory examples

This optional casebook turns familiar robotics work into examples of the general relations in illustration-design.md. Start from the figure job and actual transformation, condition, constraint, state update, shared structure or evidence relation. Use a relevant example for insight; extend the same reasoning to unfamiliar methods and other domains. A framework, mechanism, training diagram and result board select different detail from the same method.

## Learn explanatory moves from robotics examples

| Robotics example | Contribution often needs to expose | Useful compact visual |
|---|---|---|
| BFM / behavior foundation model | Shared behavior representation and how conditions select/control behavior | Conditioning cases around one shared core; structured goal/state carrier |
| WBC / whole-body control | Goal decomposition, native commands, coupled contacts/dynamics and feedback | Reference/command → policy/controller → plant loop; body/contact or time-aligned inset |
| VLA | How visual/language/state information conditions actual action generation | Aligned modality carriers, expert interaction detail, explicit action representation |
| WAM / world-action model | What is predicted, how action and world information interact, and what prediction supports | Aligned time/action/state lanes; shared model with actual conditioning settings |
| Tracking / retargeting | Reference construction versus closed-loop realization; error/constraints used | Matching reference/achieved traces, geometric relation or solver/feedback inset |
| Residual / online adaptation | Where correction enters, what evidence it can use and what changes online | Nominal and correction paths meeting at the true operation; read/update timeline |
| RL / policy optimization | Interaction data, reward/target construction and the actual parameter update | Rollout/data lane plus evaluator/update lane; explicit collection/update clocks |
| Mapping / navigation | Association across observations, stored spatial structure and how a goal becomes a feasible route | Matched observation/map inset; semantic hierarchy beside geometric connectivity and selected route |
| Tactile / geometric perception | What measurements reveal, registration and the inferred physical quantity | Registered sensor/object views, actual contact or correspondence inset, prediction/reference pair |

Select an operation the reader must understand, then use one of these visuals to show it. A topic label alone is not a reason to add every object in its row.

## BFM: shared behavior and controllable conditions

Show the common behavior interface and representation before expanding embodiment-specific adapters. If a control mask selects parts of a goal, show one small meaningful goal/mask/result example. If task codes, latent skills or another conditioning mechanism is used instead, show that actual operation. A shared core can occupy a broad region with alternative conditions next to it; separate preparation and learning if they use different information. Do not imply distinct weights by repeating the model for each use case.

Show pretraining coverage with genuine motion/behavior examples and actual data categories. Privileged encoders, priors, decoders or distillation belong only when implemented/described. Label which paths survive inference. A generic latent Gaussian/network drawing cannot establish the representation's mechanism. Scaling evidence separates amount, diversity and embodiment coverage; sharing a model alone does not establish unseen-body generalization.

## WBC: commands, dynamics and achievable motion

Name the real command space: velocity, pose, keypoint, joint target, torque or another supported interface. Show how high-level goals reach body/limb controllers and what measured state closes the loop. Contact support, coordinate frames and morphology deserve a small inset when they determine the contribution. Genuine robot sequences or renders communicate geometry; code-native stick robots cannot substitute for the real embodiment.

Place imitation/reward, privileged observations, domain randomization and optimizer in a separate training region when used. Multi-rate control needs a small timeline or explicit clocks: policy decisions, actuator commands and simulator integration differ. When whole-body coupling is the novelty, expose the coupling/contact relation rather than drawing an empty “whole-body policy” box. Sim-to-real evidence distinguishes simulation, physical collection and deployment stages.

## VLA: conditioning and action generation

Align visual/language/proprioception carriers by their actual roles. Put tokenization/encoding next to the source; show where context conditions generation. A backbone/expert diagram may include a compact interaction or attention-mask inset when that is the contribution. Features, cache and expert association have different meanings from computation arrows.

Distinguish discrete action-token prediction from continuous flow/denoising or direct action regression. For iterative generation, display the update operation that produces the next/final action and reserve a distinct execution feedback route. Future/video teachers and targets belong in training only unless the method has an actual inference route for them. A frozen label describes parameters, not all recurrent state. Show real robot action-space interfaces without inventing a robot identity.

## WAM: world and action information over time

Identify the predicted entity: pixels, visual latents, physical state, reward, action or a joint distribution. Align observation/action/outcome at the same temporal support. Label conditioning versus prediction and measured versus imagined outcomes. For a joint/shared model, aligned graphical conditioning cases can show what is supplied, held or sampled without repeating full model detail. Use settings tables for precise lookup when needed, rather than asking them to explain the operation. Independent sampling/noise clocks need their own notation.

Choose the downstream use from the project: direct policy generation, planning, ranking candidates, imagined rollouts, supervision or online correction. Show the operation that turns prediction into the claimed use. A visually plausible future is not automatically a usable learning signal or controller. Training targets/teacher forcing and inference inputs stay distinct; generated next frames are not genuine execution evidence. Align qualitative prediction comparisons with real timestamps and exact error/progress traces when available.

## Tracking and retargeting: reference versus realization

Separate offline geometric reference construction from online feedback. Retargeting explains source geometry, correspondences/task-space relationships, target morphology constraints and the actual solver/output interface. A compact before/after correspondence or constraint example often explains more than a long list of optimizer terms. Freeze, companion outputs and physical feasibility have their actual scope.

Tracking shows the reference representation, actual measured state, commanded action, plant and feedback. A reference/achieved overlay or aligned pose sequence can reveal phase, contact or geometry error; units and frames are explicit. Enlarge the reference selection, state conditioning or error transformation when it is new. Keep unavailable future measurements outside causal inputs. Success, tracking error, task progress and constraint satisfaction are different results; choose evidence that answers the figure's question.

## Residual and online adaptation: information and insertion point

Show the nominal output and the correction's insertion point: action, latent, dynamics prediction or another actual quantity. Use an addition symbol only for an additive correction; gating, blending, postprocessing and parameter updates are distinct operations. Name the corrected quantity and preserve its units. A nominal controller is frozen only when that is true.

Make feedback availability visible. Show what is read before execution, which observations arrive afterward, how fast state/weights change, and what the next decision consumes. Support/query or before/after state strips are useful when the update order is central. Slow offline weights, online fast weights and factual memory have distinct roles. TTT is not automatically RL or a residual sum. Reset/publication boundaries belong in the figure when they explain causality or evidence ownership. Avoid implying gains when only the adaptation mechanism is implemented.

## RL: collection, evaluation and optimization

Read the actual algorithm before choosing actor/critic, replay, advantage or model-based imagery. Arrange collection and update as distinct lanes connected by the data they actually exchange. Label observations, actions, reward/termination and bootstrap/return/target construction where these matter. Show the update's recipient parameters and distinguish behavior/target/frozen components when used. Some methods have no critic, replay buffer or online simulator.

For on-policy versus offline/off-policy learning, show the real source of samples and when data are reused. For model-based/imagination learning, distinguish genuine experience, predicted outcomes and evaluator signals. Multiple environments/backends share an interface and update only when the implementation does. Reward and gradient/update arrows have separate meanings. Learning curves use actual exposure/time and appropriate run-level uncertainty; selected rollouts do not establish population success.

## Mapping and navigation: representation versus route

Identify what the map stores and how observations enter it: occupancy, geometry, object identity, semantic features, uncertainty or a combination. Show a small association/fusion example when it is the contribution; repeated views of one object are not automatically different objects. State the pose or registration input used to put observations in a common frame, especially when it is provided rather than estimated by the method.

Keep semantic structure and traversability separate. A room/object hierarchy, an adjacency graph and a collision-free route have different edge meanings even when they share one scene. Let query grounding identify a goal, then expose the actual planner/connectivity representation that produces the route. Map construction may be offline while navigation is online; use temporal scope rather than adding a speculative closed-loop map update. Genuine map/trajectory overlays retain their coordinates and camera projection; conceptual module arrows follow the normal orthogonal routing rules.

## Tactile and geometric perception: measurement versus inference

Show the measured modality and the quantity estimated from it. A tactile image, contact force, deformation field, reconstructed surface and inferred material property are different carriers. A matched sensor/object inset can establish correspondence without turning every stage into an encoder block. Name the reference frame and synchronization when comparing touch, vision, geometry or motion; separate visible observations from ground-truth supervision and latent estimates.

Preserve true spatial structure in contact patches, flow fields and correspondences. Qualitative panels use matched contact state, load or timestamp when the claim depends on them, and disclose unmatched conditions. Indicate unobserved/occluded regions independently of predicted value; a blank region is not evidence of zero force or free space. Use genuine sensor/render assets for measured scenes, and label a conceptual contact sketch as schematic.

## Data, backend and scaling figures

Data-generation figures explain source → transformation → validity/QA → capture/export, with planned/implemented/verified status. Genuine observation channels and logged contracts can expose completeness; renderer or simulator logos come from official sources. Sampling distribution, source weights and shared optimization are separate from runtime backend orchestration.

Separate reference diversity, rollout quantity, model parameters and compute. Use matched plots or a two-factor matrix for independent factors. A conceptual data pyramid is not a quantitative scaling law. Task photos, trajectory overlays, pose sequences, transfer matrices and embeddings each serve different questions. Embeddings require recorded projection/settings and cannot establish causality. Numeric layouts/aggregation follow results.md; ink and colors follow the selected profile. Preserve useful density through mechanisms and aligned evidence, not smaller type.
