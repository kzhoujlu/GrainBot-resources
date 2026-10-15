Original GrainBot UNet baseline checkpoint for automatic installation in Studio and the Windows launch center.

This release contains only the existing 128 MB GrainBot baseline weight, preserved byte-for-byte. It does not add a new network, train a model or change inference/postprocessing. Studio post6 and installer5 download it automatically into the model directory and check that it can load in the selected scientific environment.

The original 50 GrainBot training image/annotation pairs are installed directly from the pinned original GrainBot-V2 repository, retaining the source files and historical 256 x 256 training preprocessing. They are training data, not an independent test set. No extra third-party candidates or new datasets are mirrored by this release.

Existing resources1/resources2 remain available and unchanged. This release does not replace their default latest pointer.
