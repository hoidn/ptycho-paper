# Synthetic benchmark

Ten dense objects under the Fly128 probe: N is raw network output, D is flat plus tilt polish, C is network plus tilt polish, and L is LSQ-ML at 200 sweeps. Neural cells average three seeds per object; intervals are 95% object-bootstrap confidence intervals (10,000 resamples).

| Arm | Phase MAE, mean [95% CI] | Median | Phase FRC50, mean [95% CI] | Amplitude MAE, mean [95% CI] | C wins | Vortex canvases |
|---|---:|---:|---:|---:|---:|---:|
| Network only | 0.3195 [0.2161, 0.4509] | 0.2624 | 0.1853 [0.1610, 0.2063] | 0.1371 [0.1237, 0.1460] | 10/10 | 21/30 |
| DPC only | 0.1098 [0.0407, 0.2017] | 0.0712 | 0.1530 [0.1450, 0.1660] | 0.0298 [0.0027, 0.0683] | 2/10 | 0/30 |
| Combined | 0.1866 [0.1553, 0.2374] | 0.1626 | 0.2027 [0.1810, 0.2253] | 0.1371 [0.1237, 0.1460] | — | 21/30 |
| LSQ-ML 200 | 0.0188 [0.0159, 0.0223] | 0.0169 | 0.2860 [0.2390, 0.3340] | 0.0157 [0.0152, 0.0164] | 0/10 | 0/10 |

## LSQ-ML phase MAE by sweep

| Sweeps | Mean [95% CI] |
|---:|---:|
| 10 | 0.0981 [0.0409, 0.1745] |
| 20 | 0.0502 [0.0247, 0.0819] |
| 50 | 0.0217 [0.0169, 0.0273] |
| 100 | 0.0190 [0.0161, 0.0225] |
| 200 | 0.0188 [0.0159, 0.0223] |
