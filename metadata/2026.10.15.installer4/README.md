Windows x64 single-file installer with incremental application and dependency updates.

下载 EXE 后，关闭旧启动中心及其网站服务，选择原安装目录和原来的 CPU/CUDA 配置运行安装。完整、版本匹配的软件包会显示已跳过；仅新增、变化或缺失的部分会安装或修复。

- Maintenance core is updated once when its version or files change. Unchanged dependency versions are detected locally, avoiding redundant package installation and package-index requests. Import and dependency checks remain in place for repair.
- Application updates compare installed files by role. Repeated installation skips intact parts, while changed or damaged package data and frontend files remain repairable. Legacy installation records are supported; missing proof of an intact component triggers installation instead of a false skip.
- Includes maintenance control core 0.2.9. The application remains post5 with its original scientific maintenance dependency 0.2.8; no application wheels, model weights or datasets are republished here.
- Uses the existing fixed resource-directory snapshot and matching local metadata to avoid unnecessary repeated directory requests. User source selections and local model/data files are retained.

The frozen artifact was checked with the recorded incremental-installation regressions and repeated installation runs. Download and double-click this one EXE; no extraction or adjacent config file is required. The supplied icon and single-file bootstrap are retained. This release does not replace post5 as the latest application release.
