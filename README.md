# Breast-Cancer-Classification-using-Support-Vector-Machine

This project aims to classify breast tumors as **benign** or **malignant** using **Support Vector Machine (SVM)** models. It leverages the **Breast Cancer Wisconsin Diagnostic Dataset** and includes detailed data analysis, preprocessing, visualization, model training, and evaluation.

---

## 📌 Objectives

- Perform **Exploratory Data Analysis (EDA)** to understand feature importance.
- Train and evaluate **SVM models** using both **Linear** and **RBF kernels**.
- Use **GridSearchCV** to optimize SVM hyperparameters.
- Visualize decision boundaries using **PCA**.
- Evaluate models with **confusion matrix, ROC curves, and classification reports**.

---

## 📊 Dataset

- **Source**: (https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)
- **Instances**: 569
- **Features**: 30 numeric features + 1 target (`diagnosis`)
  - `1` = Malignant
  - `0` = Benign

---

## 🔧 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Google Colab

---

## 📈 Key Steps

### ✔️ Data Preprocessing
- Label encoding of target
- Feature scaling using `StandardScaler`
- Dimensionality reduction with `PCA` for visualization

### ✔️ EDA & Visualization
- Correlation heatmaps
- KDE plots, violin plots, boxen plots
- PCA scatter plots
- ROC Curve for model comparison

### ✔️ Model Training & Evaluation
- **SVM with Linear Kernel**
  - Accuracy: **96.49%**
  - F1-score (Malignant): **0.95**
- **SVM with RBF Kernel**
  - Accuracy: **95.91%**
  - F1-score (Malignant): **0.94**
- **Optimized RBF SVM** (via GridSearchCV)
  - Accuracy: **95.32%**
  - Best Parameters: `C=1`, `gamma=0.01`

---

## 📊 Results Summary

| Model         | Accuracy | Precision (1) | Recall (1) | F1-Score (1) |
|---------------|----------|----------------|------------|--------------|
| Linear SVM    | 96.49%   | 1.00           | 0.91       | 0.95         |
| RBF SVM       | 95.91%   | 1.00           | 0.89       | 0.94         |
| RBF SVM (Tuned) | 95.32% | 1.00           | 0.88       | 0.93         |

---

## 📌 Conclusion

This project demonstrates that **SVM models are highly effective** in classifying breast cancer, with Linear SVM slightly outperforming in terms of accuracy and recall. Visualizations and PCA analysis confirm that the data is well-separated and suitable for SVM classification.

---

## 🙋‍♂️ Author

**Siddardha Shayini**  

---
