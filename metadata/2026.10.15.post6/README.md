Install and update existing resources directly from GrainBot Studio and the Windows launch center.

- Unified installation handles the existing GrainBot baseline, SAM ViT-B, SAM2, Cellpose and UO2 DS backends. It downloads the selected weights, checks runtime dependencies, registers their paths and refreshes model availability. New UO2 variants and other development candidates are not enabled.
- GrainBot's original 50 training pairs and the six previously published dataset components have integrated installation. Material-phase and grain-boundary targets from the perovskite source remain separate. Newly enabled data is visible without restarting; repeat installation retains user review records.
- Model installation shows progress, errors and retry controls. Resource references are not presented as runnable models merely because a source link exists.
- Existing inference and postprocessing are retained, with the local compatibility changes needed by the selected dependency versions. No retraining or new scientific accuracy claim is part of this release.
- The frontend was rebuilt from the finalized source for this release. 本轮已重新编译前端；此前版本复用既有构建产物的说明仅适用于此前版本。

Three Python wheels and one frontend ZIP form this application release. MatMorph post2 is reused byte-for-byte. The maintenance version is pinned by the backend wheel. Use the separately published installer5 once to add launch-center self-updates to older installers; subsequent updates can be started in the launch center.

Validation includes isolated wheel installation, authenticated model/dataset APIs, frontend document/assets, focused installation/activation tests and repeated native installation checks. GrainBot, SAM ViT-B and UO2 DS were loaded using existing real weights. Full remote SAM2 and Cellpose checkpoints were not downloaded again during this release; their complete end-to-end validation remains pending.
