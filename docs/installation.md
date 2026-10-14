## Current dataset compatibility update

For the existing signed resources1 datasets, use GrainBot Maintenance 0.2.7 or newer and the [post4 application](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.14.post4). Legacy SPDX and attribution fields are read without changing signed resource bytes or license conditions. [Download maintenance core 0.2.7](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.14.post4/grainbot_maintenance-0.2.7-py3-none-any.whl). Install the core wheel in the native maintenance Python environment separately from scientific application wheels. This wheel does not replace the compiled native Launcher UI; no Launcher or Setup EXE is part of this publication.

The new EMPS and ExONE datasets use the explicit [resources2 release](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2). The default resource latest remains resources1, whose ten assets are unchanged.

# Installing resources

Use the Windows launcher's Version and updates panel with the repository URL https://github.com/kzhoujlu/GrainBot-resources. Select a resource and install only the files it needs. Metadata is fetched automatically from the repository; public downloads need no publishing token or private key.

## Maintenance compatibility

This repository-backed metadata layout requires GrainBot Maintenance 0.2.5 or newer. [Download the maintenance wheel](https://raw.githubusercontent.com/kzhoujlu/GrainBot-distribution/maintenance-0.2.5/maintenance/0.2.5/grainbot_maintenance-0.2.5-py3-none-any.whl). Install it into the native maintenance environment, separate from the scientific application environment:

```powershell
"<maintenance-python>" -m pip install --no-deps --force-reinstall "https://raw.githubusercontent.com/kzhoujlu/GrainBot-distribution/maintenance-0.2.5/maintenance/0.2.5/grainbot_maintenance-0.2.5-py3-none-any.whl"
```

The current local Windows launcher has been updated to this version. Existing model weights and data packages keep their release URLs and hashes. Configured signing keys still require valid signatures. Model-quality and structure-retention decisions remain with the user.
