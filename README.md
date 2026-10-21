# Paper figures and tables

Active galleries split datasets by the saved C1/C4 comparison: select C4 only
when phase MAE decreases **and** phase SSIM increases on the same domain.
This is retrospective selection, not independent validation. Original C1
timing, reservation and training-sweep protocols remain separate; their values
are not C4 measurements. Each output has input-hash provenance. Main IC2 reconstruction images use C4;
C1 IC2 images are supplementary.

## Main figures

| Figure | Outputs under `figures/` | Scope |
|---|---|---|
| 2, local PtychoPINN-CI | [C4 primary](figures/fig2-experimental-gallery-B.png), [C1](figures/fig2-experimental-gallery-B-c1.png) | C4: TP2, IC1, IC2, NCM1. C1: microLFP single, Fly001, S200. Hybrid, PtychoPINN-CI C1, LSQ-ML; IC2 has a shared 192 px detail. TP2 is full-field only. |
| 2, timing | [C1 timing](figures/fig2-timing.png) | Inference, stitching and offset/tilt correction only; component breakdown and patterns/s. C4 and CNN timings are unavailable. |
| 3 | [Quality/time](figures/fig3-quality-vs-time.png) | Original C1 reserved-frame protocol; no corresponding C4 evidence. |
| 4 | [Decomposition](figures/fig4-decomposition.png) | Existing Fly/synthetic C1 stages. Saved TP2 C4 stages are supplementary. |
| 5 | [C4 scan-trained](figures/fig5-c4-scan-trained-main.png), [C1 scan-trained](figures/fig5-c1-scan-trained-main.png) | Synthetic-trained comparator remains C1; the C4 comparison does not isolate training source. |
| 6 | [Synthetic benchmark](figures/fig6-synthetic-benchmark.png) | Original C1 benchmark; no matched C4 campaign. |

Matching PDFs contain all pages; extra PNGs append `-page2`, etc. Main comparison
images omit the supplied reference; SI retains it. Scoring references, frozen
masks and evaluation gauges are unchanged. Fly is main and TP1 is SI. IC1 is
retained main with C4. TP2 may appear in comparisons but has no enlarged detail
or active FRC result: grid artifacts make its FRC interpretation misleading.

## Supplementary evidence

| Output | Basenames under `figures/` |
|---|---|
| S1 phase | `si1-resolution-c4`, `si1-resolution-c1` |
| S1 amplitude | `si1-resolution-amplitude-c4.png`, `si1-resolution-amplitude-c1.png` |
| S2 | `si2-c4-crossdataset-summary`; original `si2-data-efficiency` retains C1 training/pitch sweeps |
| S3 local PtychoPINN-CI | `si3-experimental-gallery-B-c4`, `si3-experimental-gallery-B-c1` |
| S3 amplitude | `si3-amplitude-gallery-c4`, `si3-amplitude-gallery-c1` |
| Fig. 4 C4 stages | `fig4-c4-stages-supplementary`; missing seed-only stage is explicitly unavailable |
| Fig. 5 | `fig5-c4-scan-trained-supplementary`; original C1 in `fig5-synthetic-generalization-supplementary` |
| IC2 grouping ablation | [C1 and C4, identical full field and detail](figures/si-ic2-c1-c4-comparison.png) |
| Conventional objective | Original `si5-synthetic-objective-check`, independent of grouping |

Whole-object C4 galleries contain TP1, TP2, IC1, IC2, NCM1 and ALS; C1 contains
the remaining five acquisitions. ALS qualifies for C4 whole-object display but
not heldout: heldout MAE improves while SSIM worsens. The
[selection CSV](metrics/model-selection.csv) and [JSON](metrics/model-selection.json)
record both arms, other metric tradeoffs, inputs and reasons. TP2's stored FRC
evidence is excluded from active resolution plots and summaries.

Unsuffixed main gallery A/B and Fig. 5 files are aliases of the selected C4
figures. The explicit C1 main companions show the other datasets; they omit
IC2. Original C1 IC2 images remain in SI and the paired grouping ablation.

## Comparison identities

`raw` already includes offsets; `polished_tilt` adds tilt seeding and field
refinement. **PtychoPINN-CI (CNN, C=1)** is our local CNN trained on the same
measured low half as Hybrid ResNet. It uses its own `unaligned` reconstruction,
with **no patch-offset alignment, tilt seed or phase-field refinement**.
Intrinsic CI VarPro and scalar count calibration remain. The shared global
evaluation gauge is applied for scoring/display. These are local measured-half
results, not images extracted from the prior paper or its synthetic-only recipe.

Main columns are Hybrid, PtychoPINN-CI, LSQ-ML; SI prepends Reference. B is
the canonical gallery filename. Former A filenames now alias the same local
computed comparison, including the matched IC2 detail; A/B no longer denote
different baselines. All eleven models and twenty-two whole/high-half records
passed the [local CNN audit](metrics/local-cnn-audit.json). Existing runs supply
every panel, so no training or inference rerun was needed.

