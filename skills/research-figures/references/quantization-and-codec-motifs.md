# Quantization, index and reconstruction motifs

Read when a figure must explain discrete representations, FSQ, VQ, residual quantization, codec training or decoder conditioning. These recipes describe different operations, not a compulsory codec architecture. Resolve the actual implementation first; counts, grids, codebooks, units and losses come from the project. Apply the current ink/type treatment around precise numerical carriers and native connections.

## Overview and operation detail have different scales

In an overview, several encoding lanes can meet one compact Quantizer, followed by a short regular shared-code carrier and clearly named parallel consumers. A few carrier cells are schematic; disclose the actual representation/count in the caption without turning those cells into an unsupported time/chunk axis. Distinguish a motion-reconstruction branch from a state-conditioned current-control branch by their names, inputs and outputs.

Expand fixed levels, rounding, IDs/restoration or training surrogates only when that operation answers the figure's question; use a local magnifier or companion mechanism figure. Four equal workflow boxes for routine quantizer internals can overpower alignment or control in the main framework. Follow the actual forward representation at its seam: a restored scalar vector, discrete scalar IDs and a packed token index are different carriers even when a reference calls all of them tokens.

## Fixed scalar levels: bound then round

Enlarge one channel into a small regular scale: a continuous value enters its bounded interval, then selects a fixed level through rounding. A few parallel channels and continuation dots can explain the repeated operation. Use short labels such as Scalar channels, Bound, Round and Fixed levels. The selected level preserves that channel's identity.

Supply channel count, per-channel levels, bound/offset/normalization and any projections. FSQ uses an implicit fixed quantization grid; do not depict a learned embedding table or codebook-update arrow. Encoder/projections can still learn. Straight-through training is a separate backward annotation, not a continuous forward bypass.

## Reversible index representation

If the interface packs discrete scalars, show the quantized group → Pack index → integer carrier, with Unpack restoring the same level group. If it keeps one level ID per scalar, preserve that actual arrangement. Index conversion changes representation; it is not another learned quantizer or a neural reconstruction.

Supply index ordering/range and the real packing interface. A decoder may consume the quantized vector directly; do not force storage serialization into every training forward. A Cartesian grid can illustrate combinations without enumerating all codewords. A scalar ID is not a continuous latent vector.

## Nearest learned entry

For vector quantization, show a continuous query vector selecting one learned entry. Highlight the same selected entry in a compact table and in a schematic local geometry view if useful. One whole vector selects an entry; this is different from independent scalar rounding.

Supply entry count/width, distance/normalization, sharing and position support. Use ellipses for omitted entries. Schematic points do not claim measured embedding distances or clustering. A fixed grid and a learned table need different visual mechanisms even if both emit IDs.

## Restore the representation before decoding

Distinguish IDs → Lookup/Restore levels → quantized vector → decoder → reconstruction. The actual API may combine the middle operations, but an expanded mechanism should expose what the decoder consumes. Pair original and reconstructed carriers at their comparison when the figure explains learning.

Supply learned lookup versus deterministic restoration, post-quantization projection, sequence order and output units. Do not connect raw integer IDs directly to a block labeled as consuming floating vectors while hiding the conversion. Reconstruction, a generated command and successful physical execution are separate outputs.

## Training relations and their recipients

Keep the discrete forward route solid and local. A training lane can show reconstruction updating decoder/encoder through the actual surrogate, an entry/dictionary update, and commitment updating its actual recipient. If the table uses EMA, depict that parameter update instead of implying a dictionary-loss gradient. A stop-gradient mark belongs on the relevant gradient path.

Supply implemented losses, gradient recipients, update rule and phase. FSQ does not automatically inherit learned-codebook or commitment objectives. Different table-update methods should not be combined merely to make the diagram detailed. Freezing all parameters is distinct from stopping one gradient.

## Serial residual refinement and accumulated contribution

Show at least one real subtraction: the current residual enters a quantizer; its selected vector contribution is subtracted to produce the next residual. Contributions also enter the actual accumulation/sum that produces the decoder representation. Each stage emits its index into a separate code carrier.

Supply stage count, quantizer type, table sharing, residual space and accumulation. Do not send every stage the same original input, add IDs as though they were vectors, or draw refinement depth as execution time. An arbitrary bitrate/prefix claim needs actual training/inference support.

## Position, stage and storage axes

A small code board can place real time/spatial position on one axis and scalar group or residual stage on the other. IDs cross a storage/transmission boundary and are restored on the receiving side when that is part of the method. Label each axis explicitly.

Supply token shape, ordering, position/rate and serialization. Show entropy coding or bit packing only when implemented. Multiple codes at one frame are not future frames; bitstream, integer carrier and floating decoder input are different objects. Quantitative bitrate and waveforms need actual data.

## Condition at its real consumer

Keep the code route intact while an independent condition enters the actual decoder/head operation. Expand the implemented combination when it is the contribution: concatenation, scale/shift, cross-attention or head selection. A target occupies the objective lane; it does not become an available inference condition.

Supply condition source/time, consuming layer, dimensions, phase and whether it must be transmitted. Do not infer conditioning from the word decoder. A code-only reconstruction decoder and a state-conditioned controller may be parallel consumers of the same representation; an executable controller need not consume the reconstructed signal.

Choose the one mechanism answering the reader's question and keep the others as small interfaces or caption detail. A quantization contribution deserves the level/entry operation; residual refinement deserves the residual update; a training or conditioning contribution deserves its actual recipient/combination. One overview need not display every codec recipe.
