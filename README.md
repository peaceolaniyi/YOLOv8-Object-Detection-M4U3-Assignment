
# YOLOv8 PPE Detection – M4U3 Assignment

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/peaceolaniyi/YOLOv8-Object-Detection-M4U3-Assignment/blob/main/notebooks/yolov8_object_detection_project_m4u3_group_3.ipynb)

---

## 1. Problem Statement

This project develops a YOLOv8 object detection model for Construction PPE Detection in AECO environments.

The goal is to detect:
- Human
- Helmet
- Vest
- Boots
- Gloves

The system supports safety compliance screening in construction environments.

---

## 2. Dataset

- Source: Roboflow – Construction PPE Detection
- Format: YOLOv8
- Train/Validation split: 80/20
- Image size: 640x640

---

## 3. Model Configuration

- Model: YOLOv8s (Small)
- Epochs: 30
- Image size: 640
- Batch size: default (Colab GPU)
- Ultralytics version: 8.4.x
- Environment: Google Colab (Tesla T4 GPU)

---

## 4. Results Summary

Validation Performance:

- Precision: ~0.90+
- Recall: ~0.85+
- mAP50: ~0.90
- mAP50–95: ~0.75

Training curves available in `/results/`.

### Key Observations:
- Strong detection for helmets and vests
- Slightly lower performance for gloves (small object size)
- Stable convergence over 30 epochs

---

## 5. Inference Evidence

Validation predictions and new image predictions are available in:

`/results/evidence/`

Example detection:

- Human detected with 0.97 confidence
- Vest detected with 0.93 confidence
- Boots detected with 0.88 confidence

---

## 6. Reproducibility

To reproduce results:

1. Click **Open in Colab**
2. Runtime → Restart Runtime
3. Run All Cells
4. Model will:
   - Install dependencies
   - Download dataset
   - Train for 30 epochs
   - Generate evaluation metrics
   - Save prediction outputs

---

## 7. Governance & Limitations

This model is an assistive screening tool only.

It:
- Produces false positives
- Produces false negatives
- Must NOT be used as the sole verifier for life-safety decisions.

See `/docs/governance_checklist.md` for full governance review.

---

## 8. License

MIT License – Academic use.

---
