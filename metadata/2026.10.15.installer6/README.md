GrainBot Windows launch center with reliable entry-point replacement and the SEM pore dataset.

首次从旧版升级：关闭旧启动中心及网站服务，下载并运行这一个 EXE，选择原安装目录和原 CPU/CUDA 配置。旧 installer4 没有自更新入口，因此首次需要下载新版一次。之后在启动中心的“版本与更新”中检查并更新，无需每次手动访问 GitHub。

- The launch center checks, downloads and verifies its own update, exits safely, replaces its executable in the original directory and restarts. Its maintenance core is updated separately from the scientific environment.
- Application updates reuse the existing check/download/install pipeline with a direct action. Intact, unchanged dependencies and application packages are skipped. Existing user model/data directories and settings are retained.
- Installs Studio post7 with the integrated original GrainBot baseline and its 50 training pairs; the existing third-party resources remain optional installs. No new model variants, retraining or postprocessing changes are introduced.
- If an old launcher remains open, the verified new entry point is staged and replaced after that process exits, without repeating dependency, application or data installation.
- Adds the single GrainBot-V2 SEM Pores dataset source.
- Single EXE, supplied icon and high-DPI layout are retained. This installer is published separately so the application's four-role release remains the latest application source.

The frozen native artifact was checked locally before publication. This is installation/update validation; full remote SAM2 and Cellpose model downloads were not repeated.

<!-- grainbot-launcher-update {"schema_version":1,"version":"0.2.11.0","asset":"GrainBot-Setup-Windows-x64-2026.10.15.installer6.exe"} -->
