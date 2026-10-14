# Installing resources

Use the Windows launcher's Version and updates panel with the repository URL https://github.com/kzhoujlu/GrainBot-resources. Select a resource and install only the files it needs. Metadata is fetched automatically from the repository; public downloads need no publishing token or private key.

## Maintenance compatibility

This repository-backed metadata layout requires GrainBot Maintenance 0.2.5 or newer. [Download the maintenance wheel](https://raw.githubusercontent.com/kzhoujlu/GrainBot-distribution/maintenance-0.2.5/maintenance/0.2.5/grainbot_maintenance-0.2.5-py3-none-any.whl). Install it into the native maintenance environment, separate from the scientific application environment:

```powershell
"<maintenance-python>" -m pip install --no-deps --force-reinstall "https://raw.githubusercontent.com/kzhoujlu/GrainBot-distribution/maintenance-0.2.5/maintenance/0.2.5/grainbot_maintenance-0.2.5-py3-none-any.whl"
```

The current local Windows launcher has been updated to this version. Existing model weights and data packages keep their release URLs and hashes. Configured signing keys still require valid signatures. Model-quality and structure-retention decisions remain with the user.
