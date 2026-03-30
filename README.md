# PMAJT
Prototype-Guided Multimodal Alignment Joint Training for Facial Expression Recognition on Multiple Datasets

This repository provides the label text files used in our experiments.

## Available Materials

- Selected AffectNet subset for **RAF-DB** as the target dataset
- Selected AffectNet subset for **CAER-S** as the target dataset
- Label files for the full **RAF-DB** dataset
- Label files for the full **CAER-S** dataset

## Original Public Datasets

Please download the original datasets from their official websites:

- RAF-DB: http://whdeng.cn/RAF/model1.html#dataset
- AffectNet: https://mohammadmahoor.com/pages/databases/affectnet/
- CAER-S: https://caer-dataset.github.io/

This repository does not include the original image data.
The files in this repository are provided for academic research purposes only.  
Users must also comply with the terms and licenses of the original datasets (RAF-DB, AffectNet, and CAER-S).

## Abstract

Facial expression recognition plays an important role in human–computer interaction and affective computing.  
Although combining multiple FER datasets in joint training can potentially improve model robustness, such training remains challenging due to inconsistent labeling criteria, cross-cultural annotation differences, and dataset-specific biases.  
To address inconsistent labeling criteria across datasets, we propose a Prototype-Guided Multimodal Alignment Joint Training (PMAJT) framework for multi-dataset FER.  
The core idea is to leverage the image-text alignment knowledge learned by Vision-Language Models (VLMs) from the target dataset as a unified emotion labeling criterion across datasets, while deriving prototypes from the class-wise mean of visual features to serve as emotion anchors for reliable feature alignment in the latent space.  
Based on the consistency among semantic predictions, prototype-distance predictions, and auxiliary labels, semantically consistent auxiliary samples are selected for joint training.  
This alignment strategy unifies labeling criteria across datasets while preserving complementary information from multiple data sources.  
Extensive experiments show that the proposed framework, with the Amending Representation Module (ARM) as the backbone network, achieves 93.74% accuracy on the RAF-DB dataset and 98.31% on the CAER-S dataset, attaining state-of-the-art performance with strong robustness.  
The experimental results demonstrate that establishing semantically consistent labeling criteria across datasets is an effective strategy for multi-dataset FER learning.

## Notes

For related questions or code requests, please contact: liujj279@mail2.sysu.edu.cn
