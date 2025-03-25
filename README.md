# SOCAL Dataset YOLOv8 Training Results

This repository contains the training results of a YOLOv8n model on the SOCAL dataset, which includes endoscopic surgical videos with 31,443 annotated frames across 147 trials. The model was trained for 50 epochs on a Mac with a CPU.

## Contents
- `results.csv`: Training and validation metrics for each epoch.
- `weights/`: Model weights (`best.pt` and `last.pt`).
- `plots/`: Validation plots including confusion matrix, F1 curve, precision-confidence curve, precision-recall curve, and recall-confidence curve.
- `args.yaml`: Training arguments used.

## Key Metrics (Epoch 50)
- Precision: 0.73438
- Recall: 0.57335
- mAP50: 0.6283
- mAP50-95: 0.4643

## Notes
- The model struggles with rare classes like `scalpel` and `drill` due to class imbalance.
- Training took approximately 82 hours on a CPU.

