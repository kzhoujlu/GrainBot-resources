Three existing recommended models: TEM, perovskite phases and metallography.

- Patrick BF-TEM U-Net Official: bright-field TEM grain boundaries in nanocrystalline aluminum films, using the original HDF5 weights and existing checked adapter.
- Perovskite YOLOv8x instances: perovskite, PbI2 and defect region classification and instance masks for matching SEM images.
- 316L RG DeepLabV3+: the existing distilled single-pass boundary model for real 316L optical metallography.

Each model has its own ZIP, containing unchanged original weights and necessary model metadata. Install with Studio post9 / maintenance 0.2.13 / installer8. The existing backends and scientific inference/postprocessing remain unchanged; only installation and model-root discovery are connected. No retraining is included.

Powder keeps the previously published EMPS BPartIS model; it is not repackaged. The SEM pore model and single SEM Pores dataset remain available from resources5/resources4.

Validation: actual CPU installations, registered backend discovery and three representative images per model producing exactly the same outputs as their original local artifacts; repeated installation skips intact files. Thirty-five focused catalog/installer/web-download tests and an independent final application install passed. These checks validate packaging and behavior preservation, not new independent scientific accuracy or suitability for other materials.

These ZIPs are ordinary pinned model archives for the existing backend installers, not ComponentBackend components. Archive/member hashes and instructions are recorded in versioned repository metadata. Historical releases remain unchanged.
