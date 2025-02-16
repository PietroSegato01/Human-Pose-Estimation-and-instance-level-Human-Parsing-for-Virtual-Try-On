# Human Pose Estimation and instance-level Human Parsing for Virtual Try-On

This repository contains the code and resources for the VITONHD-based virtual try-on pipeline, developed as a group project for the **Vision and Cognitive System** course at the University of Padova.

---

## Table of Contents
- [Overview](#overview)
- [Process Workflow](#process-workflow)
- [Notebooks](#notebooks)
- [Authors](#authors)
- [References](#references)
- [License](#license)

---

## Overview

The goal of this project is to implement a virtual try-on system by integrating our custom modules within the VITONHD framework. The system leverages:
- **Self-Correction Segmentation:** Our segmentation module for accurately extracting garment masks.
- **OpenPose Pose Estimation:** A robust module for detecting human keypoints to ensure proper garment alignment.
- **VITONHD Framework:** A high-resolution virtual try-on method that synthesizes realistic images by combining the outputs from the segmentation and pose estimation stages.

---

## Process Workflow

1. **Segmentation:**
   - Apply our Self-Correction segmentation module to generate precise garment masks.
2. **Pose Estimation:**
   - Use OpenPose to extract keypoints and determine the human pose accurately.
3. **Integration with VITONHD:**
   - Feed the outputs from the segmentation and pose estimation modules into the VITONHD pipeline.
   - The main Colab notebook (`VITONHD_main`) consolidates these inputs to produce the final try-on images.

---

## Notebooks

- **VITONHD_main:**  
  This is the primary Colab notebook. It integrates the outputs from the other two notebooks and executes the final virtual try-on synthesis.  
  **Note:** Ensure that the files produced by the segmentation and pose estimation notebooks are provided as inputs here.

- **Segmentation Notebook:**  
  Generates the garment masks using our Self-Correction segmentation method.

- **Pose Estimation Notebook:**  
  Utilizes OpenPose to detect and output the keypoints for accurate pose estimation.

---

## Authors

- **Segato Pietro** (pietro.segato.1@studenti.unipd.it)
- **Vezzosi Giacomo** (giacomo.vezzosi@studenti.unipd.it)
- **Vitali Giovanni** (giovanni.vitali@studenti.unipd.it)

*This project is a collaborative work carried out for the Vision and Cognitive System course at the University of Padova.*

---

## References

- **VITONHD Framework:**  
  [VITONHD Repository](https://github.com/shadow2496/VITON-HD)
- **OpenPose:**  
  [OpenPose GitHub](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
  [OpenPose Pytorch](https://github.com/Hzzone/pytorch-openpose)
- **Self-Correction Segmentation:**  
  [SSSegmentation]([https://github.com/shadow2496/VITON-HD](https://github.com/SegmentationBLWX/sssegmentation)) 
  [Self-Correction Human parsing](https://github.com/GoGoDuck912/Self-Correction-Human-Parsing)

*Additional references and citations to related works and methodologies are included as appropriate.*
