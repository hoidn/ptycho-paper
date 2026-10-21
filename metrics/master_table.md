| dataset | case | model | canvas | frames (train/heldout/whole) | method | deviance | deviance_floor | phase_frc50 | throughput_fps | wall_clock_s | timing_basis |
|---|---|---|---|---|---|---|---|---|---|---|---|
| ALS | heldout | Hybrid ResNet C=1 | raw | 722/722/1444 | Hybrid raw ablation | n/a | n/a | 0.115 | 1078 | 0.6698 | c1-inference-stitch-offset-tilt-v1 |
| ALS | heldout | Hybrid ResNet C=1 | polished_tilt | 722/722/1444 | ours (C=1, after correction) | n/a | n/a | 0.125 | 869.6 | 0.8303 | c1-inference-stitch-offset-tilt-v1 |
| ALS | heldout | Hybrid ResNet C=1 | lsqml100 | 722/722/1444 | LSQ-ML100 | n/a | n/a | 0.345 | 90.13 | 8.011 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| CNM scan39 | heldout | Hybrid ResNet C=1 | raw | 13041/12880/25921 | Hybrid raw ablation | 61.72 | 0.726 | 0.145 | 1412 | 9.122 | c1-inference-stitch-offset-tilt-v1 |
| CNM scan39 | heldout | Hybrid ResNet C=1 | polished_tilt | 13041/12880/25921 | ours (C=1, after correction) | 54.92 | 0.7256 | 0.155 | 1058 | 12.18 | c1-inference-stitch-offset-tilt-v1 |
| CNM scan39 | heldout | Hybrid ResNet C=1 | lsqml100 | 13041/12880/25921 | LSQ-ML100 | 52.86 | 0.7959 | 0.145 | 91.29 | 141.1 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| Fly001 | heldout | Hybrid ResNet C=1 | raw | 5180/5124/10304 | Hybrid raw ablation | 2.65 | 0.5119 | 0.235 | 1488 | 3.443 | c1-inference-stitch-offset-tilt-v1 |
| Fly001 | heldout | Hybrid ResNet C=1 | polished_tilt | 5180/5124/10304 | ours (C=1, after correction) | 2.211 | 0.5193 | 0.225 | 1394 | 3.676 | c1-inference-stitch-offset-tilt-v1 |
| Fly001 | heldout | Hybrid ResNet C=1 | lsqml100 | 5180/5124/10304 | LSQ-ML100 | 1.943 | 0.5494 | 0.285 | 84.61 | 60.56 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| microLFP double | heldout | Hybrid ResNet C=1 | raw | 1900/1850/3750 | Hybrid raw ablation | n/a | n/a | 0.175 | 1345 | 1.376 | c1-inference-stitch-offset-tilt-v1 |
| microLFP double | heldout | Hybrid ResNet C=1 | polished_tilt | 1900/1850/3750 | ours (C=1, after correction) | n/a | n/a | 0.145 | 1049 | 1.764 | c1-inference-stitch-offset-tilt-v1 |
| microLFP double | heldout | Hybrid ResNet C=1 | lsqml100 | 1900/1850/3750 | LSQ-ML100 | n/a | n/a | 0.185 | 92.3 | 20.04 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| microLFP single | heldout | Hybrid ResNet C=1 | raw | 2850/2775/5625 | Hybrid raw ablation | n/a | n/a | 0.205 | 1277 | 2.173 | c1-inference-stitch-offset-tilt-v1 |
| microLFP single | heldout | Hybrid ResNet C=1 | polished_tilt | 2850/2775/5625 | ours (C=1, after correction) | n/a | n/a | 0.205 | 1001 | 2.773 | c1-inference-stitch-offset-tilt-v1 |
| microLFP single | heldout | Hybrid ResNet C=1 | lsqml100 | 2850/2775/5625 | LSQ-ML100 | n/a | n/a | 0.205 | 89.66 | 30.95 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| IC2 | heldout | Hybrid ResNet C=1 | raw | 4742/4694/9436 | Hybrid raw ablation | 3.837 | 0.5411 | 0.245 | 1463 | 3.208 | c1-inference-stitch-offset-tilt-v1 |
| IC2 | heldout | Hybrid ResNet C=1 | polished_tilt | 4742/4694/9436 | ours (C=1, after correction) | 3.619 | 0.5412 | 0.245 | 1262 | 3.721 | c1-inference-stitch-offset-tilt-v1 |
| IC2 | heldout | Hybrid ResNet C=1 | lsqml100 | 4742/4694/9436 | LSQ-ML100 | 2.926 | 0.6112 | 0.275 | 84.92 | 55.28 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| NCM1 | heldout | Hybrid ResNet C=1 | raw | 1207/1259/2466 | Hybrid raw ablation | 15 | 0.4341 | 0.065 | 1269 | 0.9923 | c1-inference-stitch-offset-tilt-v1 |
| NCM1 | heldout | Hybrid ResNet C=1 | polished_tilt | 1207/1259/2466 | ours (C=1, after correction) | 7.546 | 0.4505 | 0.125 | 1035 | 1.216 | c1-inference-stitch-offset-tilt-v1 |
| NCM1 | heldout | Hybrid ResNet C=1 | lsqml100 | 1207/1259/2466 | LSQ-ML100 | 6.593 | 0.5557 | 0.255 | 70.24 | 17.92 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| S200 | heldout | Hybrid ResNet C=1 | raw | 8294/8319/16613 | Hybrid raw ablation | 6.692 | 0.2624 | 0 | 1358 | 6.125 | c1-inference-stitch-offset-tilt-v1 |
| S200 | heldout | Hybrid ResNet C=1 | polished_tilt | 8294/8319/16613 | ours (C=1, after correction) | 5.115 | 0.275 | 0.085 | 857.6 | 9.701 | c1-inference-stitch-offset-tilt-v1 |
| S200 | heldout | Hybrid ResNet C=1 | lsqml100 | 8294/8319/16613 | LSQ-ML100 | 8.854 | 0.306 | 0 | 34.81 | 239 | historical host-to-host; includes preparation, transfers, gauge and scoring boundary as originally recorded |
| IC2 | heldout | CNN C=1 | unaligned | 4742/4694/9436 | CNN C=1, unaligned (no offset/tilt) | 3.735 | 0.5437 | 0.175 | n/a | n/a | n/a |
| NCM1 | heldout | CNN C=1 | unaligned | 1207/1259/2466 | CNN C=1, unaligned (no offset/tilt) | 13.79 | 0.4348 | 0.145 | n/a | n/a | n/a |
| CNM scan39 | heldout | CNN C=1 | unaligned | 13041/12880/25921 | CNN C=1, unaligned (no offset/tilt) | 126.2 | 0.6788 | 0 | n/a | n/a | n/a |
| Fly001 | heldout | CNN C=1 | unaligned | 5180/5124/10304 | CNN C=1, unaligned (no offset/tilt) | 2.953 | 0.51 | 0.175 | n/a | n/a | n/a |
| ALS | heldout | CNN C=1 | unaligned | 722/722/1444 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.255 | n/a | n/a | n/a |
| microLFP single | heldout | CNN C=1 | unaligned | 2850/2775/5625 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.145 | n/a | n/a | n/a |
| microLFP double | heldout | CNN C=1 | unaligned | 1900/1850/3750 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.125 | n/a | n/a | n/a |
| S200 | heldout | CNN C=1 | unaligned | 8294/8319/16613 | CNN C=1, unaligned (no offset/tilt) | 13.75 | 0.2407 | 0 | n/a | n/a | n/a |

The low half trains; the high half selects checkpoints and supplies spatial-validation scores, not an independent test. No guard band. Whole-acquisition scores include the training region. Reference: supplied experimental estimate. All object scores share the declared interior and global gauge; diffraction is scored on native objects. C1 neural timing includes inference, stitching and offset/tilt correction only. LSQ-ML100 retains its historical host-to-host boundary; these are not matched speedup measurements. Times are medians on an idle GPU. C4 and CNN timing are unavailable.
