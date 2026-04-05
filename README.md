# 🛢️ Oil Spill Detection using SAR Imagery and Deep Learning

## 📌 Introduction
Oil spills in oceans pose serious environmental threats, impacting marine ecosystems and coastal regions. Detecting oil spills accurately using satellite imagery is challenging due to noise, low contrast, and similar-looking patterns (look-alikes).  

This project presents an advanced deep learning pipeline for **oil spill detection using Synthetic Aperture Radar (SAR) images**, leveraging preprocessing techniques, attention-based neural networks, and robust training strategies.

---

## 🎯 Objective
- Detect oil spills from SAR images
- Improve classification accuracy using advanced preprocessing and deep learning
- Handle noise and environmental variability in satellite imagery

---

## 📂 Dataset
- Dataset format: **COCO segmentation format**
- Classes include:
  - Oil Spill
  - Look-alike
  - Ship
  - Land

⚠️ Dataset is not included due to size constraints.  
You can use any SAR oil spill dataset in COCO format.

---

## 🧠 Key Features

### 🔬 SAR Preprocessing
- Advanced despeckling (Lee filter)
- Contrast enhancement using CLAHE
- Texture feature extraction using GLCM

---

### 🔄 Data Augmentation
- Albumentations-based pipeline
- Flips, rotations, noise, distortion
- Improves model robustness

---

### 🏗️ Model Architecture
- Based on **ResNet50**
- Custom improvements:
  - Attention blocks for feature enhancement
  - Fully connected deep classifier
  - Dropout & batch normalization

---

### ⚙️ Training Techniques
- Label Smoothing + Focal Loss
- Mixed Precision Training (faster & efficient)
- Gradient Clipping
- Gradient Accumulation
- Cosine Annealing Scheduler
- Stochastic Weight Averaging (SWA)
- Early Stopping

---

### 📈 Evaluation Metrics
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- ROC Curve & AUC Score

---

## 📊 Results

- ✅ Validation Accuracy: **~89.45%**
- ✅ Test Accuracy: **~88%**
- 📈 ROC AUC Score: **0.9259**

The model demonstrates strong performance in distinguishing oil spills from similar patterns.

---

## ⚙️ Project Workflow

1. Data Loading (COCO format)
2. SAR Image Preprocessing
3. Data Augmentation
4. Model Training (ResNet50 + Attention)
5. Evaluation (metrics + visualization)
6. Inference with Test-Time Augmentation (TTA)

---

## ▶️ How to Run

### 1. Clone Repository
### 2. Install Dependencies
### 3. Run in Google Colab
- Mount Google Drive
- Update dataset paths
- Run all cells
