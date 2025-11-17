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



## 3. Installation

Install required packages:

```bash
pip install segmentation-models-pytorch
pip install git+https://github.com/albumentations-team/albumentations
pip install opencv-contrib-python

```
## 4. Models Used

- **UNet**  
  UNet is a convolutional neural network architecture designed for biomedical image segmentation.  
  It has an encoder-decoder structure with skip connections that help preserve spatial information, making it effective for segmenting small structures.

- **FPN (Feature Pyramid Network)**  
  FPN is designed to enhance feature extraction at multiple scales.  
  It builds a pyramid of features from different layers of a backbone network, allowing the model to detect objects or regions of various sizes effectively.

- **DeepLabV3+**  
  DeepLabV3+ is a state-of-the-art semantic segmentation model that uses atrous (dilated) convolutions to capture multi-scale context.  
  It also includes an encoder-decoder structure to refine segmentation boundaries and produce precise masks.

All models are implemented using `segmentation-models-pytorch`.


##  5. Training Configuration

This section summarizes the training configuration used for all models in this project. 

| Parameter      | Value               |
|----------------|-------------------|
| Epochs         | 25                 |
| Batch Size     | 16                 |
| Optimizer      | Adam               |
| Learning Rate  | 0.003              |
| Encoder        | EfficientNet-B0    |
| Image Size     | 320×320            |
| Loss Function  | Dice Loss + BCE    |

