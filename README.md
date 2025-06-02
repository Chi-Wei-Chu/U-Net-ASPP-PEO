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

For the researchers in this field who would like to use our model for pore position segmentation directly, please copy the code in the "PEO coating segmentation" file and download the Keras file in the link: 
[Google Drive link](https://drive.google.com/file/d/1_IejbF5LSs8bOgJJdlCHCfl_AXI8H7Y8/view?usp=drive_link)
