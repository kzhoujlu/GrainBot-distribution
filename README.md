# GrainBot-distribution

## Windows 安装器

<!-- grainbot-incremental-installer4 -->
新版安装器支持增量安装：完整且版本匹配的软件包会跳过，仅更新变化或缺失的部分。应用仍为 post5。

[直接下载 Windows x64 安装器（单个 EXE）](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.15.installer4/GrainBot-Setup-Windows-x64-2026.10.15.installer4.exe)

下载后双击运行，无需解压或另配文件。首次使用建议选择 CPU。已有安装请选择原安装目录及原来的 CPU/CUDA 配置运行安装，按需更新维护工具和应用。[安装说明](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.15.installer4)。

新版补齐第三方模型和数据集目录，并合并历次已发布来源。界面明确区分已安装、可下载、待配置、尚未发布和待接入；目录登记数量不等于可直接运行的模型数量。

## 应用组件包

[GrainBot Studio 2026.10.14.post5](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.14.post5) 提供三个后端 wheel 和一个前端 ZIP。包含 Maintenance 0.2.8；此次为修复资源目录重新编译前端。

## 数据集与模型来源

- [resources1：既有数据集包、模型适配器和原始权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources1)
- [resources2：EMPS 和 ExONE 原始数据](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2)

安装器同时接入两次发布的已有组件，数据集按需下载。第三方官网来源和尚待适配的资源也显示在目录中；本次没有重新发布大型数据或模型文件。已发布的旧版文件保留不变。
