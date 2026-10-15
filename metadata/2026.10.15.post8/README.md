Adds one-click installation for the existing SEM pore ASPP (instance-balanced) model.

- The web model catalog and native launch center install sem-pore-aspp-instance-balanced-v1 from one pinned resources5 archive.
- Uses the existing trained:sem-pore-aspp-instance-balanced-v1 backend and pore workflow. Correctly resolves the trained-model download alias, installed receipt and readiness state.
- Preserves the existing pore pipeline, thresholds, weights and postprocessing. No new training is included.
- Includes maintenance 0.2.12. The single GrainBot-V2 SEM Pores dataset and the previous layout/file-replacement fixes remain available.

Three Python wheels and one frontend ZIP form the application. The frontend reuses the post7 build byte-for-byte and was not recompiled for this release. MatMorph post2 is also reused unchanged. 本轮复用 post7 前端构建产物，未重新编译。

Validation: final application independently installed, health/frontend/catalog APIs checked, all 16 dataset image/label previews and web-open requests passed. The model was installed on CPU and produced exactly the original probabilities on the existing 16-image training snapshot; 31 focused catalog/installer/web-download tests passed. This is packaging and behavior validation, not independent scientific accuracy acceptance.
