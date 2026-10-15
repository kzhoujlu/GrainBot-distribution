# GrainBot-distribution

## Windows 安装与更新

[下载 Windows x64 安装器（单个 EXE）](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.15.installer7/GrainBot-Setup-Windows-x64-2026.10.15.installer7.exe)

首次运行建议选择 CPU。已有新版启动中心请在“版本与更新”中检查并更新应用与启动中心。旧 installer4 首次需关闭旧启动中心和网站服务，运行新版并选择原安装目录及原 CPU/CUDA 配置。现有模型、数据、设置及完整依赖会保留。

## 应用软件包

[GrainBot Studio post8](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.15.post8) 提供三个 Python wheel 和一个前端 ZIP，维护核心 0.2.12。本轮前端复用 post7 构建产物，未重新编译；MatMorph post2 保持不变。

新增已有 SEM pore ASPP (instance-balanced) 孔洞模型的一键安装入口，使用既有孔洞流程与 trained 后端；模型权重、阈值及后处理未改变，没有重新训练。安装及 CPU16 张逐项概率一致性已验证，这些训练图像不构成独立精度测试。

## 模型与数据资源

- [resources5：SEM pore ASPP (instance-balanced) 模型](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources5)
- [resources4：GrainBot-V2 SEM Pores（唯一 16 张合并集）](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources4)
- [resources3：GrainBot 原始默认权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources3)
- [resources1：既有数据集、模型适配包及 UO2 权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources1)
- [resources2：EMPS 与 ExONE 原始数据](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2)

孔洞模型按需单独安装：更新应用后，在模型库找到 SEM pore ASPP (instance-balanced)，安装完成后在孔洞识别中选择它。第三方尚未集成或尚未完整验收的模型不会因此获得可用性或精度承诺。所有历史 Release 文件保持不变。
