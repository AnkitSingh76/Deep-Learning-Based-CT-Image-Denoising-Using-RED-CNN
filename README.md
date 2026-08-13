# Deep-Learning-Based-CT-Image-Denoising-Using-RED-CNN

## Overview

This project uses a **RED-CNN (Residual Encoder-Decoder CNN)** model to reduce noise and enhance CT images.

The model is trained using clean CT images with simulated low-dose noise and evaluated using **PSNR** and **SSIM**.

## Dataset

* Training images: **211**
* Inference images: **211**
* Slice thickness: **3 mm**
* Training: **Sharp Kernel (D45)**
* Inference: **Soft Kernel (B30)**
* Image size: **256 × 256**

## Model & Training

* Framework: **PyTorch**
* Model: **RED-CNN**
* Epochs: **5**
* Batch size: **8**
* Learning rate: **0.0001**
* Optimizer: **Adam**
* Loss: **MSE**
* Validation split: **10%**

## Results

The model evaluates CT image quality using:

* **PSNR** – measures image reconstruction quality.
* **SSIM** – measures structural similarity.

The best model is saved based on the highest validation PSNR as:

`best_redcnn_by_psnr.pth`

Enhanced CT images are saved in:

`enhanced_results/`

### Result Summary

| Parameter        |     Result |
| ---------------- | ---------: |
| Training Images  |        211 |
| Inference Images |        211 |
| Epochs           |          5 |
| Image Size       |  256 × 256 |
| Evaluation       | PSNR, SSIM |

> Actual epoch-wise PSNR, SSIM, and loss values are generated when the model is trained and are not included in the uploaded code.

## Technologies

Python • PyTorch • NumPy • OpenCV/PIL • scikit-image • pydicom • Matplotlib


