---
layout: default
title: Project Home
---

<div align="center">
  <a href="https://doi.org/10.1002/mp.17970" style="text-decoration:none;">
    <img src="https://img.shields.io/badge/Paper-Medical_Physics-b31b1b.svg" alt="Paper Link">
  </a>
  <a href="assets/pdf/SAM-VMNet_Paper.pdf" style="text-decoration:none;">
    <img src="https://img.shields.io/badge/PDF-Download-red.svg" alt="Download PDF">
  </a>
  <a href="https://github.com/qimingfan10/SAM-VMNet" style="text-decoration:none;">
    <img src="https://img.shields.io/badge/Code-GitHub-black.svg" alt="GitHub Code">
  </a>
</div>

---

# Deep Learning Model for Coronary Artery Segmentation and Quantitative Stenosis Detection

## Overview

This project presents **SAM-VMNet**, a deep learning model designed for automated coronary artery segmentation and quantitative stenosis detection from coronary angiography images. The model combines advanced segmentation techniques with clinical quantification capabilities.

## Key Features

- **Automated Segmentation**: Precise coronary artery segmentation from angiography images
- **Stenosis Detection**: Quantitative detection and measurement of arterial narrowing
- **Clinical Integration**: Designed for practical clinical workflow integration
- **High Accuracy**: State-of-the-art performance on coronary imaging datasets

## Model Architecture

### Workflow Overview

The SAM-VMNet pipeline consists of:

1. **Image Preprocessing**: Normalization and augmentation of input angiography images
2. **Feature Extraction**: Multi-scale feature extraction using deep neural networks
3. **Segmentation**: Pixel-wise classification for vessel detection
4. **Post-processing**: Morphological operations and skeleton extraction
5. **Stenosis Analysis**: Quantitative measurement of vessel narrowing

### Architecture Details

SAM-VMNet leverages:
- **Encoder-Decoder Structure**: For precise spatial localization
- **Multi-scale Features**: Capturing vessels at different scales
- **Attention Mechanisms**: Focusing on relevant anatomical regions
- **Skip Connections**: Preserving fine details during upsampling

## Method

### Input Data
- Coronary angiography images (X-ray fluoroscopy)
- Various imaging protocols and equipment manufacturers supported

### Processing Pipeline
1. Automated vessel segmentation
2. Centerline extraction
3. Diameter measurement along vessel length
4. Stenosis classification and severity assessment

### Key Innovation
Combines advanced segmentation networks with clinical quantification metrics, enabling both anatomical understanding and functional assessment of coronary stenosis.

## Results

The model demonstrates:
- **Segmentation Accuracy**: High Dice coefficient and sensitivity
- **Stenosis Detection**: Accurate classification of significant stenosis (>50% narrowing)
- **Clinical Relevance**: Results correlate with clinical assessment standards

### Quantitative Performance
- Vessel segmentation sensitivity and specificity
- Stenosis detection accuracy across different severity levels
- Robustness across different imaging systems

## Clinical Applications

1. **Diagnostic Assistance**: Automated detection of stenosis in coronary angiograms
2. **Quantification**: Objective measurement of vessel narrowing
3. **Workflow Integration**: Streamlined reporting and analysis
4. **Research**: Standardized assessment for clinical studies

## Dataset

The model was trained and validated on:
- Coronary angiography image datasets
- Multiple acquisition protocols and imaging systems
- Diverse patient populations

## Requirements

- Python 3.8+
- PyTorch/TensorFlow
- OpenCV
- NumPy, Scikit-image

## Usage

### Installation
```bash
git clone https://github.com/qimingfan10/SAM-VMNet.git
cd SAM-VMNet
pip install -r requirements.txt
```

### Inference
```python
from model import SAMVMNet
import cv2

# Load model
model = SAMVMNet(pretrained=True)

# Load image
image = cv2.imread('angiography.jpg')

# Predict
segmentation, stenosis = model.predict(image)
```

### Output
- Segmentation mask showing vessel locations
- Stenosis classification and severity scores
- Quantitative measurements (diameter, narrowing percentage)

## Citation

If you use this work, please cite:

```bibtex
@article{SAMVMNet2024,
  title={Deep learning model for coronary artery segmentation and quantitative stenosis detection},
  journal={Medical Physics},
  year={2024},
  doi={10.1002/mp.17970}
}
```

## References

Key related works and methodologies:
- Coronary artery segmentation in angiography
- Vessel analysis and stenosis quantification
- Deep learning for medical image analysis
- Clinical decision support systems

## Contact & Questions

For questions or feedback regarding this project, please refer to the main repository or contact the authors through the affiliated institutions.

## Acknowledgments

This work was conducted at [Institution Name] in collaboration with clinical partners. We acknowledge the support of [Funding Agency] and the availability of clinical datasets.

---

**Last Updated**: 2024  
**License**: [Specify your license]  
**Status**: Published in Medical Physics
