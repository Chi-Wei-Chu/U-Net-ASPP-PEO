## Introduction

This repository contains the full training code and model architectures for the Basic U-Net 9 and all the model architecture codes for MACB U-Net variants used in the study:
"Systematic Evaluation of Atrous Spatial Pyramid Pooling in U-Net for Pore Segmentation in Plasma Electrolytic Oxidation Coatings"
Chi-Wei Chu, Chun-Ming Lu, Wing Kiu Yeung (NTUT)

The project systematically evaluates the effect of Atrous Spatial Pyramid Pooling (ASPP) in different positions of the U-Net architecture (Encoder, Bridge, Decoder, and their combinations) to optimize segmentation performance on SEM images of PEO coatings.

Model training in our research was conducted on Google Colab, leveraging an NVIDIA L4 GPU to accelerate deep learning computations. The experiments were implemented using TensorFlow 2.18.0 and executed in a Python 3.11.11 environment.

## Dataset

This study uses a dataset of 200 annotated SEM images of Plasma Electrolytic Oxidation (PEO) coatings, each with a resolution of 800×800 pixels and a corresponding binary segmentation mask. The link of the image data is provided below:

- **All 200 images refined**: Contains 120 pairs of SEM images and binary masks used for training.  
  [Google Drive link](https://drive.google.com/drive/folders/1TA9XAipXuTeZOXL-kHosGFEmb7UryPmN?usp=sharing)


If you use this dataset, please cite this repository or contact the authors for further information.

## The Trained PEO Coating Segmentation Model

Researchers interested in using our trained model for pore segmentation in PEO coatings can do the following:

1. Download the trained Keras model file:  
   📥 [Direct Download (model.keras)](https://drive.google.com/uc?export=download&id=1_IejbF5LSs8bOgJJdlCHCfl_AXI8H7Y8)

2. Copy and run the inference code provided in the [`PEO coating segmentation`](https://github.com/Chi-Wei-Chu/U-Net-ASPP-PEO/blob/main/PEO%20coating%20segmentation) script.

📌 This project was tested with **Python 3.11.11**. The used libraries are listed below:
keras==3.6.0
numpy==1.26.4
scikit-image==0.25.0 
Pillow==11.1.0

