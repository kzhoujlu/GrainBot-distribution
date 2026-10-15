# GrainBot-distribution

## Windows 安装与更新

[下载 Windows x64 安装器（单个 EXE）](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.15.installer5/GrainBot-Setup-Windows-x64-2026.10.15.installer5.exe)

首次使用双击运行，建议选择 CPU。已有安装请关闭旧启动中心和网站服务，运行新版并选择原安装目录及原 CPU/CUDA 配置；无需删除已有模型、数据或重新安装未变化的依赖。

旧 installer4 首次需要手动升级到本版一次。此后在启动中心进入“版本与更新”，即可检查并安装应用更新及启动中心更新，无需每次访问 GitHub 手动下载。更新会跳过完整且未变化的部分。

[installer5 发布说明](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.15.installer5)

## 应用软件包

[GrainBot Studio 2026.10.15.post6](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.15.post6) 提供三个 Python wheel 和一个前端 ZIP，维护核心为 0.2.10。前端本轮已重新编译，MatMorph post2 原包保持不变。

本版接通 GrainBot 默认模型、原始 50 对晶界训练数据及既有第三方资源的一键安装、路径登记和自动识别，支持安装进度、错误和重试。不重新训练或调整既有后处理。SAM2、Cellpose 完整远程权重的端到端验收尚未完成。

## 数据集与模型资源

- [resources3：GrainBot 原始默认权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources3)
- [resources1：既有数据集、模型适配包及 UO2 权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources1)
- [resources2：EMPS 与 ExONE 原始数据](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2)

GrainBot 自有的 50 对数据从固定版本的原作者仓库直接安装，保留原始图像与标注；这些是训练数据，不是独立测试集。六个已发布数据组件按需安装。仅提供来源信息、尚未集成的资源会明确标注。已有历史 Release 文件保持不变。
