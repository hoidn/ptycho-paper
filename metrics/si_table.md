| dataset | case | model | canvas | frames (train/heldout/whole) | method | deviance | deviance_floor | phase_frc50 | throughput_fps | wall_clock_s | amp_mae | phase_wrapped_mae | amplitude_ssim | phase_ssim |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| ALS | diagnostic-whole | Hybrid ResNet C=1 | raw | 722/722/1444 | Hybrid raw ablation | n/a | n/a | 0.165 | 1075 | 1.344 | 0.02613 | 0.05579 | 0.8464 | 0.9703 |
| ALS | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 722/722/1444 | ours (C=1, after correction) | n/a | n/a | 0.165 | 905.5 | 1.595 | 0.02613 | 0.02699 | 0.8464 | 0.9856 |
| ALS | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 722/722/1444 | LSQ-ML100 | n/a | n/a | 0.345 | 91.13 | 15.85 | 0.01241 | 0.01002 | 0.943 | 0.9934 |
| ALS | heldout | Hybrid ResNet C=1 | raw | 722/722/1444 | Hybrid raw ablation | n/a | n/a | 0.115 | 871.1 | 0.8288 | 0.03436 | 0.06919 | 0.8304 | 0.9614 |
| ALS | heldout | Hybrid ResNet C=1 | polished_tilt | 722/722/1444 | ours (C=1, after correction) | n/a | n/a | 0.125 | 687.4 | 1.05 | 0.03436 | 0.03153 | 0.8304 | 0.9831 |
| ALS | heldout | Hybrid ResNet C=1 | lsqml100 | 722/722/1444 | LSQ-ML100 | n/a | n/a | 0.345 | 90.13 | 8.011 | 0.01179 | 0.01036 | 0.9536 | 0.9954 |
| CNM scan39 | diagnostic-whole | Hybrid ResNet C=1 | raw | 13041/12880/25921 | Hybrid raw ablation | 57.97 | 0.7226 | 0.145 | 1151 | 22.52 | 0.03177 | 0.1511 | 0.5591 | 0.9549 |
| CNM scan39 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 13041/12880/25921 | ours (C=1, after correction) | 51.96 | 0.7217 | 0.145 | 950.2 | 27.28 | 0.03177 | 0.06573 | 0.5591 | 0.9757 |
| CNM scan39 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 13041/12880/25921 | LSQ-ML100 | 50.04 | 0.7897 | 0.145 | 82.98 | 312.4 | 0.03462 | 0.06316 | 0.4716 | 0.9717 |
| CNM scan39 | heldout | Hybrid ResNet C=1 | raw | 13041/12880/25921 | Hybrid raw ablation | 61.72 | 0.726 | 0.145 | 1171 | 11 | 0.02762 | 0.1737 | 0.602 | 0.9561 |
| CNM scan39 | heldout | Hybrid ResNet C=1 | polished_tilt | 13041/12880/25921 | ours (C=1, after correction) | 54.92 | 0.7256 | 0.155 | 887.6 | 14.51 | 0.02762 | 0.06193 | 0.602 | 0.9808 |
| CNM scan39 | heldout | Hybrid ResNet C=1 | lsqml100 | 13041/12880/25921 | LSQ-ML100 | 52.86 | 0.7959 | 0.145 | 91.29 | 141.1 | 0.02848 | 0.05417 | 0.5348 | 0.9775 |
| Fly001 | diagnostic-whole | Hybrid ResNet C=1 | raw | 5180/5124/10304 | Hybrid raw ablation | 2.638 | 0.5104 | 0.235 | 1223 | 8.423 | 0.04731 | 0.107 | 0.3689 | 0.9525 |
| Fly001 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 5180/5124/10304 | ours (C=1, after correction) | 2.242 | 0.5165 | 0.225 | 1185 | 8.698 | 0.04731 | 0.05477 | 0.3689 | 0.9762 |
| Fly001 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 5180/5124/10304 | LSQ-ML100 | 1.986 | 0.5505 | 0.285 | 92.68 | 111.2 | 0.03272 | 0.04401 | 0.5531 | 0.9766 |
| Fly001 | heldout | Hybrid ResNet C=1 | raw | 5180/5124/10304 | Hybrid raw ablation | 2.65 | 0.5119 | 0.235 | 1226 | 4.18 | 0.05058 | 0.1143 | 0.3484 | 0.9429 |
| Fly001 | heldout | Hybrid ResNet C=1 | polished_tilt | 5180/5124/10304 | ours (C=1, after correction) | 2.211 | 0.5193 | 0.225 | 1152 | 4.447 | 0.05058 | 0.05783 | 0.3484 | 0.9732 |
| Fly001 | heldout | Hybrid ResNet C=1 | lsqml100 | 5180/5124/10304 | LSQ-ML100 | 1.943 | 0.5494 | 0.285 | 84.61 | 60.56 | 0.0355 | 0.04586 | 0.5452 | 0.9748 |
| Gold TP1 | diagnostic-whole | Hybrid ResNet C=1 | raw | 572/571/1143 | Hybrid raw ablation | 46.18 | 0.517 | 0.165 | 886.2 | 1.29 | 0.08404 | 0.2281 | 0.219 | 0.7971 |
| Gold TP1 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 572/571/1143 | ours (C=1, after correction) | 23.69 | 0.5446 | 0.155 | 731.9 | 1.562 | 0.08404 | 0.1098 | 0.219 | 0.9092 |
| Gold TP1 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 572/571/1143 | LSQ-ML100 | 11.58 | 0.7048 | 0.315 | 92.13 | 12.41 | 0.04068 | 0.07458 | 0.7676 | 0.9534 |
| Gold TP1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 572/571/1143 | Hybrid raw ablation | 27.26 | 0.5334 | 0.175 | n/a | n/a | 0.05626 | 0.1048 | 0.5208 | 0.9088 |
| Gold TP1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 572/571/1143 | ours (C=4, after correction) | 20.02 | 0.5524 | 0.165 | n/a | n/a | 0.05627 | 0.09218 | 0.521 | 0.927 |
| Gold TP1 | heldout | Hybrid ResNet C=1 | raw | 572/571/1143 | Hybrid raw ablation | 41.82 | 0.4995 | 0.135 | 917.1 | 0.6226 | 0.09169 | 0.2454 | 0.1894 | 0.7704 |
| Gold TP1 | heldout | Hybrid ResNet C=1 | polished_tilt | 572/571/1143 | ours (C=1, after correction) | 20.83 | 0.528 | 0.155 | 692.8 | 0.8242 | 0.09167 | 0.1224 | 0.1904 | 0.8949 |
| Gold TP1 | heldout | Hybrid ResNet C=1 | lsqml100 | 572/571/1143 | LSQ-ML100 | 12.36 | 0.6825 | 0.335 | 89.78 | 6.36 | 0.04929 | 0.08543 | 0.7161 | 0.9453 |
| Gold TP1 | heldout | Hybrid ResNet C=4 (group region) | raw | 572/571/1143 | Hybrid raw ablation | 26.45 | 0.518 | 0.175 | n/a | n/a | 0.06711 | 0.1324 | 0.449 | 0.8788 |
| Gold TP1 | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 572/571/1143 | ours (C=4, after correction) | 18.93 | 0.5368 | 0.185 | n/a | n/a | 0.06711 | 0.1063 | 0.449 | 0.9118 |
| microLFP double | diagnostic-whole | Hybrid ResNet C=1 | raw | 1900/1850/3750 | Hybrid raw ablation | n/a | n/a | 0.165 | 1077 | 3.483 | 0.009452 | 0.04382 | 0.9164 | 0.9904 |
| microLFP double | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 1900/1850/3750 | ours (C=1, after correction) | n/a | n/a | 0.165 | 850.8 | 4.408 | 0.009452 | 0.01221 | 0.9164 | 0.9966 |
| microLFP double | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 1900/1850/3750 | LSQ-ML100 | n/a | n/a | 0.205 | 89.53 | 41.88 | 0.005927 | 0.008595 | 0.9544 | 0.9968 |
| microLFP double | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 1900/1850/3750 | Hybrid raw ablation | n/a | n/a | 0.165 | n/a | n/a | 0.007752 | 0.02379 | 0.9399 | 0.9946 |
| microLFP double | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 1900/1850/3750 | ours (C=4, after correction) | n/a | n/a | 0.165 | n/a | n/a | 0.007752 | 0.01176 | 0.9399 | 0.9963 |
| microLFP double | heldout | Hybrid ResNet C=1 | raw | 1900/1850/3750 | Hybrid raw ablation | n/a | n/a | 0.175 | 1103 | 1.676 | 0.009239 | 0.03264 | 0.8698 | 0.9899 |
| microLFP double | heldout | Hybrid ResNet C=1 | polished_tilt | 1900/1850/3750 | ours (C=1, after correction) | n/a | n/a | 0.145 | 866.5 | 2.135 | 0.009239 | 0.01218 | 0.8698 | 0.9968 |
| microLFP double | heldout | Hybrid ResNet C=1 | lsqml100 | 1900/1850/3750 | LSQ-ML100 | n/a | n/a | 0.185 | 92.3 | 20.04 | 0.005569 | 0.007878 | 0.9254 | 0.9969 |
| microLFP double | heldout | Hybrid ResNet C=4 (group region) | raw | 1900/1850/3750 | Hybrid raw ablation | n/a | n/a | 0.145 | n/a | n/a | 0.008068 | 0.0199 | 0.8872 | 0.9936 |
| microLFP double | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 1900/1850/3750 | ours (C=4, after correction) | n/a | n/a | 0.155 | n/a | n/a | 0.008068 | 0.01128 | 0.8872 | 0.9963 |
| microLFP single | diagnostic-whole | Hybrid ResNet C=1 | raw | 2850/2775/5625 | Hybrid raw ablation | n/a | n/a | 0.235 | 1182 | 4.759 | 0.008333 | 0.04354 | 0.9473 | 0.9953 |
| microLFP single | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 2850/2775/5625 | ours (C=1, after correction) | n/a | n/a | 0.235 | 924.3 | 6.086 | 0.008334 | 0.01159 | 0.9473 | 0.9976 |
| microLFP single | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 2850/2775/5625 | LSQ-ML100 | n/a | n/a | 0.235 | 91.93 | 61.19 | 0.004793 | 0.007982 | 0.9647 | 0.9981 |
| microLFP single | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 2850/2775/5625 | Hybrid raw ablation | n/a | n/a | 0.205 | n/a | n/a | 0.00739 | 0.01949 | 0.9592 | 0.9971 |
| microLFP single | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 2850/2775/5625 | ours (C=4, after correction) | n/a | n/a | 0.205 | n/a | n/a | 0.00739 | 0.01332 | 0.9592 | 0.9975 |
| microLFP single | heldout | Hybrid ResNet C=1 | raw | 2850/2775/5625 | Hybrid raw ablation | n/a | n/a | 0.205 | 1065 | 2.606 | 0.007622 | 0.03619 | 0.917 | 0.9942 |
| microLFP single | heldout | Hybrid ResNet C=1 | polished_tilt | 2850/2775/5625 | ours (C=1, after correction) | n/a | n/a | 0.205 | 836.5 | 3.317 | 0.007623 | 0.01291 | 0.917 | 0.9975 |
| microLFP single | heldout | Hybrid ResNet C=1 | lsqml100 | 2850/2775/5625 | LSQ-ML100 | n/a | n/a | 0.205 | 89.66 | 30.95 | 0.004603 | 0.008535 | 0.9436 | 0.998 |
| microLFP single | heldout | Hybrid ResNet C=4 (group region) | raw | 2850/2775/5625 | Hybrid raw ablation | n/a | n/a | 0.195 | n/a | n/a | 0.007216 | 0.02346 | 0.9277 | 0.9959 |
| microLFP single | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 2850/2775/5625 | ours (C=4, after correction) | n/a | n/a | 0.205 | n/a | n/a | 0.007216 | 0.01392 | 0.9277 | 0.9975 |
| Gold TP2 | diagnostic-whole | Hybrid ResNet C=1 | raw | 3841/3868/7709 | Hybrid raw ablation | 4.981 | 0.4106 | 0.105 | 1250 | 6.166 | 0.04845 | 0.1534 | 0.5264 | 0.9243 |
| Gold TP2 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 3841/3868/7709 | ours (C=1, after correction) | 4.023 | 0.4216 | 0.125 | 961.4 | 8.018 | 0.04843 | 0.05631 | 0.5267 | 0.9464 |
| Gold TP2 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 3841/3868/7709 | LSQ-ML100 | 3.063 | 0.4947 | 0.225 | 87.33 | 88.27 | 0.03519 | 0.0641 | 0.7519 | 0.9641 |
| Gold TP2 | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 3841/3868/7709 | Hybrid raw ablation | 3.715 | 0.447 | 0.135 | n/a | n/a | 0.04328 | 0.06382 | 0.6175 | 0.9431 |
| Gold TP2 | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 3841/3868/7709 | ours (C=4, after correction) | 3.536 | 0.4513 | 0.135 | n/a | n/a | 0.04328 | 0.05392 | 0.6175 | 0.9465 |
| Gold TP2 | heldout | Hybrid ResNet C=1 | raw | 3841/3868/7709 | Hybrid raw ablation | 4.507 | 0.4106 | 0.125 | 1148 | 3.369 | 0.04718 | 0.1541 | 0.5417 | 0.9253 |
| Gold TP2 | heldout | Hybrid ResNet C=1 | polished_tilt | 3841/3868/7709 | ours (C=1, after correction) | 3.629 | 0.4217 | 0.135 | 917.2 | 4.217 | 0.04717 | 0.05216 | 0.5418 | 0.9487 |
| Gold TP2 | heldout | Hybrid ResNet C=1 | lsqml100 | 3841/3868/7709 | LSQ-ML100 | 2.674 | 0.4917 | 0.225 | 85.84 | 45.06 | 0.03243 | 0.06613 | 0.7751 | 0.9687 |
| Gold TP2 | heldout | Hybrid ResNet C=4 (group region) | raw | 3841/3868/7709 | Hybrid raw ablation | 3.356 | 0.4475 | 0.145 | n/a | n/a | 0.04196 | 0.05712 | 0.626 | 0.9446 |
| Gold TP2 | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 3841/3868/7709 | ours (C=4, after correction) | 3.203 | 0.452 | 0.145 | n/a | n/a | 0.04197 | 0.05156 | 0.626 | 0.9497 |
| IC1 | diagnostic-whole | Hybrid ResNet C=1 | raw | 579/564/1143 | Hybrid raw ablation | 4.433 | 0.5539 | 0.185 | 922.6 | 1.239 | 0.03613 | 0.1332 | 0.1891 | 0.9169 |
| IC1 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 579/564/1143 | ours (C=1, after correction) | 3.939 | 0.554 | 0.185 | 739.9 | 1.545 | 0.03612 | 0.05569 | 0.1895 | 0.9428 |
| IC1 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 579/564/1143 | LSQ-ML100 | 2.978 | 0.6226 | 0.265 | 93.13 | 12.27 | 0.02286 | 0.04272 | 0.6106 | 0.9666 |
| IC1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 579/564/1143 | Hybrid raw ablation | 3.784 | 0.5733 | 0.205 | n/a | n/a | 0.02891 | 0.08124 | 0.3413 | 0.9503 |
| IC1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 579/564/1143 | ours (C=4, after correction) | 3.579 | 0.5731 | 0.205 | n/a | n/a | 0.02891 | 0.04751 | 0.3414 | 0.956 |
| IC1 | heldout | Hybrid ResNet C=1 | raw | 579/564/1143 | Hybrid raw ablation | 3.678 | 0.5498 | 0.185 | 931 | 0.6058 | 0.03529 | 0.1542 | 0.2003 | 0.9175 |
| IC1 | heldout | Hybrid ResNet C=1 | polished_tilt | 579/564/1143 | ours (C=1, after correction) | 3.221 | 0.5506 | 0.185 | 707.8 | 0.7969 | 0.03529 | 0.05402 | 0.2003 | 0.942 |
| IC1 | heldout | Hybrid ResNet C=1 | lsqml100 | 579/564/1143 | LSQ-ML100 | 2.583 | 0.6017 | 0.285 | 87.22 | 6.466 | 0.02488 | 0.04182 | 0.548 | 0.9654 |
| IC1 | heldout | Hybrid ResNet C=4 (group region) | raw | 579/564/1143 | Hybrid raw ablation | 3.191 | 0.5653 | 0.205 | n/a | n/a | 0.03109 | 0.1034 | 0.2613 | 0.942 |
| IC1 | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 579/564/1143 | ours (C=4, after correction) | 2.989 | 0.5649 | 0.205 | n/a | n/a | 0.03109 | 0.04825 | 0.2614 | 0.9514 |
| IC2 | diagnostic-whole | Hybrid ResNet C=1 | raw | 4742/4694/9436 | Hybrid raw ablation | 3.798 | 0.5408 | 0.185 | 1248 | 7.559 | 0.03967 | 0.09511 | 0.278 | 0.9312 |
| IC2 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 4742/4694/9436 | ours (C=1, after correction) | 3.586 | 0.5411 | 0.185 | 1125 | 8.389 | 0.03967 | 0.05317 | 0.2781 | 0.9479 |
| IC2 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 4742/4694/9436 | LSQ-ML100 | 2.898 | 0.6174 | 0.245 | 91.29 | 103.4 | 0.03755 | 0.04686 | 0.4067 | 0.9517 |
| IC2 | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 4742/4694/9436 | Hybrid raw ablation | 3.293 | 0.5611 | 0.185 | n/a | n/a | 0.03599 | 0.05478 | 0.3403 | 0.9524 |
| IC2 | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 4742/4694/9436 | ours (C=4, after correction) | 3.261 | 0.561 | 0.185 | n/a | n/a | 0.03599 | 0.04643 | 0.3404 | 0.9544 |
| IC2 | heldout | Hybrid ResNet C=1 | raw | 4742/4694/9436 | Hybrid raw ablation | 3.837 | 0.5411 | 0.245 | 1122 | 4.183 | 0.04013 | 0.0991 | 0.2774 | 0.9276 |
| IC2 | heldout | Hybrid ResNet C=1 | polished_tilt | 4742/4694/9436 | ours (C=1, after correction) | 3.619 | 0.5412 | 0.245 | 968.4 | 4.847 | 0.04013 | 0.05399 | 0.2774 | 0.944 |
| IC2 | heldout | Hybrid ResNet C=1 | lsqml100 | 4742/4694/9436 | LSQ-ML100 | 2.926 | 0.6112 | 0.275 | 84.92 | 55.28 | 0.03754 | 0.04839 | 0.4107 | 0.9478 |
| IC2 | heldout | Hybrid ResNet C=4 (group region) | raw | 4742/4694/9436 | Hybrid raw ablation | 3.344 | 0.5612 | 0.245 | n/a | n/a | 0.03735 | 0.05893 | 0.3231 | 0.9463 |
| IC2 | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 4742/4694/9436 | ours (C=4, after correction) | 3.299 | 0.561 | 0.245 | n/a | n/a | 0.03735 | 0.04831 | 0.3231 | 0.9494 |
| NCM1 | diagnostic-whole | Hybrid ResNet C=1 | raw | 1207/1259/2466 | Hybrid raw ablation | 10.32 | 0.4388 | 0.005 | 1081 | 2.282 | 0.01839 | 0.7272 | 0.4173 | 0.8738 |
| NCM1 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 1207/1259/2466 | ours (C=1, after correction) | 6.656 | 0.4512 | 0.145 | 961.5 | 2.565 | 0.01839 | 0.09658 | 0.4172 | 0.9804 |
| NCM1 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 1207/1259/2466 | LSQ-ML100 | 5.537 | 0.5488 | 0.255 | 88.71 | 27.8 | 0.0168 | 0.06869 | 0.53 | 0.9856 |
| NCM1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | raw | 1207/1259/2466 | Hybrid raw ablation | 8.583 | 0.4592 | 0.085 | n/a | n/a | 0.01725 | 0.5258 | 0.455 | 0.9199 |
| NCM1 | diagnostic-whole | Hybrid ResNet C=4 (group region) | polished_tilt | 1207/1259/2466 | ours (C=4, after correction) | 6.356 | 0.466 | 0.155 | n/a | n/a | 0.01725 | 0.0796 | 0.455 | 0.9826 |
| NCM1 | heldout | Hybrid ResNet C=1 | raw | 1207/1259/2466 | Hybrid raw ablation | 15 | 0.4341 | 0.065 | 906.8 | 1.388 | 0.01944 | 0.5972 | 0.3655 | 0.8875 |
| NCM1 | heldout | Hybrid ResNet C=1 | polished_tilt | 1207/1259/2466 | ours (C=1, after correction) | 7.546 | 0.4505 | 0.125 | 747.3 | 1.685 | 0.01944 | 0.177 | 0.3655 | 0.9714 |
| NCM1 | heldout | Hybrid ResNet C=1 | lsqml100 | 1207/1259/2466 | LSQ-ML100 | 6.593 | 0.5557 | 0.255 | 70.24 | 17.92 | 0.01562 | 0.1795 | 0.5958 | 0.9786 |
| NCM1 | heldout | Hybrid ResNet C=4 (group region) | raw | 1207/1259/2466 | Hybrid raw ablation | 14.25 | 0.4398 | 0.065 | n/a | n/a | 0.01888 | 0.532 | 0.4078 | 0.9064 |
| NCM1 | heldout | Hybrid ResNet C=4 (group region) | polished_tilt | 1207/1259/2466 | ours (C=4, after correction) | 7.488 | 0.4545 | 0.185 | n/a | n/a | 0.01888 | 0.1704 | 0.4078 | 0.9736 |
| S200 | diagnostic-whole | Hybrid ResNet C=1 | raw | 8294/8319/16613 | Hybrid raw ablation | 5.397 | 0.2553 | 0.015 | 1220 | 13.62 | 0.03355 | 0.502 | 0.4147 | 0.8697 |
| S200 | diagnostic-whole | Hybrid ResNet C=1 | polished_tilt | 8294/8319/16613 | ours (C=1, after correction) | 4.665 | 0.2663 | 0.025 | 834.8 | 19.9 | 0.03355 | 0.6414 | 0.4147 | 0.8385 |
| S200 | diagnostic-whole | Hybrid ResNet C=1 | lsqml100 | 8294/8319/16613 | LSQ-ML100 | 6.817 | 0.2992 | 0 | 35.89 | 462.9 | 0.0475 | 0.885 | 0.2929 | 0.7609 |
| S200 | heldout | Hybrid ResNet C=1 | raw | 8294/8319/16613 | Hybrid raw ablation | 6.692 | 0.2624 | 0 | 1153 | 7.215 | 0.03687 | 0.6489 | 0.3085 | 0.7634 |
| S200 | heldout | Hybrid ResNet C=1 | polished_tilt | 8294/8319/16613 | ours (C=1, after correction) | 5.115 | 0.275 | 0.085 | 781.2 | 10.65 | 0.03687 | 0.783 | 0.3085 | 0.7869 |
| S200 | heldout | Hybrid ResNet C=1 | lsqml100 | 8294/8319/16613 | LSQ-ML100 | 8.854 | 0.306 | 0 | 34.81 | 239 | 0.05343 | 1.199 | 0.2824 | 0.6623 |
| Gold TP1 | heldout | CNN C=1 | unaligned | 572/571/1143 | CNN C=1, unaligned (no offset/tilt) | 45.05 | 0.4771 | 0.095 | n/a | n/a | 0.1176 | 0.3066 | 0.1348 | 0.6911 |
| Gold TP1 | diagnostic-whole | CNN C=1 | unaligned | 572/571/1143 | CNN C=1, unaligned (no offset/tilt) | 54.19 | 0.4756 | 0.095 | n/a | n/a | 0.1112 | 0.294 | 0.1435 | 0.7209 |
| Gold TP2 | heldout | CNN C=1 | unaligned | 3841/3868/7709 | CNN C=1, unaligned (no offset/tilt) | 4.046 | 0.3896 | 0.145 | n/a | n/a | 0.03909 | 0.06489 | 0.6485 | 0.9446 |
| Gold TP2 | diagnostic-whole | CNN C=1 | unaligned | 3841/3868/7709 | CNN C=1, unaligned (no offset/tilt) | 4.587 | 0.3903 | 0.125 | n/a | n/a | 0.04147 | 0.06707 | 0.6261 | 0.9419 |
| IC1 | heldout | CNN C=1 | unaligned | 579/564/1143 | CNN C=1, unaligned (no offset/tilt) | 3.735 | 0.5507 | 0.135 | n/a | n/a | 0.0318 | 0.1977 | 0.1634 | 0.8866 |
| IC1 | diagnostic-whole | CNN C=1 | unaligned | 579/564/1143 | CNN C=1, unaligned (no offset/tilt) | 4.512 | 0.5557 | 0.135 | n/a | n/a | 0.03144 | 0.1641 | 0.1771 | 0.8915 |
| IC2 | heldout | CNN C=1 | unaligned | 4742/4694/9436 | CNN C=1, unaligned (no offset/tilt) | 3.735 | 0.5437 | 0.175 | n/a | n/a | 0.03741 | 0.117 | 0.2819 | 0.9309 |
| IC2 | diagnostic-whole | CNN C=1 | unaligned | 4742/4694/9436 | CNN C=1, unaligned (no offset/tilt) | 3.676 | 0.5438 | 0.185 | n/a | n/a | 0.03667 | 0.1119 | 0.2893 | 0.9369 |
| NCM1 | heldout | CNN C=1 | unaligned | 1207/1259/2466 | CNN C=1, unaligned (no offset/tilt) | 13.79 | 0.4348 | 0.145 | n/a | n/a | 0.01841 | 0.5388 | 0.3838 | 0.8907 |
| NCM1 | diagnostic-whole | CNN C=1 | unaligned | 1207/1259/2466 | CNN C=1, unaligned (no offset/tilt) | 10.13 | 0.4372 | 0.015 | n/a | n/a | 0.01811 | 0.6817 | 0.4251 | 0.8771 |
| CNM scan39 | heldout | CNN C=1 | unaligned | 13041/12880/25921 | CNN C=1, unaligned (no offset/tilt) | 126.2 | 0.6788 | 0 | n/a | n/a | 0.06751 | 0.5193 | 0.2761 | 0.5796 |
| CNM scan39 | diagnostic-whole | CNN C=1 | unaligned | 13041/12880/25921 | CNN C=1, unaligned (no offset/tilt) | 125.8 | 0.6773 | 0 | n/a | n/a | 0.06735 | 0.5161 | 0.2831 | 0.5784 |
| Fly001 | heldout | CNN C=1 | unaligned | 5180/5124/10304 | CNN C=1, unaligned (no offset/tilt) | 2.953 | 0.51 | 0.175 | n/a | n/a | 0.04165 | 0.1092 | 0.4684 | 0.925 |
| Fly001 | diagnostic-whole | CNN C=1 | unaligned | 5180/5124/10304 | CNN C=1, unaligned (no offset/tilt) | 2.72 | 0.5102 | 0.185 | n/a | n/a | 0.03867 | 0.09003 | 0.5012 | 0.9481 |
| ALS | heldout | CNN C=1 | unaligned | 722/722/1444 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.255 | n/a | n/a | 0.02977 | 0.05485 | 0.8564 | 0.9558 |
| ALS | diagnostic-whole | CNN C=1 | unaligned | 722/722/1444 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.255 | n/a | n/a | 0.02551 | 0.04586 | 0.8552 | 0.9628 |
| microLFP single | heldout | CNN C=1 | unaligned | 2850/2775/5625 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.145 | n/a | n/a | 0.007857 | 0.05959 | 0.9219 | 0.9884 |
| microLFP single | diagnostic-whole | CNN C=1 | unaligned | 2850/2775/5625 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.165 | n/a | n/a | 0.008838 | 0.05344 | 0.9479 | 0.9926 |
| microLFP double | heldout | CNN C=1 | unaligned | 1900/1850/3750 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.125 | n/a | n/a | 0.00861 | 0.02134 | 0.8788 | 0.9937 |
| microLFP double | diagnostic-whole | CNN C=1 | unaligned | 1900/1850/3750 | CNN C=1, unaligned (no offset/tilt) | n/a | n/a | 0.115 | n/a | n/a | 0.008688 | 0.02118 | 0.9191 | 0.993 |
| S200 | heldout | CNN C=1 | unaligned | 8294/8319/16613 | CNN C=1, unaligned (no offset/tilt) | 13.75 | 0.2407 | 0 | n/a | n/a | 0.04672 | 1.145 | 0.2877 | 0.6711 |
| S200 | diagnostic-whole | CNN C=1 | unaligned | 8294/8319/16613 | CNN C=1, unaligned (no offset/tilt) | 10.21 | 0.242 | 0 | n/a | n/a | 0.04373 | 0.9063 | 0.3947 | 0.7731 |

The low half trains; the high half selects checkpoints and supplies spatial-validation scores, not an independent test. No guard band. Whole-acquisition scores include the training region. Reference: supplied experimental estimate. All object scores share the declared interior and global gauge; diffraction is scored on native objects. Timings are inference-only, host-to-host medians on an idle GPU. Training is excluded.
