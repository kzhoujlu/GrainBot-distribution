GrainBot-V2 SEM Pores is now one installable, web-viewable dataset.

- Adds the single combined 16-image pore dataset to the web and native catalog. Type 1 and Type 2 remain source metadata rather than separate visible datasets. The original combined dataset ID is preserved for saved work.
- Collapses known duplicate source/combined entries in presentation while preserving existing review records, historical IDs and user collections. The dataset name is GrainBot-V2 SEM Pores throughout the visible library.
- Reads the primary pore semantic target and auxiliary grain-boundary target explicitly. Original pixels and the existing training snapshot are retained; no model training or postprocessing changes are included.
- The dataset was previously local-only and absent from the published catalog. Its legacy manifest also needed conversion to the current schema before it could be installed as a signed data component. The new resources4 package supplies the portable data and complete manifest.
- Includes maintenance 0.2.11. Installer6 additionally fixes installation completion when the old launcher executable remains open, by deferring only entry-point replacement until that process exits.

Three Python wheels and one frontend ZIP form the application. MatMorph post2 is reused byte-for-byte. The frontend is rebuilt for the dataset thumbnail/detail layout correction. 本轮为数据集缩略图与详情布局修复重新编译前端。

Validation: signed installation, all 16 image/label previews and web-open requests, auxiliary target links, foreground equality, legacy-ID access and duplicate presentation. The final four-role application is independently installed and checked before publication. Existing model behavior and prior releases remain unchanged.
