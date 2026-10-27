Keep grain analysis results available when the optional area-distribution fit does not converge.

- Segmentation, editable regions, grain measurements, angles, CSV exports and statistical plots remain available. The failed fit exponent is null, with an explicit warning; no fitted value is invented.
- Successful fits retain the existing equation, parameters and iteration limit. Model weights, preprocessing, postprocessing and measurement methods are unchanged.
- Verified with the reported image through an independently installed application: upload and analysis return HTTP 200; segmentation, labels, grain features and angles match the pre-fix outputs byte-for-byte.
- Includes a rebuilt frontend warning. Maintenance 0.2.16 and MatMorph post2 are reused unchanged; existing dependencies and model downloads do not need replacement.

Update the application in the launch center and restart Studio. New installations use installer12. Model effectiveness and structure preservation remain subject to human review.
