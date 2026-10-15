SEM pore ASPP (instance-balanced)

Publishes exactly the existing sem-pore-aspp-instance-balanced-v1 model for SEM pore identification. It was selected for the existing SEM16 training domain and instance-balanced small-pore training. No training or postprocessing changes are included.

One ZIP supplies the original TorchScript model, model metadata, provenance and report; the duplicate training checkpoint is omitted. Studio post8 / maintenance 0.2.12 / installer7 provide automatic installation using the existing TrainedMaterialBackend and backend ID trained:sem-pore-aspp-instance-balanced-v1. This archive is not a ComponentBackend component.

Validation: actual CPU installation and trained-backend discovery; probability arrays on all 16 existing SEM images are bit-for-bit equal to the original model. Repeated installation skips downloading and loading intact files. 31 focused installer/catalog/web-download tests passed. These checks establish packaging and behavior preservation; the existing training images are not an independent accuracy test and no scientific acceptance is asserted.

Archive and member hashes are recorded in versioned repository metadata. Historical resources and software releases are preserved.