CNM scan39 CNN failed to recover phase structure within 40 epochs. Native and
displayed objects match exactly on the scored mask; whole phase standard
deviation is 0.000194 rad and FRC50 is zero. Validation loss improved 2.38%.
The image is annotated as a poor fixed-budget result, not a converged
reconstruction. Its cause remains unknown; see the
[diagnostic receipt](metrics/cnm-cnn-diagnosis.json).

S200 galleries use historical **LSQ-ML2000 on 8,308 distributed patterns**,
versus 16,613 neural patterns. The solver exhausted its iteration budget;
convergence is not established. This image is neither the matched LSQ-ML100
timing comparator nor heldout evidence. See the
[mapping/scoring receipt](metrics/s200-lsqml2000.json). Computed S200 phase
panels share cyclic `twilight` colours from −π to π; amplitude and metrics
are unchanged.


`Patterns` counts displayed acquisition patterns; `Training` counts distinct
training patterns. Every C4 arm uses **10× training-group oversampling**:
ten four-pattern groups per training center. For IC2, 4,742 distinct training
patterns produce 47,420 groups. C4 is not compute matched to C1.
The [checkpoint/input audit](metrics/c4-oversampling-audit.json) verifies all
eight C4 candidate arms, including the six selected acquisitions. The saved
configuration counts unique centers; training consumes the expanded group
container. [Dataset metadata](metrics/datasets.csv) retains both counts.
The high half selects checkpoints and is spatial validation, not independent
testing; no footprint guard band separates halves. Whole images include the
training region.

The microLFP single and double acquisitions contain 5,625 and 3,750 patterns,
respectively, with different probes and fields. Matched dose, exposure and
registration are not established; they are separate acquisitions.

## Timing and scale bars

“Whole acquisition” reconstructs all patterns from both spatial halves; it
excludes training. Fig. 2 now times **inference (including intrinsic VarPro),
stitching, patch-offset correction and tilt/phase refinement only**. RAM
preparation, external transfers, frame selection, separate scalar count
calibration, loading, compilation, scoring and plotting are excluded.

All 22 C1 whole/heldout cases use one warmup of the measured dense field
implementation and three fresh trials on an otherwise idle RTX 3090. The
total is the median of per-trial component sums. Components below are from
the actual median-total trial, so they add to that total. Assembly inside
offset correction belongs to that column and is not counted twice.

| Whole acquisition | Patterns | Inference (s) | Stitching (s) | Offsets (s) | Tilt/refinement (s) | Total (s) | Patterns/s |
|---|---:|---:|---:|---:|---:|---:|---:|
| IC2 | 9,436 | 5.075 | 0.133 | 0.947 | 0.956 | 7.110 | 1,327 |
| Fly001 | 10,304 | 5.550 | 0.142 | 1.091 | 0.247 | 7.030 | 1,466 |
| S200 | 16,613 | 9.817 | 0.231 | 1.877 | 7.045 | 18.970 | 876 |

[Component timing CSV](metrics/core-timing.csv) includes both spatial cases
and identifies the timing boundary on every row. This reproduces the shown
C1 recipe with dense field evaluation, not the later compact implementation.
The saved raw ALS replay exactly reproduces its stored refined object;
fresh network runs have small numerical variation documented in the trial
receipts. S200 also stopped at 15 iterations in the bounded replay, under
the unchanged cap of 16; the [saved/fresh score comparison](metrics/s200-timing-quality-diagnostic.json)
records the numerical difference. Displayed images and quality scores were
not replaced. [All 22 timing receipts](metrics/core-timing-index.json) are
packaged with their source hashes.

Historical LSQ-ML100 times and Fig. 3 retain their wider host-to-host boundary;
no matched speedup is calculated against the narrower neural Fig. 2 times.
For context, the old whole-acquisition times were 8.389 s (IC2), 8.698 s
(Fly001) and 19.899 s (S200). The original `metrics/timing.csv` is retained.
Fig. 3 reserves frames before every fitting stage and uses the first sampled
LSQ-ML quality crossing without interpolation. C4 and CNN timings remain
unavailable; no C1 throughput is attributed to their images.

No verified object-plane nm/pixel calibration was recovered for the eleven
acquisitions. Bars remain in **pixels**; the
[metadata audit](metrics/acquisition-scale-audit.md) identifies the missing
sampling/resampling information. No units were inferred from raster bars.

## Reproduction

The C1 protocol `master_table` omits TP1, TP2 and IC1; complete SI evidence retains those
datasets. Selected model metrics are in `model-selection.csv`. Figure-specific
tables and receipts identify C1/C4 explicitly. Historical `whole.*`, `heldout.*`
and `<dataset>-whole.png` exports do not supply current comparisons.

Generators live in `scripts/studies/paper_figures/` in PtychoPINN. The active
plan is `docs/plans/2026-10-20-paper-c4-figure-variants.md`; it links the original
design, execution, CNN baseline and readability plans. Current gallery commands
and audit live under `.artifacts/paper-local-cnn-20261020/` in that checkout;
earlier figure commands and receipts remain under
`.artifacts/paper-c4-figures-20261020/`.
