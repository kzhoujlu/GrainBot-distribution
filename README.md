# GrainBot-distribution

## 安装与更新

[Windows x64 单个 EXE 安装器（installer12，约 1.4 MB）](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.27.installer12/GrainBot-Setup-Windows-x64-2026.10.27.installer12.exe)

当前应用为 [2026.10.27.post1](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.27.post1)，启动中心版本 0.2.16.1。本版修复面积分布拟合不收敛导致整次分析失败：保留分割、晶粒测量、角度、CSV 和统计图，失败的拟合参数显示为不可用并说明原因。

已有用户在启动中心“版本与更新”检查并更新应用，然后重启 Studio。也可运行上述 EXE，选择原安装目录和原 CPU/CUDA 配置。模型权重、科学依赖、数据和设置保留，未变化的软件包继续跳过。

本次前端已重新构建；维护核心 0.2.16 与 MatMorph post2 原样复用。没有重新训练模型或修改后处理，科学有效性与结构保留仍由用户人工判断。

安装器 Release 仅一个 EXE；应用 Release 为三个 wheel 和一个前端 ZIP。清单、签名、说明保存在 Git。此前本地交付的便携 ZIP 未上传。

## 推荐模型

| 场景 | 模型 | 安装源 |
|---|---|---|
| 粉末颗粒 | EMPS BPartIS Official | resources1，沿用已发布版本 |
| TEM 晶界 | Patrick BF-TEM U-Net Official | resources6 |
| 钙钛矿晶相 | Perovskite YOLOv8x instances | resources6 |
| 316L 光学金相晶界 | 316L RG DeepLabV3+ | resources6 |
| SEM 孔洞 | SEM pore ASPP (instance-balanced) | resources5 |

更新到 post11 并重启网页服务后，在模型库分别安装所需模型。模型推荐以适用图像和任务为依据，现有权重、阈值及后处理不变；未重新训练，也不因此获得跨材料精度承诺。

## 发布资源

- [resources6：TEM／钙钛矿／316L 三个独立模型包](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources6)
- [resources5：SEM 孔洞模型](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources5)
- [resources4：GrainBot-V2 SEM Pores，唯一 16 张合并集](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources4)
- [resources3：GrainBot 原始权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources3)
- [resources2：EMPS／ExONE 原始数据](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2)
- [resources1：BPartIS、既有数据及 UO2 资源](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources1)

全部历史 Release 文件保持不变。
