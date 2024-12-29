# OxfordPet Classifier and Segmentation

This repository contains the implementation of an advanced deep learning project focused on pet image classification, segmentation, and data augmentation using the **Oxford-IIIT Pet Dataset**. The project incorporates a **Custom CNN**, fine-tuned **TResNet_large**, **Generative Adversarial Networks (GANs)** for data augmentation, and a **UNet-like model** for image segmentation.

---

## Features

### 1. **Custom CNN**
- Built from scratch for classifying pet images into 37 categories.
- Architecture optimized with `SiLU` activation, `BatchNorm`, and pooling layers.
- Designed for flexibility and simplicity in experimentation.

### 2. **Pre-trained Model with Fine-Tuning**
- Fine-tuned **TResNet_large** for enhanced accuracy and efficiency.
- Leverages transfer learning to accelerate training.

### 3. **GAN-based Data Augmentation**
- Generates synthetic images to improve dataset diversity.
- Enhances model robustness and performance.

### 4. **UNet-like Segmentation Model**
- Performs pixel-level segmentation for accurate pet region extraction.
- Useful for object localization and ROI segmentation tasks.

---

## Dataset

The project uses the **Oxford-IIIT Pet Dataset**, which includes:
- **37 pet categories** with approximately 200 images per class.
- Ground truth annotations:
  - **Trimaps**: Foreground, background, and unclassified regions.
  - **Head bounding boxes**: Provided in PASCAL VOC format.
- Standardized train-validation-test splits for consistent evaluation.

---

## Results

### Custom CNN

- **Train Accuracy**: 78.79%
- **Validation Accuracy**: 76.46%

### Pre-trained Model with Fine-Tuning (TResNet_large)

- **Train Accuracy**: 99.49%
- **Validation Accuracy**: 93.81%

### UNet-like Segmentation
- **Intersection over Union (IoU)**: 0.7097


