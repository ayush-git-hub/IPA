# INFWIDE NightShot Image Restoration

## 📌 Overview

This project implements and evaluates **INFWIDE (Image and Feature Space Wiener Deconvolution)** for restoring degraded low-light and night-shot images.

The notebook automates the complete workflow including:

- Environment setup
- Dataset configuration
- Repository installation
- Bug fixes for dependency compatibility
- Model training
- Model evaluation
- Image restoration experiments

The project is designed to improve image quality in challenging night-time conditions by reducing blur and enhancing visual details.

---

## 🎯 Objectives

- Restore blurred night-shot images
- Improve image sharpness and quality
- Evaluate INFWIDE performance on low-light datasets
- Provide a reproducible training and testing pipeline

---

## 🚀 Features

- End-to-end training pipeline
- Automatic dataset setup
- INFWIDE model integration
- NightShot dataset support
- Training and validation workflows
- Dependency management
- Compatibility fixes for SciPy-related issues
- Colab-ready implementation

---

## 🛠 Technologies Used

- Python
- PyTorch
- Hydra
- NumPy
- SciPy
- OpenCV
- Scikit-Image
- PyTorch MSSSIM
- Google Colab

---

## 📂 Project Structure

```text
IPA-main/
│
├── INFWIDE_from_user_working_notebook_final.ipynb
├── README.md
└── Dataset/
```

---

## 📊 Dataset

This project uses the **NightShot Dataset**.

Dataset location expected by the notebook:

```text
INFWIDE/dataset/NightShot
```

The notebook automatically links the dataset from Google Drive when executed in Colab.

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/IPA.git
cd IPA
```

### Install Dependencies

```bash
pip install hydra-core
pip install hydra-colorlog
pip install colorlog
pip install pytorch-msssim
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### 1. Open the Notebook

```bash
jupyter notebook
```

or upload the notebook to Google Colab.

### 2. Mount Google Drive

The notebook automatically mounts Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

### 3. Place Dataset

Store the NightShot dataset in:

```text
/content/drive/MyDrive/NightShot
```

### 4. Run All Cells

Execute notebook cells sequentially to:

- Install dependencies
- Configure dataset
- Patch compatibility issues
- Train the model
- Evaluate results

---

## 🔧 Compatibility Fix

The notebook patches a known issue involving:

```python
scipy.finfo
```

which is replaced with:

```python
numpy.finfo
```

to ensure compatibility with newer package versions.

---

## 📈 Expected Outputs

- Trained model checkpoints
- Restored images
- Validation metrics
- Performance comparisons
- Qualitative visual results

---

## 🎥 Project Demonstration

### Phase 1

https://drive.google.com/file/d/18Gr5WNzTNl3nX0496Nrhoe6B4YPH5TqQ/view

### Phase 2

https://drive.google.com/file/d/1P2Fl_UXJoIwlfTCyMnSq2qL923UdT3BQ/view

---

## 🔬 Applications

- Night-time photography enhancement
- Surveillance systems
- Autonomous driving vision systems
- Mobile camera image restoration
- Low-light image processing research

---

## 📚 References

INFWIDE:
Image and Feature Space Wiener Deconvolution Network for Non-Blind Image Deblurring

Official Repository:
https://github.com/zhihongz/INFWIDE

---
