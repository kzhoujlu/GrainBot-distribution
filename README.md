# GrainBot-distribution

## 安装与更新

[Windows x64 单个 EXE 安装器（installer12，约 1.4 MB）](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.27.installer12/GrainBot-Setup-Windows-x64-2026.10.27.installer12.exe)

当前应用为 [2026.10.27.post2](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.27.post2)，启动中心版本继续为 0.2.16.1。本版修正 GrainBot UNet 推理：BatchNorm 使用当前图像统计量，关闭随机 Dropout。模型权重、输入预处理、侵蚀核和次数、后续测量流程保持不变。

已有用户：在启动中心“版本与更新 → 应用软件”检查更新，更新完成后重启 Studio，再用相同图像重新分析。旧结果不会自动重算。上一版 [2026.10.27.post1](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.27.post1) 完整保留，已验证应用升级与回滚均保留测试账号。

安装器 installer12 仍可安装，其初始应用为 post1；新安装用户安装后可通过上述入口更新至本版。选择原安装目录和相同 CPU/CUDA 配置可保留原有数据。此次没有重发安装器或上传便携 ZIP。

前端复用 post1 构建产物，本次未重新编译；维护核心 0.2.16 原样复用。应用 Release 仅三个 wheel 和一个前端 ZIP，清单和签名保存在 Git。四个文件均已验证可匿名下载，SHA256 一致。实际晶界效果由用户检查，不以区域数量增加作为准确性结论。

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
