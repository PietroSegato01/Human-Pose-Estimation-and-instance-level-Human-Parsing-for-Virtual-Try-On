# VITONHD Virtual Try-On Project

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

The goal of this project is to implement a state-of-the-art virtual try-on system by integrating our custom modules within the VITONHD framework. The system leverages:
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

- **Segato Pietro**
- **Vezzosi Giacomo**
- **Vitali Giovanni**

*This project is a collaborative work carried out for the Vision and Cognitive System course at the University of Padova.*

---

## References

- **VITONHD Framework:**  
  [VITONHD Repository](https://github.com/your-vitonhd-repository) *(replace with the actual link)*
- **OpenPose:**  
  [OpenPose GitHub](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
- **Self-Correction Segmentation:**  
  *(Include relevant paper or repository link if available)*

*Additional references and citations to related works and methodologies are included as appropriate.*

---

## License

This project is licensed under the [MIT License](LICENSE).

---

For any questions, contributions, or further information, please feel free to open an issue or contact one of the authors.
