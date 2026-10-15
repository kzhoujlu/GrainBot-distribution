One-click installation of the existing recommended TEM, perovskite phase and 316L models.

- Adds Patrick BF-TEM U-Net Official, Perovskite YOLOv8x instances and 316L RG DeepLabV3+ from three pinned resources6 ZIPs.
- Preserves the existing inference, weights, thresholds and postprocessing. No model is trained or scientifically reaccepted by this release.
- Routes the installed BF-TEM and 316L models to the selected model directory and resolves the perovskite MatMorph backend alias. Existing powder and pore resources remain available.
- Includes maintenance 0.2.13 and the matching native catalog. All three models remain optional downloads.

Three Python wheels and one frontend ZIP form the application. Frontend build reused byte-for-byte from post7/post8; it was not recompiled. MatMorph post2 is unchanged. 前端复用已有构建产物，未重新编译。

Validation: 35 focused catalog/installer/web-download tests; actual CPU install and three-image output equality per model against original local artifacts; repeat-install skip; final independent application install, health/frontend/catalog and 16 SEM dataset image/label previews and web opens. Domain limits remain: TEM recommendation is BF-TEM aluminum, metallography recommendation is real 316L optical imaging, and perovskite phase identity follows the existing three-class schema.
