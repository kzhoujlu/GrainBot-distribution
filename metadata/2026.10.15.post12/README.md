Fix optional perovskite YOLO dependencies blocking application installation and updates.

- Uses the official ultralytics-opencv-headless 8.4.124 distribution, matching GrainBot's existing opencv-python-headless. All 361 ultralytics source files match the former 8.4.124 wheel byte-for-byte.
- Resolves the complete optional dependency graph, including nvidia-ml-py and ultralytics-platform. Keeps the original strict pip check; no metadata edits or duplicate cv2 distributions.
- Existing legacy YOLO environments are migrated before application dependency checks. Downloads are staged first; journal and backup preserve the original YOLO package if migration fails or is interrupted. PyTorch/CPU/CUDA and scientific-library versions are constrained.
- Environments without YOLO remain unchanged; model installs use the same shared repair path.

Maintenance 0.2.16 / installer11. Frontend reuses the exact post11 ZIP; it was NOT rebuilt. MatMorph post2 is unchanged. 前端复用 post11 构建产物，未重新编译。Model weights and datasets are unchanged.

Upgrade the launch center first so its maintenance environment receives the repair, then update the application and restart the web service.
