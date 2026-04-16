# Assignment 03 - Kaggle Competition

![Competition Score](score.png)

## Overview
This repository contains my coursework project for the **Plant Pathology 2021** Kaggle competition.
It includes training, offline inference, and submission workflows built around a DINOv2-based classifier.

## Notebooks
- `PlantPathology2021_Competition-1.ipynb`: training pipeline.
- `PlantPathology2021_Competition-Inference-Offline.ipynb`: offline inference and submission pipeline.

## Model Artifact
The trained model is published on Kaggle:
- **Model name**: `v005pth`
- **Kaggle model page**: https://www.kaggle.com/models/junyaoshi6416/v005pth

## Public Kaggle Notebook
- https://www.kaggle.com/code/junyaoshi6416/assignmentnotebookd2890fcc7c

## Version Notes
### v003 / v004
These versions introduced:
- Tile-based inference (slice first, then resize), which significantly increased compute cost.
- Threshold tuning, which also increased computation and led to overfitting.
- AutoAugment.

Potential issue observed:
- Color-heavy augmentation may harm disease recognition in some cases (e.g., color shifts that make one disease pattern resemble another).

### v005 (Current Preferred Setup)
v005 simplifies the pipeline and uses a more stable baseline:
- Default threshold = `0.5`.
- No extra threshold tuning.
- No tile-based inference.
- Directly resize input to `518`, following the original notebook approach.

## Additional Files
- `v003logo.md` and `v005logo.md`: logo/visual records for the corresponding versions.

## Notes
All experiment versions are available on Kaggle.
