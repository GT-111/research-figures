# Routing, sequence and streaming motifs

Read when illustrating sparse routing, autoregression, aligned multimodal tracks, within-step prediction or streaming readiness. Select by the actual operation and reader question; these recipes transfer beyond language/audio. Project counts and dependency rules determine the picture. Use regular indexed carriers, the current type/palette and native connector grammar.

## Selected experts and any independent shared path

One token supplies features and router scores. Show an expert bank with its true total count or an explicit schematic count, highlighting only the selected computation paths for this token. Their outputs enter a weighted merge. An always-on expert path bypasses the router only when the current method has one. A dense variant uses its real mapping rather than a decorative router.

Supply total/selected counts, routing and weight normalization, expert ownership and merge operation. Activation color means selected computation, not trainability. Shared expert computation, shared weights across calls and shared input representations are different facts. Do not infer a shared branch from another model's architecture.

## Generated output becomes later history

Two adjacent steps can show the dependency more clearly than a page-wide loop: the current output passes through its actual selection/sample/embedding operation, enters the history carrier and becomes next-step input. A compact overview may fold this into one labeled local repeat. If a cache exists, give its reads/writes a distinct state lane.

Supply generated versus teacher-forced history, output type, step index/delay, termination and cache behavior. Feedback returns to the consuming history/input operation; a waveform cannot be fed back into a token-only model. Cache maintenance and output-token recurrence are separate relations. See connector-design.md for continuous native return paths.

## Aligned tracks with an explicit combination

Two carrier rows share the supported temporal columns. Distinguish padding/absence from actual values; a named combination operation states whether the tracks concatenate along channels, sum or interact another way. Prefix, generated and optional sections can use short brackets before the common trunk.

Supply alignment/offset, padding semantics, combination axis and phase. Two tracks do not establish two models or two output heads. Time positions, representation channels and attention visibility need distinct notation. Do not imply exact word-to-frame correspondence when the method does not provide it.

## Across-step versus within-step prediction

Arrange execution time horizontally and the codes/components belonging to one step vertically. A base prediction can feed a smaller within-step predictor, followed by aggregation of that step's required codes and its decoder. Cross-step feedback stays on the temporal route; within-step dependencies remain local.

Supply component counts, base/residual ordering, parallel versus sequential dependencies, aggregation and step rate. Codebook depth is not a future-time axis. A head dependency is not a training-stage sequence. Show only the branches the implementation has; input tracks alone do not prove separate heads.

## Prefix, reference-derived condition and identity

A prefix is a bounded part of the actual input sequence. A reference sample enters its real encoder before its condition embedding reaches the actual injection point. Paired in-context examples remain a paired prefix. Alternative conditioning modes use a selection/comparison inset rather than an unsupported mandatory chain.

Supply prefix versus cross-attention/additive injection, required/optional/exclusive inputs, availability and encoder ownership. A learned identity vector, a natural-language instruction and a supervised label are distinct sources. Genuine reference imagery is an independent insert; a schematic signal must be labeled accordingly.

## Readiness, first output and steady-state windows

Use separate lanes for generated carriers, decodable blocks and emitted packets/results. Show left context, current block and actual lookahead support. A first-output waiting bracket ends at the last required input, then connects decoding and emission; one later cycle can show steady-state behavior. A strictly causal method has no future-support window.

Supply chunk size, context, rate, output grouping and any measured processing latency. Distinguish content duration, input wait and compute delay. Without measured times, show dependencies/order rather than fabricated milliseconds. An inverse token rate is not a measured first-packet wall-clock delay.

## Supervision and checkpoint evolution

Keep teachers, discriminators and reconstruction targets in a training side lane reaching the actual objective/update recipient. When phase evolution is the reader question, use a separate checkpoint → training operation → checkpoint track. A teacher's supervised transfer reaches student training; it does not imply a deployment cascade.

Supply trainable/frozen state, loss domain, phase ownership and retained computation. Optional, training-only and frozen are different properties even when their source figures use dashes. Define the local line semantics. Residual code refinement is covered by quantization-and-codec-motifs.md; do not infer it merely from multiple output codebooks.
