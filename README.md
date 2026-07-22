# 🚀 Suspicious Behavior Classification Benchmark
### *Part I of the Suspicious Behavior Research Series*

<p align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-red?style=for-the-badge)
![Torchvision](https://img.shields.io/badge/Torchvision-Latest-orange?style=for-the-badge)
![Vision Transformer](https://img.shields.io/badge/Vision%20Transformer-ViT-success?style=for-the-badge)
![Computer Vision](https://img.shields.io/badge/Computer-Vision-purple?style=for-the-badge)
![Research Benchmark](https://img.shields.io/badge/Research-Benchmark-darkgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-black?style=for-the-badge)

</p>

---

# 📖 Overview

This repository presents **Part I** of the **Suspicious Behavior Research Series**, a research-oriented benchmarking study that investigates the effectiveness of multiple deep learning architectures for suspicious behavior image classification.

Rather than proposing a novel model, this work focuses on **systematically comparing established architectures under identical experimental conditions** to establish a reliable experimental baseline for future computer vision research.

The study evaluates three fundamentally different learning paradigms:

- CNN + Bi-LSTM
- Vision Transformer (ViT)
- CNN Feature Extraction + Support Vector Machine (SVM)

The findings from this benchmark serve as the foundation for the subsequent object detection study presented in **Part II** of the research series.

---

# 🔬 Research Motivation

Selecting an appropriate deep learning architecture is often one of the most important decisions in computer vision research.

Before developing larger surveillance and intelligent monitoring systems, it is essential to understand how different feature learning strategies perform on the same dataset.

This benchmark was conducted to answer a simple research question:

> **Which deep learning architecture provides the most effective representation for suspicious behavior image classification under a unified experimental pipeline?**

---

# 🎯 Objectives

- Develop a reproducible benchmarking pipeline
- Compare CNN-based and Transformer-based architectures
- Evaluate hybrid deep feature learning approaches
- Analyze model performance using identical preprocessing
- Establish a baseline for future suspicious behavior research

---

# 🏗️ Experimental Pipeline

```text
Dataset
    │
    ▼
Data Preprocessing
    │
    ▼
Image Normalization
    │
    ▼
Model Training
    │
    ├─────────────────────────────┐
    │                             │
    ▼                             ▼
CNN + Bi-LSTM            Vision Transformer
    │                             │
    └──────────────┐              │
                   ▼              ▼
        CNN Feature Extraction + SVM
                   │
                   ▼
        Performance Evaluation
                   │
                   ▼
         Model Benchmarking
                   │
                   ▼
      Best Architecture Selection
```

---

# 🧠 Models Evaluated

## 1️⃣ CNN + Bi-LSTM

A hybrid architecture combining convolutional feature extraction with Bidirectional Long Short-Term Memory to capture spatial feature relationships.

---

## 2️⃣ Vision Transformer (ViT)

A transformer-based architecture that processes images as sequences of visual patches using self-attention mechanisms.

---

## 3️⃣ CNN Feature + SVM

A hybrid machine learning pipeline where CNN acts as a deep feature extractor while Support Vector Machine performs the final classification.

---

# 📊 Evaluation Metrics

The benchmark uses standard classification metrics:

- Accuracy
- Precision
- Recall
- F1-score

---

# 🏆 Experimental Results

| Rank | Model | Accuracy | Precision | Recall | F1-score |
|------|--------|---------:|----------:|--------:|----------:|
| 🥇 | Vision Transformer | **96.53%** | **94.86%** | **96.53%** | **95.68%** |
| 🥈 | CNN Feature + SVM | **95.95%** | **94.30%** | **95.95%** | **95.10%** |
| 🥉 | CNN + Bi-LSTM | **93.06%** | **91.70%** | **93.06%** | **92.20%** |

---

# 📈 Key Findings

- Vision Transformer achieved the highest overall classification performance.
- CNN Feature + SVM demonstrated highly competitive results while maintaining a simpler decision boundary.
- CNN + Bi-LSTM provided a strong baseline but achieved comparatively lower overall performance.
- The benchmark highlights the effectiveness of transformer-based architectures for suspicious behavior classification.

---

# 🔬 Research Series

This repository is part of a broader research initiative exploring deep learning methods for suspicious behavior analysis.

## ✅ Part I — Image Classification Benchmark *(Current Repository)*

Models evaluated:

- CNN + Bi-LSTM
- Vision Transformer
- CNN Feature + SVM

Focus:

> Suspicious Behavior Image Classification

---

## 🚀 Part II — Object Detection Benchmark

Repository:

**Suspicious Behavior YOLOv10 vs RT-DETR Benchmark**

Models evaluated:

- YOLOv10n
- RT-DETR

Focus:

> Suspicious Behavior Object Detection

Together, these repositories provide a comprehensive evaluation of classification and detection paradigms for suspicious behavior analysis.

---

# 📂 Repository Structure

```text
Suspicious-Behavior-Classification-Benchmark
│
├── notebook/
│   └── Suspicious_Behavior_Benchmark.ipynb
│
├── results/
│   ├── cnn_lstm_results.csv
│   ├── final_model_comparison.csv
│   ├── vit_results.csv
│   
│
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

---

# ⚙️ Technologies Used

- Python
- PyTorch
- Torchvision
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

# 🚀 Future Work

This benchmark serves as an initial experimental study.

Future directions include:

- ConvNeXt Benchmark
- EfficientNetV2 Benchmark
- Swin Transformer Evaluation
- Cross-Dataset Validation
- Explainable AI (Grad-CAM)
- Real-Time Video Classification
- Lightweight Edge Deployment
- Multi-modal Behavior Analysis

---

# ⚠️ Disclaimer

This repository is intended for educational and research benchmarking purposes.

The objective of this project is to compare multiple deep learning architectures under a unified experimental setup rather than proposing a novel classification algorithm.

---

# 👨‍💻 Author

**Md Delwar Husen**

Undergraduate Student  
Information and Communication Engineering (ICE)

**Research Interests**

- Computer Vision
- Machine Learning
- Deep Learning
- Medical AI
- Vision Transformers
- Intelligent Surveillance

---

# ⭐ Support

If you found this repository useful for learning or research, consider giving it a ⭐.

It helps support open research and motivates future benchmarking studies.
