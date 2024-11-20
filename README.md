# Chronic Kidney Disease Prediction Using Machine Learning  

This project predicts **Chronic Kidney Disease (CKD)** using machine learning techniques. It implements **K-Nearest Neighbors (KNN)** and **Decision Tree** classifiers to analyze patient health data and determine the likelihood of CKD. The goal is to develop a predictive model that can assist in early diagnosis, enabling timely medical interventions.  

---

## 🚀 Project Overview  
Chronic Kidney Disease is a progressive condition affecting kidney function. Early detection is crucial to prevent complications. This project uses patient health records to train machine learning models that classify individuals into two categories:  
- **0:** CKD detected  
- **1:** No CKD  

The pipeline includes data preprocessing, feature scaling, and the application of classification algorithms to predict CKD.  

---

## 📂 Dataset  
The dataset contains **400 patient records** with **25 attributes**, including:  
- Age  
- Blood Pressure (BP)  
- Specific Gravity (SG)  
- Hemoglobin (HB)  
- Blood Glucose Random (BGR)  
- Red Blood Cell Count (RBC)  
- White Blood Cell Count (WBCC)  
- Target variable: `class` (0 for CKD, 1 for no CKD)  

---

## 🔧 Data Preprocessing  
1. **Handling Missing Values:**  
   - Missing values (`?`) were replaced using the KNN imputation method.  
2. **Feature Scaling:**  
   - Standardized all numerical features using `StandardScaler` for better algorithm performance.  
3. **Encoding Target Variable:**  
   - The `class` column was encoded as 0 (CKD) and 1 (no CKD) using label encoding.  

---

## 🧠 Machine Learning Models  
### 1. K-Nearest Neighbors (KNN):  
- **Description:** A non-parametric algorithm that classifies instances based on the majority class of their nearest neighbors.  
- **Reason for Use:**  
   - Effective for small datasets.  
   - Suitable for non-linear decision boundaries.  

### 2. Decision Tree:  
- **Description:** A tree-based model that splits data based on feature thresholds to make predictions.  
- **Reason for Use:**  
   - Provides interpretable and visualizable decision-making.  
   - Handles numerical and categorical features effectively.  

---

## 🧪 Model Evaluation  
The dataset was split into **50% training** and **50% testing** sets. The models were evaluated using:  
- **Accuracy:** Overall correctness of predictions.  
- **Precision:** Percentage of correctly predicted positive cases.  
- **Recall:** Percentage of actual positives correctly identified.  
- **F1-Score:** Harmonic mean of precision and recall.  

### Results:  
| Metric          | KNN       | Decision Tree |  
|------------------|-----------|---------------|  
| **Accuracy**     | 78.75%    | 75.00%        |  
| **Precision**    | 85.71%    | 81.25%        |  
| **Recall**       | 76.60%    | 72.22%        |  
| **F1-Score**     | 80.90%    | 76.47%        |  

---

## 📊 Visualizations  
- A **bar chart** shows the distribution of CKD and non-CKD patients.  
- **Confusion matrix heatmaps** illustrate correct and incorrect predictions for both models.  

---

## 💡 Challenges and Future Work  
### Challenges:  
- Handling missing data efficiently.  
- Addressing class imbalance in the dataset.  

### Future Work:  
- Implement other algorithms like **Random Forest** and **SVM** for comparison.  
- Use oversampling techniques like **SMOTE** to handle class imbalance.  
- Incorporate larger and more diverse datasets to improve model generalization.  

---

## 🛠️ Tools and Libraries  
- **Programming Language:** Python  
- **Libraries Used:**  
  - Pandas  
  - NumPy  
  - scikit-learn  
  - seaborn  
  - Matplotlib
