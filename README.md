# IABI — Intelligent Analysis of Biomedical Images (Sharif University of Technology - Fall2025)

[![Course](https://img.shields.io/badge/Course-IABI-blue.svg)]()
[![Jupyter](https://img.shields.io/badge/Uses-Jupyter%20Notebooks-orange.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A curated repository of materials for the course **Intelligent Analysis of Biomedical Images**:
lecture notes, slides, notebooks, and paper presentations.

---

## Overview

- **University / Department:** Sharif University of Technology, CE 
- **Term:** Fall 2025  
- **Instructor:** Dr. Rohban 

This course covers classical and deep-learning approaches for biomedical image analysis,
including preprocessing, segmentation, classification, registration, MIL/WSI pipelines,
transformers, diffusion models, evaluation, and reproducibility.

---

## Syllabus (High-Level)

1. **Intro & Biomedical Imaging Modalities** (X-ray, CT, MRI, histopathology)
2. **Image Preprocessing & Classical CV** (filtering, morphology, features)
3. **CNNs for Classification** (transfer learning, imbalance, calibration)
4. **Segmentation** (U-Net family, metrics, post-processing)
5. **Detection & Localization** (two-stage/one-stage, nuclei/lesion detection)
6. **Registration** (classical vs. learning-based, metrics)
7. **Multiple Instance Learning** (WSI pipelines, attention MIL)
8. **Transformers in Vision** (ViT/UNETR/Swin for med-imaging)
9. **Generative Models** (VAEs & diffusion for augmentation/synthesis)
10. **Self-/Weakly-Supervised Learning** (contrastive, CLIP-like)
11. **Evaluation & Robustness** (metrics, uncertainty, domain shift)
12. **Reproducibility & MLOps** (wandb, DVC, Lightning)
13. **Ethics & Responsible AI** (fairness, privacy, data governance)
14. **Project Presentations**


---

## Getting Started

### 1) Environment

- **Python:** 3.10+  
- **Recommended:** `conda` (or `mamba`) + `pip`

```bash
# Create env
conda create -n iabi python=3.10 -y
conda activate iabi

# Core scientific stack
pip install numpy scipy scikit-image scikit-learn matplotlib jupyter

# DL stack (pick one that matches your GPU/CUDA)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
# or: pip install tensorflow

# Med-imaging helpers (optional)
pip install opencv-python albumentations SimpleITK monai nibabel tqdm pandas
