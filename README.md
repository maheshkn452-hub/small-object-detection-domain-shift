# Small Object Detection Under Domain Shift

> **Status:** Ongoing Master's Thesis (2025 – Present) — Preliminary code, augmentation pipelines, and evaluation results uploaded.

## Overview
This Master's thesis investigates the robustness of modern object detection architectures when detecting small objects under cross-domain distribution shifts. Specifically, it evaluates how targeted data augmentation strategies affect detection performance across aerial/drone imagery (**VisDrone**) and general-purpose object benchmarks (**COCO**).

## Models & Tools Evaluated
* **Architectures:** YOLOv5, YOLOv8, Faster R-CNN
* **Datasets:** VisDrone, MS COCO
* **Frameworks & Libraries:** Python, PyTorch, Albumentations

## Datasets
Raw image datasets are excluded from this repository due to GitHub file size limits. Experiments are conducted using standard public object detection benchmarks:
* **VisDrone2019-DET** (aerial/drone small-object benchmark)
* **MS COCO** (general-purpose object detection benchmark)
## Datasets & Expected Directory Structure
Raw dataset archives are excluded from this repository due to file size limits. To reproduce experiments, download the standard **VisDrone2019-DET** and **MS COCO 2017** splits and place them in the following directory structure:

```text
data/
├── VisDrone2019-DET-train/
├── VisDrone2019-DET-val/
├── annotations_trainval2017/
└── val2017/

## Repository Contents
* `src/` / scripts — Training, inference, and domain-shift evaluation pipelines
* `augmentations/` — Albumentations configurations for small-object robustness
* `results/` — Preliminary mAP metrics, precision-recall curves, and visual comparisons

## Roadmap
- [x] Baseline evaluations on VisDrone and COCO
- [x] Data augmentation pipeline setup using Albumentations
- [ ] Cross-domain generalization experiments across YOLOv5, YOLOv8, and Faster R-CNN
- [ ] Final thesis benchmarking and ablation analysis
