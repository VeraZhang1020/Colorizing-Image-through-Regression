# Image Colorization using Machine Learning and Deep Learning

## 📌 Project Overview
This project focuses on building models to automatically colorize grayscale images. The goal is to reconstruct realistic color information from single-channel images using both traditional machine learning and deep learning approaches.

Due to the large size of the original ImageNet dataset, we use the Tiny ImageNet dataset from Kaggle as a manageable subset for training and evaluation.

---

## 📊 Data
- Dataset: Tiny ImageNet (Kaggle)
- Contains a subset of ImageNet images across multiple categories
- Images are preprocessed into:
  - Grayscale input (1 channel)
  - RGB output (3 channels)

---

## 🛠 Methods

### 1. Baseline Models
- **Linear Regression (Gradient Descent)**
- **Support Vector Regression (SVR)**

### 2. Neural Network Models
- **Baseline Neural Network**
  - Fully connected layers
  - Learns pixel-wise color mapping

- **U-Net Architecture**
  - Encoder-decoder structure
  - Captures spatial features for improved color reconstruction

---

## ⚙️ Model Training
- Framework: PyTorch
- Loss Functions:
  - Mean Squared Error (MSE)
  - L1 Loss (in some experiments)
- Input:
  - Grayscale images
- Output:
  - Predicted RGB images

---

## 📈 Results
- Baseline models provide limited color reconstruction
- Neural networks significantly improve results
- **U-Net produces the most realistic and spatially consistent colorizations**

---

## 💡 Key Insights
- Pixel-wise regression is insufficient for complex image tasks
- Deep learning models capture spatial and contextual information better
- U-Net is highly effective for image-to-image translation tasks

---

## 🔗 Tools & Technologies
- Python
- PyTorch
- NumPy
- Matplotlib
- Scikit-learn

---

## 📁 Project Structure
- `AML25_GroupE_Combined_Notebook_1209_v1.ipynb` → Main notebook
- Data preprocessing → grayscale + RGB conversion
- Model training and evaluation included in notebook

## 📓 Notebook

The notebook contains rich visual outputs and may not render directly on GitHub.

- 👉 [View on GitHub](https://github.com/VeraZhang1020/Colorizing-Image-through-Regression/blob/main/AML25_GroupE_Combined_Notebook_1209_v1.ipynb)
- 👉 [View via nbviewer](https://nbviewer.org/github/VeraZhang1020/Colorizing-Image-through-Regression/blob/main/AML25_GroupE_Combined_Notebook_1209_v1.ipynb)
- 👉 [Download Notebook](./AML25_GroupE_Combined_Notebook_1209_v1.ipynb)

---

## 🚀 Future Work
- Improve perceptual quality using advanced loss functions (e.g., perceptual loss)
- Apply GAN-based models for more realistic colorization
- Scale to larger datasets for improved generalization
