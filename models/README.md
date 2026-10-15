# Model update directory

`latest.json` and `latest.sig` are a paired, signed directory for Studio post11 and later. Each model has an independent version. Model ownership is separate from architecture, training-data references and installation state.

Publish immutable model assets first, then update this directory. The application pins the checked versions before starting a selected batch. New archives may reuse an existing backend/storage contract; changed inference contracts require an application update. Local models without published sources remain untouched. No weights are replaced under existing release tags.
