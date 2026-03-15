# BUSI 3-Class Classification Project

This folder contains a complete Deep Learning mini-project for classifying breast ultrasound images into:
- normal
- benign
- malignant

## Start Here

Primary document (recommended first read):
- `DLMI_BUSI_report.pdf`

Implementation notebook:
- `BUSI_assignment_DLMI.ipynb`

## Project Objective

Build and evaluate a 3-class classifier on the BUSI dataset while explicitly handling class imbalance.

## What This Project Implements

- Dataset loading from class-wise folders.
- Exclusion of segmentation mask images (`*_mask.png`) from training/evaluation.
- Stratified train/test split.
- Data augmentation for training.
- Transfer learning with pretrained ResNet-18.
- Alpha-weighted focal loss for imbalance handling.
- AdamW optimizer + cosine annealing LR scheduler.
- Checkpoint saving for best training loss.
- Final evaluation with confusion matrix and per-class precision/recall/F1.

## Expected Outputs

From the notebook, you should get:
- Best checkpoint file under `checkpoints_busi_cnn/`.
- Test accuracy printout.
- Confusion matrix plot.
- Training loss curve.
- Per-class metrics table in console output.

## Reproducibility

The notebook sets random seeds for Python, NumPy, and PyTorch. Results may still vary slightly across hardware/software environments.

## Notes

- Detailed methodology, equations, dataset statistics, and final interpretation are documented in `DLMI_BUSI_report.pdf`.
- Use this README as a quick index; use the report for full technical discussion.
