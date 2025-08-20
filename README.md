# CSC14116 – Applied Parallel Programming - Changing Image Background using U-Net

## 📌 Introduction

This project applies the **U-Net model** to change image backgrounds by segmenting the foreground object and replacing the background. The work explores both **sequential** and **parallel implementations** to evaluate model performance in terms of **accuracy** and **execution time**.

---

## 📂 Project Framework

* **Framework Project**: U-Net-based image segmentation
* **Approach**: Sequential → Parallel implementation
* **Evaluation**: Accuracy and runtime performance

---

## 🛠️ Approach

1. **Reference Model**: Introduce the baseline segmentation model for comparison.

2. **Version 1 – Sequential Setup**:

   * **Design**: Architecture with convolutional, pooling, and activation layers.
   * **Implementation**: Added required libraries and drive connection.
   * **Layers used**:

     * Activation (`relu`, `sigmoid`)
     * MaxPool2D
     * Conv2D
     * Conv2D Transpose

3. **U-Net Model**: Build and train the U-Net for segmentation.

4. **Background Replacement**: Apply the trained model to replace the background of images.

5. **Model Evaluation**:

   * Accuracy
   * Execution Time

6. **Parallel Implementation**:

   * **Design**: Optimize kernel usage and GPU parallelization.
   * **Analysis**: Compare sequential vs parallel.

---

## 📊 Results  

- **Accuracy**: Evaluated using reference metrics.  
- **Runtime**: Compared sequential vs parallel execution to highlight speedup.  
- **Background Replacement Demo**: Successfully applied on sample images.  

| Original Image | Background Removed | Background Replaced |
|----------------|--------------------|----------------------|
| ![Original](images/zoom5.jpg) | ![Removed](images/ver_1.jpg) | ![Replaced](images/ver_1_bg.jpg) |

---

## ⚙️ Installation & Requirements

```bash
pip install tensorflow keras numpy matplotlib opencv-python
```

Run the notebook on **Google Colab** (recommended for GPU acceleration).

---

## 🚀 Usage

1. Upload the notebook to Google Colab or Jupyter Notebook.
2. Connect to runtime and install dependencies.
3. Train the U-Net model using sample dataset.
4. Run background replacement on test images.

---

## 👥 Project Members

| Name                | Student ID |
| ------------------- | ---------- |
| Doan Ngoc Mai       | 21127104   |
| Le Nguyen Kieu Oanh | 21127129   |

---

## 📖 References

* [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)
* TensorFlow & Keras Documentation

---

## 📜 License

```
MIT License

Copyright (c) 2025 Doan Ngoc Mai and Le Nguyen Kieu Oanh
```
