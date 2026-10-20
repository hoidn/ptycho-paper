# Synthetic versus scan-trained heldout scores

Heldout means the high-half spatial-validation acquisition. The scan-trained checkpoint was selected on that high half, so it is not an independent test. All rows use the saved common physical anchor, intersection mask, border, and source-frame IDs in the adjacent provenance manifests.

| Dataset | Arm | Deviance | Deviance floor | Phase FRC50 (cycles/px) |
|---|---|---:|---:|---:|
| Gold TP1 | synthetic-trained | 21.24 | 0.5151 | 0.155 |
| Gold TP1 | scan-trained | 20.83 | 0.528 | 0.155 |
| Gold TP1 | LSQ-ML100 | 12.36 | 0.6825 | 0.335 |
| Gold TP2 | synthetic-trained | 3.863 | 0.4071 | 0.135 |
| Gold TP2 | scan-trained | 3.629 | 0.4217 | 0.135 |
| Gold TP2 | LSQ-ML100 | 2.674 | 0.4917 | 0.225 |
| IC1 | synthetic-trained | 3.291 | 0.5487 | 0.235 |
| IC1 | scan-trained | 3.221 | 0.5506 | 0.185 |
| IC1 | LSQ-ML100 | 2.583 | 0.6017 | 0.285 |
| IC2 | synthetic-trained | 3.821 | 0.5355 | 0.175 |
| IC2 | scan-trained | 3.619 | 0.5412 | 0.245 |
| IC2 | LSQ-ML100 | 2.926 | 0.6112 | 0.275 |
| NCM1 | synthetic-trained | 7.636 | 0.4443 | 0.135 |
| NCM1 | scan-trained | 7.546 | 0.4505 | 0.125 |
| NCM1 | LSQ-ML100 | 6.593 | 0.5557 | 0.255 |
| Fly001 | synthetic-trained | 2.276 | 0.5188 | 0.205 |
| Fly001 | scan-trained | 2.211 | 0.5193 | 0.225 |
| Fly001 | LSQ-ML100 | 1.943 | 0.5494 | 0.285 |

Missing synthetic scores are omitted; the adjacent provenance JSON lists each omitted dataset and its reason.
