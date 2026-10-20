# Paper figures and tables (2026-10-20)

Generation checkout commit: `3f0ae0c7c`. Per-output provenance is authoritative.

Headline model: Hybrid ResNet C=1; C=4 appears separately in the SI table. Conventional baseline: fixed-probe LSQ-ML100; timing curves extend through 200 sweeps. The measured low half trains the network. The high half selects checkpoints and is scored as spatial validation, not an independent test; no guard band separates probe footprints.

`raw` already includes patch-offset alignment. `polished_tilt` adds the tilt seed and phase-field refinement. The CNN C=1 baseline uses the same measured training half, CI VarPro and a scalar count gauge, with no offset alignment, tilt seed or field refinement. It is not a reproduction of the published synthetic-only recipe; its matched timing is unavailable. Measured references are experimental estimates. Display shows full supported objects with the scored boundary marked; global gauge and object metrics use one common physical anchor and probe-radius interior per comparison.

| Output | Figure basename under `figures/` | Generator module | Content |
|---|---|---|---|
| Fig. 2 | `fig2-experimental-gallery-A/B` | `experimental_gallery` | Full supported measured objects; A: cited prior-paper fragments, B: matched measured-half CNN without offset/tilt correction. |
| Fig. 2 timing | `fig2-timing` | `quality_vs_time` | Matched all-frame inference and LSQ-ML timing for every acquisition and case. |
| Fig. 3 | `fig3-quality-vs-time` | `quality_vs_time` | Reserved-frame prediction versus matched host-to-host elapsed time. |
| Fig. 4 | `fig4-decomposition` | `decomposition_figure` | Offset alignment, tilt seed, phase refinement and flat controls. |
| Fig. 5 | `fig5-synthetic-generalization` | `synthetic_generalization` | Linked generation example and synthetic-trained versus scan-trained models. |
| Fig. 6 | `fig6-synthetic-benchmark` | `synthetic_benchmark` | Ten synthetic objects and three neural seeds versus LSQ-ML200; paired object bootstrap intervals. |
| S1 | `si1-resolution; si1-resolution-amplitude` | `resolution_figure` | FRC curves, common crops and profiles; the amplitude companion is PNG only. |
| S2 | `si2-data-efficiency` | `data_efficiency` | Training-frame and acquisition-pitch sweeps. |
| S3 | `si3-experimental-gallery-A/B; si3-amplitude-gallery` | `experimental_gallery` | Remaining experimental datasets and amplitude comparisons. |
| S5 | `si5-synthetic-objective-check` | `quality_vs_time` | Gaussian versus Poisson LSQ-ML on the same reserved synthetic acquisition. |

Tracked generators are in `scripts/studies/paper_figures/`; main figures have PNG and PDF versions. Metrics and SHA-256 input provenance are under `metrics/`.

| Table | Files under `metrics/` |
|---|---|
| Main comparison | `master_table.md`, `.csv`, `.tex` |
| Extended metrics and C=4 | `si_table.md`, `.csv`, `.tex` |
| Acquisition and training metadata | `datasets.md`, `.csv`, `.tex` |
| Matched timing trials | `timing.csv` and referenced trial receipts |

Fig. 2 timing uses the all-frame protocol. Fig. 3 reserves score frames before every fitting stage; its receipts record coverage and membership. Timing includes transfers and scan setup, excludes model loading/compilation, scoring and snapshot I/O, and uses one warm-up plus three fresh trials on an idle GPU. Training is reported separately.

Fig. 3 ratios use the first sampled LSQ-ML checkpoint reaching the polished quality; they do not interpolate the crossing time. Geometry-preserving replacement reserves contain 439 CNM frames and eight synthetic frames (12,441 and 2,040 fit frames, respectively). The frozen scoring domains and support thresholds are unchanged.

Native diffraction scores use common complete windows on each native object, before reference alignment. Unavailable deviance is `n/a`, including arbitrary-intensity datasets; unknown physical acquisition metadata is `unknown (ask)`.

Previous-best fragments retain their original colour bars and a dashed boundary; they are illustrative, not rescored baselines. Missing fragments say “not reported”.

Older `<dataset>-whole.png`, `heldout.*` and `whole.*` files are historical exports. They do not supply the current figures or cross-model comparison tables.

Execution and reproduction: `docs/plans/2026-10-19-paper-figures-implementation.md`; scientific protocol: `docs/plans/2026-10-19-paper-figures-design.md`; CNN baseline: `docs/plans/2026-10-20-paper-cnn-baseline.md`.
