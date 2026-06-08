# DSCF-Net

**Dual-Space Contrastive Frequency Network for Multi-Class Medical Image Classification**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
*(Paper Under Review)*

This repository contains the official PyTorch implementation of **DSCF-Net**, a novel CNN-Transformer hybrid architecture for medical image classification.

## 📌 Overview
Medical image classification presents significant challenges due to subtle inter-class differences, complex texture patterns, and severe class imbalance. Existing spatial-domain methods often fail to exploit frequency-domain disease signatures. **DSCF-Net** addresses these limitations through three synergistic contributions:

1. **Learnable Frequency Filter (LFF):** Applies a task-adaptive MLP-based amplitude mask to the 2-D Fourier spectrum, enabling the model to learn disease-specific frequency signatures.
2. **Cross-Space Interaction Module (CSIM):** Performs bidirectional cross-attention between spatial and frequency feature streams.
3. **Hierarchical Prototype Contrastive Loss (HPCL):** Boosts alignment and rare-class recall using a two-phase training strategy.

## 📂 Datasets (Data Availability)
Our proposed method is evaluated on three publicly available datasets. You can download the datasets directly from their official repositories below:

- **[ISIC 2018](https://challenge.isic-archive.com/data/)**: Skin Lesion Analysis Towards Melanoma Detection (7-class)
- **[Kvasir](https://datasets.simula.no/kvasir/)**: A Multi-Class Image Dataset for Gastrointestinal Diseases (8-class)
- **[COVID-CT](https://github.com/UCSD-AI4H/COVID-CT)**: A CT Scan Dataset about COVID-19 (Binary classification)

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- PyTorch 1.10+
- torchvision
- timm
- scikit-learn, pandas, numpy

### Installation
Clone this repository and install the required dependencies:
```bash
git clone [https://github.com/](https://github.com/)[your-username]/dscf-net.git
cd dscf-net
pip install -r requirements.txt
