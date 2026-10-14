# GrainBot Resources

Versioned datasets, model adapters and independent weights. Release downloads contain only resource files; update metadata is stored in versioned Git directories.

# GrainBot resource downloads

Download the dataset or model variant you need. Code, weights and runtime dependencies are installed separately.

## Datasets

| Dataset | Images | Download |
|---|---:|---|
| Prior-Guided SEM Material Phase | 82 | [Dataset ZIP](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/dataset-perovskite-phase-2026.10.14.resources1.zip) |
| Prior-Guided SEM Grain Boundaries | 82 | [Dataset ZIP](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/dataset-perovskite-boundary-2026.10.14.resources1.zip) |
| UO2 SEM-BSE Grain Boundaries | 37 | [Dataset ZIP](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/dataset-uo2-2026.10.14.resources1.zip) |
| Texture Boundary in Metallography | 320 | [Dataset ZIP](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/dataset-tbm-2026.10.14.resources1.zip) |

The two Prior-Guided SEM packages use the same 82 images with different annotation tasks. TBM remains excluded from training.

## Models

- [EMPS BPartIS Official Adapter](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/model-bpartis-2026.10.14.resources1.zip): small integration adapter; official code and approximately 9.2 MB original weights download separately.
- [UO2 DS checkpoint](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/uo2-ds-2026.10.14.resources1.pt) and [UO2 implementation](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/uo2-implementation-2026.10.14.resources1.zip): separate implementation and architecture-specific weights.

<details><summary>Other official UO2 checkpoint variants</summary>

- [B](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/uo2-b-2026.10.14.resources1.pt)
- [B_SyntExp](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/uo2-b-syntexp-2026.10.14.resources1.pt)
- [HED](https://github.com/kzhoujlu/GrainBot-resources/releases/download/2026.10.14.resources1/uo2-hed-2026.10.14.resources1.pt)

</details>

## Dataset inventory and installation

[Dataset overview](https://github.com/kzhoujlu/GrainBot-resources/blob/main/docs/datasets.md) lists source sets, training snapshots, weak labels, demonstration subsets and local collections.

The 316L eight-image subset is a demonstration set, not an independent test set: seven examples belong to the retained model's training split and one to its test split. Its local metadata has been corrected; image and label bytes are unchanged.

Release assets now contain only installable resource files. Metadata, checksums, signatures and installation documentation live in the repository and are read automatically by the updater.

Use GrainBot Maintenance 0.2.5 or newer for this layout. [Maintenance package](https://raw.githubusercontent.com/kzhoujlu/GrainBot-distribution/maintenance-0.2.5/maintenance/0.2.5/grainbot_maintenance-0.2.5-py3-none-any.whl) · [Installation instructions](https://github.com/kzhoujlu/GrainBot-resources/blob/main/docs/installation.md). Install this package into the native maintenance environment; scientific model effectiveness and structure retention remain subject to human review.

Developer metadata is under `metadata/2026.10.14.resources1/`. Each upstream item retains its own attribution and license; documentation does not grant new redistribution rights.
