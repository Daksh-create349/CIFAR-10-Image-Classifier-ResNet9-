# CIFAR-10 Image Classifier (ResNet9)

This repository features a high-performance Deep Learning model built with **PyTorch** and the **ResNet9** architecture. It is optimized for speed and accuracy, achieving a final test score of **91.76%**.



---

## 🚀 Performance Summary
* **Final Test Accuracy:** 91.76%
* **Training Time:** ~13 minutes total (20 epochs at ~40s per epoch)
* **Hardware:** Trained on a **Tesla T4 GPU** via Google Colab
* **Optimization:** Used `OneCycleLR` for faster convergence and `Adam` optimizer for stable loss reduction.

---

## 🧠 Model Architecture
ResNet9 uses "Residual" skip-connections to ensure that deep layers don't lose vital image information.
* **Feature Extraction:** Sequential convolutional blocks with Batch Normalization and ReLU activation.
* **Efficiency:** Designed specifically to process 32x32 images with maximum accuracy and minimum latency.
* **Regularization:** Includes Dropout and Weight Decay to ensure the model generalizes well to unseen data.



---

## 📥 User Guidelines: How to Test
To get accurate results, please ensure you only input images belonging to the following **10 categories**:

| Category | Description |
| :--- | :--- |
| **Transportation** | Airplane, Automobile, Ship, Truck |
| **Animals** | Bird, Cat, Deer, Dog, Frog, Horse |

> **Note:** This model is specialized for these 10 classes. Providing images outside of this list (like humans or furniture) will result in an incorrect classification, as the model will try to map the input to the nearest known category.

---