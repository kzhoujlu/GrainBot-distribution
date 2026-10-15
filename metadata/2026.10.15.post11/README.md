Web model-library category checks and selected batch updates.

- The 检查更新 button checks every model in the current task category, independent of text search. Select models and update them in one batch with per-model progress and failure results.
- Independent signed model-version metadata lets future published model updates be detected without rebuilding the application. Single failures continue the batch; interrupted replacement restores the prior working model.
- Correctly identifies locally developed models as 自研. Perovskite YOLOv8x and 316L RG DeepLabV3+ are self-developed models; published weights and training dataset references are displayed separately.
- Includes maintenance 0.2.15 and installer10 source-label fixes. Frontend rebuilt for this release. MatMorph post2 is reused byte-for-byte.

No new model weights or training changes. Existing datasets, analysis selections and scientific parameters are preserved. 前端已重新编译。
