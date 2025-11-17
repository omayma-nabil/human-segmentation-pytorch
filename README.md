# human-segmentation-pytorch

A complete deep learning project for **human segmentation** using three state-of-the-art architectures: **UNet**, **FPN**, and **DeepLabV3+**.  
The models are trained on the **Human Segmentation Dataset** and evaluated using metrics such as **IoU**, **Dice Score**, and **training time**.



## 1. Project Overview

This project compares three architectures commonly used in semantic segmentation:  
**UNet**, **FPN**, and **DeepLabV3+**.  
The goal is to evaluate their performance on a human segmentation dataset and analyze:

- segmentation accuracy  
- generalization ability  
- visual prediction quality  



##  2. Dataset

**Dataset name:** Human Segmentation Dataset  
**Size:** 290 RGB images  
**Labels:** Binary masks (human vs background)

**Mask values:**

- `1` → human  
- `0` → background  


---

## 3. Installation

Install required packages:

```bash
pip install segmentation-models-pytorch
pip install git+https://github.com/albumentations-team/albumentations
pip install opencv-contrib-python
