# Automatic Renal Lithiasis Classification in Axial CT Images Using Deep Learning
This repository contains two notebooks that implement deep learning models for the **automatic classification of renal lithiasis** in axial computed tomography (CT) images.

## Repository Contents
- CNN_Model.ipynb – Implementation of a custom Convolutional Neural Network (CNN).
- MobileNetV2_Model.ipynb – Implementation of a model based on MobileNetV2 using transfer learning.

Both notebooks include:
- Data partitioning (training/validation split: 70/30).
- Complete image preprocessing pipeline.
- Model training and evaluation.

## Image Preprocessing
Each notebook includes a preprocessing pipeline with the following steps:

- **Grayscale conversion**
- **Resizing** to 512x512 pixels
- **Normalization** to range [0, 1]
- **Median filtering** for noise reduction
- **Edge masking** using the Sobel filter
- **Gamma correction** to enhance contrast

## Dataset Structure
The dataset should be organized as follows:
Kindey Stone Dataset/CT/
├── train/
│ ├── Stone/
│ └── Non-Stone/
└── val/
├── Stone/
└── Non-Stone/

**Note:** The origin and details of the dataset are described in the article. Please refer to the publication for more information on how the dataset was obtained and curated.

## Citation
W. Obregón Londoño, A. Daza Cerón, C. Torres Valencia, and D. F. Ramírez Jiménez, “Automatic Classification of Renal Lithiasis in Axial CT Images Using Deep Learning”, Cali, Colombia, 2025.

@inproceedings{Obregon2025RenalLithiasis,
  title     = {Automatic Classification of Renal Lithiasis in Axial CT Images Using Deep Learning},
  author    = {W. Obregon Londoño and A. Daza Cerón and C. Torres Valencia and D. F. Ramirez Jimenez},
  booktitle = {},
  year      = {2025},
  address   = {Cali, Colombia},
  doi       = {}
}
