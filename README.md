# GrainBot-distribution

## 安装与更新

[Windows x64 单个 EXE 安装器](https://github.com/kzhoujlu/GrainBot-distribution/releases/download/2026.10.15.installer8/GrainBot-Setup-Windows-x64-2026.10.15.installer8.exe)

已有新版启动中心请在“版本与更新”检查应用及启动中心更新。首次安装建议 CPU；旧 installer4 首次升级需关闭旧启动中心和网站服务，运行本 EXE 并选择原目录、原 CPU/CUDA 配置。现有模型、数据、设置和未变化的依赖会保留。

[Studio post9 应用四件套](https://github.com/kzhoujlu/GrainBot-distribution/releases/tag/2026.10.15.post9)：三个 wheel、一个前端 ZIP，维护核心 0.2.13。前端复用 post7/post8 构建，未重新编译；MatMorph post2 不变。

## 推荐模型

| 场景 | 模型 | 安装源 |
|---|---|---|
| 粉末颗粒 | EMPS BPartIS Official | resources1，沿用已发布版本 |
| TEM 晶界 | Patrick BF-TEM U-Net Official | resources6 |
| 钙钛矿晶相 | Perovskite YOLOv8x instances | resources6 |
| 316L 光学金相晶界 | 316L RG DeepLabV3+ | resources6 |
| SEM 孔洞 | SEM pore ASPP (instance-balanced) | resources5 |

更新到 post9 并重启网页服务后，在模型库分别安装所需模型。模型推荐以适用图像和任务为依据，现有权重、阈值及后处理不变；未重新训练，也不因此获得跨材料精度承诺。

## 发布资源

- [resources6：TEM／钙钛矿／316L 三个独立模型包](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources6)
- [resources5：SEM 孔洞模型](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources5)
- [resources4：GrainBot-V2 SEM Pores，唯一 16 张合并集](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources4)
- [resources3：GrainBot 原始权重](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.15.resources3)
- [resources2：EMPS／ExONE 原始数据](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources2)
- [resources1：BPartIS、既有数据及 UO2 资源](https://github.com/kzhoujlu/GrainBot-resources/releases/tag/2026.10.14.resources1)

全部历史 Release 文件保持不变。
