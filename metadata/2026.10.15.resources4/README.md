GrainBot-V2 SEM Pores: one combined 16-image dataset, retaining Type 1 and Type 2 as per-sample source metadata.

原 GrainBot-V2 SEM Pores · Type 1 + Type 2 统一简称为 GrainBot-V2 SEM Pores。仅发布这一份合并集，Type 1 / Type 2 不另列安装包。

Original RGB training images, original 0/255 pore masks and auxiliary grain-boundary targets are preserved byte-for-byte. A separate semantic 0/1 encoding preserves exactly the same pore foreground for the current manifest schema. No pore masks or boundaries were recomputed, and no model was trained.

The pore annotations are existing threshold/geometry-derived weak labels, not human pore ground truth. Existing training eligibility is retained; all 16 images belong to the existing training snapshot and do not constitute an independent test set. Source type, sample identity and auxiliary target linkage are recorded.

The signed dataset was installed and checked through the real dataset reader. All 16 image previews, 16 label previews and 16 web-open requests passed. Existing dataset IDs remain compatible. Studio post7 and maintenance 0.2.11 add the catalog entry, single-dataset presentation and auxiliary-target reading. Use installer6 or the launch-center update actions to obtain the matching software.

Existing releases and other model/data payloads remain unchanged.
