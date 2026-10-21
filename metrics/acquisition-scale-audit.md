# Acquisition scale-bar calibration audit

All eleven delivered acquisitions lack a verified object-plane pixel size. The figures retain pixel units. No nominal literature value has been substituted for acquisition-specific metadata.

| Dataset | Object sampling (nm/px) | Delivered source |
|---|---|---|
| ALS | unavailable | `als_128_train.npz` |
| CNM scan39 | unavailable | `cnm_xnp_scan39_128_train.npz` |
| Fly001 | unavailable | `fly001_128_train.npz` |
| Gold TP1 | unavailable | `nxs_data_gold_tp_1_128_train.npz` |
| microLFP double | unavailable | `microLFPstack_double_exposure_128_train.npz` |
| microLFP single | unavailable | `microLFPstack_single_exposure_128_train.npz` |
| Gold TP2 | unavailable | `nxs_data_gold_tp_2_128_train.npz` |
| IC1 | unavailable | `nxs_data_ic_1_128_train.npz` |
| IC2 | unavailable | `nxs_data_ic_2_128_train.npz` |
| NCM1 | unavailable | `nxs_data_ncm_1_128_train.npz` |
| S200 | unavailable | `2id_S200_multiprobe_128.npz` |

The machine-readable [audit](acquisition-scale-audit.json) records source chains and NPZ member keys, shapes and dtypes. Canonical scan conversion changes intensity scale and coordinate origin, not object sampling; the earlier transformation into the delivered pixel-standardized N128 arrays is undocumented.

To replace a bar of L pixels by a physical length requires the verified object-plane nm/px for that N128 acquisition, or original detector/energy/distance metadata together with its exact binning, cropping and resampling history. Original detector pitch alone is insufficient.

The existing source audit `PtychoPINN/.artifacts/paper-figures-2026-10-19/design/table-datasets.md` lists the missing acquisition fields and source contacts. No messages were sent to collaborators.
