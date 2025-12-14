---
title: "Automated Counting and Gender Identification of Parasitoid Wasps"
excerpt: "A two-stage deep learning framework using YOLOv7 and ResNet18 for high-accuracy parasitoid wasp counting and sex identification.<br/><img src='/images/projects/insect-detection/cover.png'>"
collection: portfolio
permalink: /projects/insect-detection/
date: 2025-07-13
venue: "ASABE Annual International Meeting"
paperurl: "https://doi.org/10.13031/aim.202500146"
pdfurl: /files/insect-paper.pdf
order: 1
---

## Project Context

This project was conducted as an **academic research and applied computer vision project**
within the Department of Biomechatronics Engineering at National Taiwan University and was
published at the **ASABE Annual International Meeting**.

**Project Type:** Academic research & applied AI system  
**Application Domain:** Precision agriculture & biological monitoring  
**Problem Focus:** Automated visual inspection for large-scale biological analysis  

This page documents the **complete system pipeline** that I designed and implemented,
from dataset preparation and model training to robustness evaluation and performance analysis.

---

## Introduction

Parasitoid wasps are widely used in sustainable agriculture for biological pest control.
In mass-rearing and quality control processes, accurate counting and gender identification
are critical, as only female wasps possess parasitism capability.

Due to their extremely small size of approximately one millimeter and subtle morphological differences, manual
microscopic inspection is labor-intensive and difficult to scale. This project develops a
semi-automated two-stage deep learning pipeline for counting and sex identification of
*Trissolcus* sp. parasitoid wasps, combining object detection and fine-grained classification
to achieve high accuracy under dense and overlapping conditions.

---

## My Role and Contributions

I was responsible for the **end-to-end design and implementation** of the proposed framework.
My contributions include:

- Designing the overall two-stage system architecture
- Preparing and organizing high-resolution annotated datasets
- Training and tuning YOLOv7 for small-object detection under dense scenes
- Implementing morphology-preserving preprocessing for gender classification
- Training and evaluating ResNet18-based fine-grained classifiers
- Designing robustness and cross-species validation experiments
- Analyzing results and preparing figures and performance reports for publication

This work reflects my direct involvement across **data preparation, model training,
evaluation, and system-level analysis**.

---

## Method Overview

The proposed system consists of two sequential stages:

1. Wasp detection and counting  
2. Gender classification  

High-resolution images are first processed to localize individual wasps efficiently,
followed by fine-grained gender classification on cropped regions.

---

## Stage I: Wasp Detection and Counting (YOLOv7)

High-resolution scanner images (3981 × 3981 px) are downsampled to **1120 × 1120 px**
for efficient detection.

A **YOLOv7** detector is trained to localize individual wasps, and the total count
is obtained by summing predicted bounding boxes.

### Training Details
- Optimizer: SGD  
- Learning rate: 0.001  
- Momentum: 0.937  
- Weight decay: 0.0005  
- Epochs: 100  
- Batch size: 4  

This stage achieved **mAP@0.5 = 99.4%**.

---

## Stage II: Gender Classification (ResNet18)

Detected bounding boxes are mapped back to the original images and cropped without resizing.
Crops are center-padded to **640 × 640 px** to preserve morphological features.

The classifier predicts:
- Female
- Male
- Unrecognizable

---

## Dataset

### Image Acquisition
- Species: *Trissolcus* sp.
- Imaging device: Flatbed scanner (6400 dpi)
- Total annotated images: 150
- Train/test split: 4:1

### Classification Dataset

| Class | Samples |
|------|--------|
| Female | 2,927 |
| Male | 1,166 |
| Unrecognizable | 584 |
| **Total** | **4,677** |

Annotations were performed by entomology experts using LabelImg.

---

## Experimental Results

### Detection Performance (YOLOv7)
- Precision: 99.9%
- Recall: 98.7%
- F1-score: 99.3%
- mAP@0.5: **99.4%**

### Gender Classification Performance (ResNet18)
- Overall accuracy: **96.74%**
- Mean average precision: **95.86%**

#### Per-Class Performance

| Class | Precision | Recall | F1-score |
|------|----------|--------|---------|
| Female | 99.3% | 95.8% | 97.5% |
| Male | 96.5% | 98.9% | 97.7% |
| Unrecognizable | 91.8% | 92.6% | 92.2% |

---

## Robustness Evaluation

### Dense & Overlapping Wasps
- Detection mAP: 99.7%
- Classification accuracy: 92.89%

### Cross-Species Validation (*Trissolcus mitsukurii*)
- Detection mAP: 99.8%
- Classification accuracy: 92.23%

These results demonstrate strong **generalization across species and imaging conditions**.

---

## Outcomes and Impact

This project enabled:

- Reliable automated counting for large-scale biological monitoring
- Accurate fine-grained classification under dense and occluded conditions
- Significant reduction of manual microscopic inspection effort

The proposed framework demonstrates how **deep learning–based perception systems**
can be deployed in real-world agricultural and biological engineering applications.

---

## Skills and Tools Used

- Python
- YOLOv7
- ResNet18
- Computer vision preprocessing
- Deep learning model training and evaluation
- Dataset annotation and quality control
- Scientific performance analysis

---

## Conclusion and Future Work

This project presents a **scalable and highly accurate automated pipeline** for parasitoid
wasp counting and gender identification.

Future work includes:
- Expanding datasets across additional species
- Improving robustness under extreme occlusion
- Integrating synthetic data augmentation
- Deployment in real-world agricultural monitoring workflows
