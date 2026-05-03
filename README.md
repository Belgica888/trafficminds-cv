# 🚦 TrafficMinds — AI-Powered Traffic Light Recognition

**Computer Vision Project | Python · EfficientNet-B0 · Transfer Learning · OpenCV**  
*Miami Dade College — Applied AI Program (2025)*  
*Team: Belgica Reyes · Eva Guimaraes · Alexander Garcia*

---

## Overview

TrafficMinds is an end-to-end computer vision system that classifies traffic light states from real-world images under challenging conditions — including glare, rain, low light, and unusual camera angles.

Built using deep learning and transfer learning, the system achieves **98.5% test accuracy** and is designed with real-world accessibility and safety applications in mind.

---

## The Problem

Traffic lights can be difficult to interpret in real-world conditions:

- ☀️ Glare from sunlight
- 🌧️ Bad weather and rain
- 🌙 Low lighting environments
- 📐 Unusual camera angles
- 👁️ Color vision deficiencies (colorblindness)

A misread traffic light — even for a few seconds — can lead to dangerous decisions. This project explores how AI can recognize traffic light states more reliably than human perception alone.

---

## Solution

An AI classification system trained on the **LISA Traffic Light Dataset** (real-world driving images) that predicts one of four states:

| Class | Description |
|-------|-------------|
| 🔴 Red | Stop signal |
| 🟡 Yellow | Caution signal |
| 🟢 Green | Go signal |
| ⬜ Unknown | Unrecognizable state |

---

## Models Evaluated

We tested three transfer learning architectures and compared their performance using accuracy and Macro-F1 score:

| Model | Test Accuracy | Macro-F1 | Notes |
|-------|--------------|----------|-------|
| ResNet18 | 97.52% | 96.72% | Strong baseline |
| MobileNetV3-Small | 98.32% | 97.62% | Lightweight, edge-ready |
| **EfficientNet-B0** | **98.50%** | **97.95%** | ✅ Selected model |

**EfficientNet-B0 was selected** for its highest accuracy, best Macro-F1 score, and most balanced performance across all traffic light classes — including minority classes like Yellow.

---

## Technical Pipeline
Real-world images (LISA Dataset)
↓
Image Preprocessing
· Resizing & normalization
· Data augmentation
· Class imbalance handling
↓
Transfer Learning (3 architectures evaluated)
· ResNet18
· EfficientNet-B0  ← selected
· MobileNetV3-Small
↓
Model Evaluation
· Accuracy · Precision · Recall
· F1-Score · Macro-F1 · Confusion Matrix
↓
Prototype Demo
· Live inference on unseen test samples
· Red / Yellow / Green classification
· Near-instantaneous latency (edge deployment ready)

---

## Results

EfficientNet-B0 demonstrated consistent performance across all classes, including the most challenging scenarios:

- ✅ Structural feature extraction under varying illumination
- ✅ Accurate chrominance mapping for Red, Green, and Yellow
- ✅ Near-instantaneous inference suitable for edge deployment
- ✅ Robust performance on unseen test samples

---

## Real-World Applications

This prototype demonstrates AI's potential to support:

- 🚗 **Driver assistance systems** — real-time traffic signal support
- 🏙️ **Intelligent traffic monitoring** — automated signal analysis
- ♿ **Accessibility tools** — assistive technology for colorblind users

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| EfficientNet-B0 | Primary classification model |
| Transfer Learning | Pre-trained weights + fine-tuning |
| OpenCV | Image preprocessing |
| LISA Dataset | Real-world training & test data |
| Jupyter Notebook | Development environment |
| Macro-F1 Scoring | Handles class imbalance fairly |

---

## Files in This Repo

| File | Description |
|------|-------------|
| `Final_Presentation_TrafficMinds.ipynb` | Full project notebook with code and analysis |
| `DemoVideo.mp4` | Live prototype demonstration |

---

## Key Takeaway

> This project demonstrates how AI and Computer Vision can be applied to real-world safety challenges — not just analyzing data, but supporting human decision-making in critical environments.

---

📧 belgicareyes85@gmail.com  
💼 [LinkedIn](https://linkedin.com/in/belgica-reyes-6bb996191)
