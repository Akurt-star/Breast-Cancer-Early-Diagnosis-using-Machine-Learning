# Breast Cancer Early Diagnosis using Machine Learning

This project focuses on **early diagnosis of breast cancer** using the **Breast Cancer Wisconsin (Diagnostic) dataset**. The aim is to classify tumors as **Malignant (M)** or **Benign (B)** based on various cell nucleus features extracted from digitized images.

---

## 📌 Project Overview
Breast cancer is one of the most common cancers among women, and early diagnosis plays a crucial role in successful treatment.  
This project uses **Machine Learning algorithms** to predict whether a tumor is benign or malignant by analyzing 30 numeric features related to cell nuclei characteristics.

**Key Features of the Dataset:**
- 30 numeric features describing tumor properties:
  - `radius`, `texture`, `perimeter`, `area`, `smoothness`, `compactness`, `concavity`, `concave points`, `symmetry`, `fractal dimension`
- Each property has three forms: `mean`, `se` (standard error), and `worst`.
- **Target variable:** `diagnosis` → `M` (Malignant) or `B` (Benign)
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

---

## 🛠️ Techniques & Algorithms
The following classification models were implemented and compared:
- **Logistic Regression**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **XGBoost**
- **Neural Network**

**Evaluation Metrics:**
- **Accuracy**
- **F1 Score** (chosen as primary metric due to medical importance of both precision and recall)
- 5-fold Cross-Validation for reliable results.

---

## 📊 Results
| Model              | Accuracy | F1 Score |
|---------------------|----------|----------|
| Logistic Regression | 0.9737   | 0.9647   |
| Random Forest       | 0.9524   | 0.9649   |
| SVM                 | 0.9647   | 0.9737   |
| XGBoost             | 0.9737   | 0.9649   |
| Neural Network      | 0.9719   | 0.9625   |

**Best Performer:**  
✅ **SVM** achieved the highest **F1 Score (0.9737)**, making it the most effective model for this dataset.

## 🔍 Notes

- Dataset is not included in this repository due to size and licensing. Download it from UCI Repository.
- This work was developed as part of BENG101: Fundamentals of Bioengineering course at Gebze Technical University (Spring 2025).
- Full report is not shared here, only the implementation and summary are provided.
