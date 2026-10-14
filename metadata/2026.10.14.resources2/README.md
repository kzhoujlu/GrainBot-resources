Approved scope: D1 and D3. This is a stable, explicitly pinned dataset release; it does not replace resources1 as the default latest source.

- D1 EMPS: 465 original images and uint16 instance maps, upstream commit dd8f86d714894fd08f3db80041893982ce058dd6; preserve 366 train / 99 held-out test. Separate binary semantic masks are derived as instance_id > 0. MIT notice and upstream metadata are included.
- D3 ExONE 316L: 336 original crops in 21 source fields × 16 crops, plus byte-preserved threshold JPEG references. Separate bright-positive PNG references use Otsu inversion without morphology. These are weak references, not expert ground truth; no training eligibility or human acceptance is inferred. CC0, Kaggle version 3. The source archive's HED model files are excluded.

Requires the post3 backend to preserve semantic targets, original labels, held-out tests and source-field groups. Use GrainBot Maintenance 0.2.6 with this exact release link. The public key remains MoVe3/7LcXOFzcMdlQgFMqRir4usKxT1FFn4hehhuxw=.
Only the two dataset ZIPs are Release downloads. Signed manifests, index and instructions live in Git at a pinned commit. Existing resources1 assets and its latest pointer remain unchanged. Validation checks packaging, hashes, dimensions and label derivations; scientific review remains pending.
