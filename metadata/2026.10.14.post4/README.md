This patch completes approved S3/S5 compatibility with existing signed resources1 dataset packages, while carrying forward the approved S4 frontend.

- Maintenance core 0.2.7 and the post4 backend read the legacy license vocabulary in memory. Original SPDX identity and attribution requirements remain in notes; signed source bytes, original archives, signatures, image/label bytes and scientific review decisions are unchanged. Unknown fields still reach strict validation.
- Existing Perovskite phase/boundary tasks and provenance-only parent IDs remain readable; the existing TBM training prohibition is preserved.
- Includes the post3 guidance and data contract fixes: EMPS semantic targets plus original uint16 instances and 99 held-out tests, and ExONE source-label polarity and source-field grouping. ExONE threshold references remain weak labels with review pending.
- The frontend ZIP reuses exactly the same existing compiled bytes as post3. 前端复用既有构建产物，本轮未重新编译。 MatMorph post2 is reused byte-for-byte as an existing dependency; no new model, dataset or scientific algorithm is introduced by this patch.

Backend dependencies pin grainbot-maintenance==0.2.7 and matmorph[analysis]==2026.10.14.post2. The maintenance core can be installed independently in the native control environment. Wheels do not replace compiled native Launcher UI. Native Launcher/Setup EXEs are not uploaded.

The final wheels were installed in isolated directories with dependency checks and verified imports. New and legacy dataset schema/mapping compatibility, held-out test protection, weak-label training policy and source groups were checked. Health, authenticated APIs, frontend document and assets passed. Technical validation does not constitute scientific acceptance.

Use this release instead of post3 for legacy resources1 compatibility. New D1/D3 data remain at https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2 . The resource repository's default latest remains resources1. Existing post2/post3 and resource assets are preserved.
