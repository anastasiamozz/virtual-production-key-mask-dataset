# virtual-production-key-mask-dataset
Dataset generation methodology, code, trained models, and experimental results for key-mask segmentation in virtual production.

# Scalable and Quality-Controlled Key-Mask Dataset Generation for Virtual Production

This repository accompanies the paper:

**Scalable and Quality-Controlled Key-Mask Dataset Generation for Virtual Production**

The repository contains the dataset-generation code, model-training and
evaluation code, experimental configurations, quantitative results, qualitative
comparisons, and links to the complete dataset and trained model checkpoints.

## Dataset

The proof-of-concept dataset contains 63 image–mask pairs generated from:

- 7 foreground assets
- 9 virtual backgrounds

The background-disjoint split contains:

- 49 training images using Backgrounds 1–7
- 7 validation images using Background 8
- 7 test images using Background 9

## Mask representation

The dataset-generation workflow produces 8-bit alpha masks with opacity values
from 0 to 255, including intermediate values along object boundaries.

For the segmentation experiments, the alpha masks were binarised by assigning
pixels with non-zero opacity to the foreground class and fully transparent
pixels to the background class.

## Evaluated models

- U-Net with a ResNet-34 encoder
- DeepLabV3 with a ResNet-34 backbone
- YOLOv8m-seg
- Detectron2 Mask R-CNN with R50-FPN
- Segment Anything with Concepts (SAM 3)

## Complete dataset and results

The complete dataset, trained checkpoints, predictions, metrics, training
histories, and comparison figures are available under the GitHub Release
`v1.0.0`.

## Reproducibility

All images were resized to 512 × 512 pixels. Training, validation, and test
subsets were separated by background. Configuration files and training logs
are provided for each evaluated model.

## Citation

Please cite the accompanying paper and repository when using these materials.
