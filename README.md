# Pneumonia Detection using CNN (ResNet50 & VGG16)

## Project Description

This project focuses on detecting pneumonia from chest X-ray images using deep learning techniques. Two pretrained convolutional neural network architectures (VGG16 and ResNet50) are used and compared.

The project also incorporates Grad-CAM (Gradient-weighted Class Activation Mapping) to provide visual explanations of model predictions, improving interpretability in a medical context.

---

## Technologies

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* OpenCV

---

## Results

* ResNet50 achieved: **78.21% accuracy**
* VGG16 achieved: **87.50% accuracy**

VGG16 showed better overall performance and more stable convergence, achieving the highest test accuracy.

---

## Dataset

The dataset is not included in this repository due to its size.

You can download it from Kaggle:  
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

After downloading:
- Extract the dataset
- Place it in your Google Drive or in a local `data/` folder

Expected structure:

chest_xray/
├── train/
├── val/
└── test/

---

## How to Run

1. Clone the repository:

```
git clone https://github.com/vecseyfanni/pneumonia-detection-xai.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Open the notebook in Google Colab or Jupyter:

```
pneumonia_xray.ipynb
```

4. Update the dataset path if needed (Google Drive or local).

---

## Features

* Transfer learning with VGG16 (feature extraction)
* Fine-tuning with ResNet50 (last layers unfrozen)
* Data preprocessing and augmentation pipeline
* Model comparison and evaluation
* Grad-CAM visualization for interpretability

---

## Credits

* Grad-CAM implementation inspiration:
  https://medium.com/@tanishqsardana/visualizing-how-cnn-thinks-cam-grad-cam-grad-cam-1dabcf886cc5

* This project was developed with the assistance of AI tools for:

  * improving code quality
  * debugging
  * refining documentation and explanations

---

## Notes

When running in Google Colab, the dataset is copied from Google Drive to local runtime (`/content`) for faster training performance.
