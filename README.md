# 🍬 Multi-class Diabetes Classification (SVM)

## 📖 Project Overview
This project applies **Support Vector Machine (SVM)** to classify patients into different diabetes categories using a **multiclass dataset**.  
The aim is to build and evaluate SVM models with different **hyperparameters** (C, gamma, kernel) and compare their performance.

---

## 📂 Dataset
- **Source**: [Kaggle - Multiclass Diabetes Dataset](https://www.kaggle.com/datasets/whenamancodes/multiclass-diabetes-dataset)  
- **File Used**: `Multiclass Diabetes Dataset.csv`  
- **Target Variable**: `Class` (renamed to `target`)  
  - `0` → Class 0  
  - `1` → Class 1  
  - `2` → Class 2  

---

## 🛠️ Tools & Libraries
- **Python** 🐍  
- **Pandas & NumPy** → Data handling  
- **Matplotlib** → Data visualization (scatter plots)  
- **Scikit-learn** → SVM models, train/test split  

---

## ⚙️ Steps Performed
1. **Load Dataset** and checked for missing values.  
2. **Preprocessing**:
   - Renamed `Class` column → `target`.  
   - Split features (`x`) and target (`y`).  
3. **Visualization**:
   - Scatter plot of `Gender` vs `AGE` for different diabetes classes.  
4. **Train/Test Split**:
   - 70% training, 30% testing.  
5. **Model Training & Evaluation**:
   - Built baseline **SVM** model.  
   - Evaluated training & test accuracy.  
6. **Hyperparameter Tuning**:
   - **Regularization (C):**
     - `C=0.1` → Accuracy: 50%  
     - `C=1` → Accuracy: 76.25%  
     - `C=1000` → Accuracy: 91.25%  
   - **Gamma:**
     - `gamma=0.1` → Accuracy: 67.5%  
     - `gamma=1` → Accuracy: 52.5%  
     - `gamma=1000` → Accuracy: 50%  
   - **Kernel:**
     - `linear` → Accuracy: **92.5%** ✅  
     - `rbf` → Accuracy: 76.25%  

---

## 📊 Results
- The **best model** achieved **92.5% accuracy** using:
  - **Kernel:** Linear  
  - **C:** High regularization value (`C=1000`)  
- Hyperparameter choice (C, gamma, kernel) significantly affects model performance.  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/mennaabdalazizyahia/multiclass-diabetes-svm.git
   cd multiclass-diabetes-svm
