# Deep-Learning-Based-CT-Image-Denoising-Using-RED-CNN


## Overview

This project uses a **RED-CNN (Residual Encoder-Decoder CNN)** model to reduce noise and enhance CT images.

The model is trained using clean CT images with simulated low-dose noise and evaluated using **PSNR** and **SSIM**.

## Dataset

The project uses CT images with different reconstruction kernels:

* Sharp Kernel (D45) for training
* Soft Kernel (B30) for inference
* 3 mm slice thickness

## Model & Training

* Framework: **PyTorch**
* Model: **RED-CNN**
* Optimizer: **Adam**
* Loss Function: **MSE**
* Data Augmentation: Flip and Rotation

## Results

The enhanced CT images are evaluated using:

* **PSNR** – measures image reconstruction quality.
* **SSIM** – measures structural similarity.

The best trained model is saved as:

`best_redcnn_by_psnr.pth`

Enhanced images are saved in:

`enhanced_results/`

## Technologies

Python • PyTorch • NumPy • scikit-image • pydicom • PIL • Matplotlib • Torchvision

## Future Improvements

* Train with a larger dataset
* Increase training epochs
* Compare with other denoising models
* Use real low-dose CT data

## Author

**Ankit Singh**
