---
# 🔢 Chapter 3 – Classification

This notebook is based on **Hands-On Machine Learning (3rd Edition), Chapter 3**.
The goal of this project is to dive deep into **classification tasks** using the **MNIST dataset**, and to explore key concepts such as **binary/multiclass classification, performance metrics, precision-recall trade-off, ROC curves, multilabel and multioutput classification**.

---

## 📚 Steps in the Notebook

### 1. Import Libraries

* `numpy`, `pandas` → data handling
* `matplotlib` → visualization
* `scikit-learn` → models, performance metrics, validation utilities

### 2. Working with the MNIST Dataset

* Loaded the **MNIST dataset** of **70,000 images of handwritten digits (0–9)**.
* Each image: **28×28 pixels**, flattened into a **784-dimensional vector**.
* Visualized digits with `matplotlib` to understand the dataset.

### 3. Training a Binary Classifier

* Simplified the problem to detect only the digit **“5” vs not-5**.
* Created binary labels (`y_train_5`, `y_test_5`).
* Trained a **Stochastic Gradient Descent (SGD) Classifier**.
* Noted that SGD is well-suited for **large datasets** and **online learning**.

### 4. Performance Measurement

* Evaluated classifiers using:

  * **Accuracy** → misleading with imbalanced datasets.
  * **Cross-validation** (`cross_val_score`, `cross_val_predict`) for robust evaluation.
  * **Confusion Matrix** to analyze true/false positives & negatives.

### 5. Precision & Recall

* Defined and calculated **Precision**, **Recall**, and **F1-Score**.
* Learned that **precision ≠ recall**:

  * Precision = correct positive predictions out of all predicted positives.
  * Recall = correct positive predictions out of all actual positives.
* Visualized the **Precision/Recall Trade-off** by adjusting decision thresholds.

### 6. Precision-Recall Trade-off & Decision Thresholds

* Explored how **raising thresholds increases precision but lowers recall**, and vice versa.
* Implemented decision score extraction using `decision_function`.
* Plotted **Precision vs Recall curves** for analysis.

### 7. ROC Curve & AUC

* Plotted the **ROC curve** (True Positive Rate vs False Positive Rate).
* Compared classifiers using **AUC (Area Under Curve)**.
* Understood the trade-off between **sensitivity and specificity**.

### 8. Multiclass Classification

* Extended binary classifiers to handle **multiple classes (0–9 digits)**.
* Explored strategies:

  * **One-vs-All (OvA)**
  * **One-vs-One (OvO)**
* Used **Random Forest** and **SVM** as multiclass classifiers.

### 9. Error Analysis

* Analyzed confusion matrices for multiclass predictions.
* Visualized common misclassifications (e.g., 8 vs 9, 3 vs 5).
* Learned how **error analysis helps guide feature engineering**.

### 10. Multilabel Classification

* Explored **multi-output prediction tasks**:

  * Example: classifying whether a digit is **large/small** AND **odd/even** at the same time.
* Learned how Scikit-Learn supports multilabel outputs.

### 11. Multioutput Classification

* Extended multilabel tasks to **multioutput classification**: predicting multiple labels per instance with multiple classes.
* Example: image denoising → input = noisy digit image, output = clean digit image.

---

## 📖 Key Learnings

* ✅ Difference between **binary, multiclass, multilabel, and multioutput classification**.
* ✅ How to **train and evaluate binary classifiers** with SGD.
* ✅ Why **accuracy can be misleading** and when to use precision/recall/F1 instead.
* ✅ The **precision-recall trade-off** and how thresholds affect results.
* ✅ How to interpret and use the **ROC curve & AUC**.
* ✅ Techniques for **multiclass classification** (OvA vs OvO).
* ✅ How to perform **error analysis** with confusion matrices and visualization.
* ✅ Real-world value of **multilabel and multioutput classification**.

---

## ⚙️ Requirements

Install the dependencies before running the notebook:

```bash
pip install numpy pandas matplotlib scikit-learn
```

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/USERNAME/HandsOnML-Projects.git
cd HandsOnML-Projects/chapter3
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook chapter3.ipynb
```

---

## 📊 Results

* Successfully built a **binary classifier** to detect digit “5”.
* Explored multiple performance metrics beyond accuracy.
* Understood the **precision-recall trade-off** and ROC-AUC evaluation.
* Extended classification to **multiclass, multilabel, and multioutput problems**.
* Gained insights on **error analysis** and how misclassifications reveal model weaknesses.

---

👉 This chapter was all about **evaluating classifiers properly** and understanding how different classification setups (binary, multiclass, multilabel, multioutput) work in real ML workflows.

---
