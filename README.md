# Breast-Cancer-Prediction-with-PyTorch
This repository contains a complete, from-scratch implementation of a binary classification model built using **PyTorch tensors only**—without using `torch.nn`, `torch.optim`.

The goal is to classify breast tumors as **benign (0)** or **malignant (1)** using the Breast Cancer Wisconsin dataset while learning how neural networks work under the hood.

---

## 📊 Dataset Information
The project uses **Breast_cancer_data.csv**, which contains clinical features extracted from fine-needle aspirate (FNA) images of breast masses.

### **Dataset Summary**
- **Total samples:** 569  
- **Features:** 30 numerical features  
- **Target:** Diagnosis (Benign = 0, Malignant = 1)  
- **Type:** Binary classification  
- **Input format:** Clean numeric dataset  

---

## **Preprocessing Steps**

Inside the notebook:
- Removed unnecessary columns (`id`, `Unnamed: 32`)
- Encoded diagnosis:  
  - `M` → 1  
  - `B` → 0  
- Standardized all features via `StandardScaler`
- Train/test split: **80% training, 20% testing**
- Converted all arrays into PyTorch tensors

---

## 🧠 Model Description

The model is a **single neuron (logistic regression)** implemented completely manually.


### **Key Components**
- **Weights:** initialized randomly  
- **Bias:** initialized as zero  
- **Activation:** Sigmoid  
- **Loss:** Custom Binary Cross-Entropy (BCE)  
- **Training:** Manual Gradient Descent  
- **Autograd:** Used only to compute gradients

---

## Requirements

- Python 3.x
- PyTorch
- NumPy
- pandas
- scikit-learn
- Jupyter Notebook

---

##  Author
**Siddharth Jain**  
[LinkedIn](https://www.linkedin.com/in/siddharth-jain-979a35253/)
