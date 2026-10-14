Approved software scope: S3, S4 and S5.

- S3: maintenance core 0.2.6 wheel, including image/model/dataset guidance. This is an independently installable Python core update; it does not replace or rebuild the compiled native Launcher UI.
- S4: frontend guidance update, repackaged from an existing compiled build. 前端复用既有构建产物，本轮未重新编译。 Source maps are not included.
- S5: installable post3 backend wheel built from the finalized source, including guidance, explicit primary annotation selection, EMPS semantic/instance label preservation and protection of its 99 held-out test samples, and ExONE source-label polarity and field grouping. Legacy dataset derivation provenance remains compatible.
- The byte-identical MatMorph post2 wheel is carried forward as an existing dependency so the four-role application updater can install this release. Its version, SHA256 and scientific methods are unchanged; no new model is included.

Backend dependencies are explicitly pinned to grainbot-maintenance==0.2.6 and matmorph[analysis]==2026.10.14.post2. The four assets form one application release. Application packages, frontend and maintenance core were installed and checked in isolated directories; dependencies came from the required existing scientific runtime libraries. Backend health, dataset APIs, frontend document/assets and all 801 new dataset samples were checked. This is packaging and integration validation, not scientific acceptance of a model or dataset.

Native Launcher and Setup EXEs are not uploaded. Updating this wheel does not update native UI binaries. Existing post2 assets remain unchanged.
