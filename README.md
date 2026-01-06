# RVIS: Rice Variety Identification System 🌾
### Automated Adulteration Detection using Computer Vision & Deep Learning

![Status](https://img.shields.io/badge/Status-Prototype_Complete-green)
![Tech](https://img.shields.io/badge/AI-YOLOv8-blue)
![Research](https://img.shields.io/badge/Research-Vestra_Logics-purple)

## 📌 Abstract
The global rice trade faces significant challenges regarding varietal purity, particularly with high-value strains like **Basmati**. Current grading mechanisms in developing economies are subjective, slow, and prone to fraud (Economically Motivated Adulteration). 

**RVIS (Rice Variety Identification System)** is a computer vision framework designed to automate this process. Developed by **Vestra Logics**, this system utilizes a fine-tuned **YOLOv8-Classification** architecture to distinguish between morphologically similar rice varieties (e.g., Basmati vs. Jasmine) with high precision on edge devices.

## 🚀 Project Roadmap
- [x] **Phase 1: Synthetic Prototype** (Completed Jan 2026)
    - Developed `SimRice-v1` synthetic data generator.
    - Achieved 100% Top-1 Accuracy on validation sets.
    - Validated YOLOv8-CLS architecture on Google Colab T4 GPU.
- [ ] **Phase 2: The "PakRice-5K" Dataset** (In Progress)
    - Collection of 5,000 expert-annotated grain samples under controlled lighting.
    - Training for fissure detection and chalkiness analysis.
- [ ] **Phase 3: Mobile Deployment**
    - Android integration for real-time field analysis.

## 🛠️ Methodology
### 1. Model Architecture
We employed **YOLOv8-CLS (Nano)**, a state-of-the-art Convolutional Neural Network (CNN) optimized for speed.
* **Backbone:** CSPDarknet53 (Feature Extraction)
* **Input:** 224x224 pixels
* **Optimization:** Transfer Learning (Pre-trained on COCO)

### 2. Training Pipeline
* **Environment:** Google Colab (Tesla T4 GPU)
* **Epochs:** 20-50
* **Optimizer:** SGD (Momentum 0.937)

## 📊 Preliminary Results
Initial testing on synthetic morphological analogues demonstrated robust feature extraction capabilities. The model successfully distinguished grain aspect ratios (Long Grain vs. Short Grain) with **95.5%+ confidence** in <15ms inference time.

---
*© 2026 Vestra Logics. All Rights Reserved.*
