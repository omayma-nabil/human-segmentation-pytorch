# human-segmentation-pytorch
Image Segmentation with PyTorch — UNet, FPN, DeepLabV3+

A complete deep learning project for human segmentation using three state-of-the-art architectures: UNet, FPN, and DeepLabV3+.
The models are trained and evaluated on the Human Segmentation Dataset, and compared using metrics such as IoU, Dice Score, and training time.

🔍 1. Project Overview

This project compares three widely used architectures for semantic segmentation: UNet, FPN, and DeepLabV3+.
The objective is to evaluate their performance on a human segmentation dataset and analyze their accuracy, generalization ability, and prediction quality.

📂 2. Dataset

Name: Human Segmentation Dataset

Size: 290 images

Type: RGB images + binary masks

Mask values:

1 → human

0 → background

👉 Dataset link: https://github.com/parth1620/Human-Segmentation-Dataset-master

🛠️ 3. Installation
pip install segmentation-models-pytorch
pip install git+https://github.com/albumentations-team/albumentations
pip install opencv-contrib-python


Clone the dataset:

git clone https://github.com/parth1620/Human-Segmentation-Dataset-master.git

🧩 4. Project Structure
├── Image_Segmentation_with_PyTorch.ipynb
├── Human-Segmentation-Dataset-master/
│   ├── train/
│   ├── test/
│   ├── train.csv
├── outputs/
│   ├── example_predictions/
└── README.md

🔧 5. Models Used

UNet

FPN (Feature Pyramid Network)

DeepLabV3+

All implemented using segmentation-models-pytorch.

⚙️ 6. Training Configuration
Parameter	Value
Epochs	25
Batch Size	16
Optimizer	Adam
Learning Rate	0.003
Encoder	EfficientNet-B0
Image Size	320×320
Loss Function	Dice Loss + BCE
📊 7. Results

(Add your actual numbers later — here is a template)

📌 Quantitative Results
Model	IoU	Dice Score	Training Time
UNet	0.87	0.92	12 min
FPN	0.85	0.91	10 min
DeepLabV3+	0.89	0.93	18 min
🖼️ 8. Visual Results

(Add images later)

Examples:

Input Image

Ground Truth Mask

Model Prediction

🚀 9. How to Run

Run training:

python train.py


Run prediction:

python predict.py


Or simply open the notebook:

Image_Segmentation_with_PyTorch.ipynb

👤 10. Author

Omayma Nabil
Master’s student in Data Science & Intelligent Systems
Passionate about Computer Vision and Deep Learning
