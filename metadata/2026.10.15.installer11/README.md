Repair YOLO dependency failures during installation and application updates.

Includes Studio post12 / maintenance 0.2.16. Migrates optional legacy ultralytics to official ultralytics-opencv-headless 8.4.124, installs its complete dependencies, and keeps strict pip check enabled. Existing scientific package versions are protected; no duplicate OpenCV, model re-downloads or retraining.

已有安装请先更新启动中心，再更新应用。若此前安装失败，运行本 EXE，选择原安装目录和原 CPU/CUDA 配置重试。用户模型、数据和设置保留。

Frontend ZIP is reused byte-for-byte from post11 and was not rebuilt. Web model-library category checks and selected batch updates remain included.

<!-- grainbot-launcher-update {"schema_version":1,"version":"0.2.16.0","asset":"GrainBot-Setup-Windows-x64-2026.10.15.installer11.exe"} -->
