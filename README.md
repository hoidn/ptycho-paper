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
| 2, matched CNN | [C4 primary](figures/fig2-experimental-gallery-B.png), [C1](figures/fig2-experimental-gallery-B-c1.png) | C4: TP2, IC1, IC2, NCM1. C1: microLFP single, Fly001, S200. Hybrid, CNN C1, LSQ-ML; IC2 has a shared 192 px detail. TP2 is full-field only. |
| 2, prior fragments | [C4 primary](figures/fig2-experimental-gallery-A.png), [C1](figures/fig2-experimental-gallery-A-c1.png) | Attributed published rasters are illustrative, not rescored. |
| 2, timing | [Historical C1 timing](figures/fig2-timing.png) | The narrower inference/stitching/offset/tilt remeasurement is running; this file still shows the historical host-to-host measurement. |
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
| S3 matched CNN | `si3-experimental-gallery-B-c4`, `si3-experimental-gallery-B-c1` |
| S3 published fragments | `si3-experimental-gallery-A-c4`, `si3-experimental-gallery-A-c1` |
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
refinement. Matched CNN B uses C1, the same measured training half, CI VarPro
and scalar count calibration, with **no offset, tilt or field correction**.
It is not the published synthetic-only recipe. B order is Hybrid, CNN, LSQ-ML,
then Reference in SI only.

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

ALS's prior fragment is **NS** in arXiv:2608.02869 Fig. 2, “+Synthetic Data
only.” It shows the same specimen field, but the relationship between its
960 patterns and the current 1,444 is unknown. The original scale is retained;
see the [source audit](metrics/als-ns-reference-match.json). Prior fragments
are cropped and rescaled under CC BY 4.0. Missing cells say “No verified panel.”

`Patterns` counts displayed acquisition patterns; `Training` counts distinct
training patterns. C4 uses ten groups per training center and is not compute
matched to C1. [Dataset metadata](metrics/datasets.csv) retains group counts.
The high half selects checkpoints and is spatial validation, not independent
testing; no footprint guard band separates halves. Whole images include the
training region.

The microLFP single and double acquisitions contain 5,625 and 3,750 patterns,
respectively, with different probes and fields. Matched dose, exposure and
registration are not established; they are separate acquisitions.

## Timing and scale bars

“Whole acquisition” reconstructs all patterns from both halves, not training.
Host-to-host timing includes per-acquisition RAM preparation, transfers,
inference/VarPro, stitch/offset alignment, count gauge and applicable tilt/
refinement. It excludes model/process loading, compilation, scoring and plots.
Measurements use one warm-up and three fresh trials on an idle GPU.

| Whole acquisition | Patterns | Polished C1 seconds | Patterns/s |
|---|---:|---:|---:|
| IC2 | 9,436 | 8.389 | 1,125 |
| Fly001 | 10,304 | 8.698 | 1,185 |
| S200 | 16,613 | 19.899 | 835 |

Fig. 3 reserves frames before every fitting stage and uses the first sampled
LSQ-ML quality crossing without interpolation. Its membership receipts and
original `metrics/timing.csv` are unchanged.

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
design, execution, CNN baseline and readability plans. Current render commands
and audits live under `.artifacts/paper-c4-figures-20261020/` in that checkout.
