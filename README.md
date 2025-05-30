## 📌 Task 4: AI & ML Internship Assignment
# Breast Cancer Diagnosis — Logistic Regression

🏥 **Objective:**  
Build and evaluate a logistic regression model to classify breast cancer diagnosis as malignant or benign using a medical dataset.

---

## Dataset

- Breast Cancer Diagnosis Dataset (`data.csv`)  
- The target variable `diagnosis` is categorical:  
  - `M` (Malignant) mapped to 1  
  - `B` (Benign) mapped to 0  
- Contains multiple numeric features extracted from digitized images of breast masses.  
- Irrelevant columns such as `id` and `Unnamed: 32` are removed during preprocessing.

---

## Tools Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## Steps Performed

1. **Data Exploration & Cleaning**  
   - Loaded dataset and checked for missing values  
   - Dropped unnecessary columns  

2. **Feature and Target Selection**  
   - Separated feature variables (`X`) and target (`y`)  

3. **Train-Test Split**  
   - Split data into 80% training and 20% testing sets  

4. **Data Preprocessing**  
   - Imputed missing values using mean strategy  
   - Standardized features using `StandardScaler`  

5. **Model Training**  
   - Trained Logistic Regression model on training data  

6. **Model Evaluation**  
   - Generated confusion matrix  
   - Produced classification report (precision, recall, F1-score)  
   - Calculated ROC-AUC score  

7. **Threshold Tuning & Visualization**  
   - Plotted ROC curve  
   - Tested custom classification threshold (0.6)  
   - Visualized confusion matrix heatmaps  

8. **Sigmoid Function Plot**  
   - Plotted sigmoid function to understand logistic regression decision boundary  

---

## Results

### Classification Report:

| Class | Precision | Recall | F1-score | Support |
|-------|-----------|--------|----------|---------|
| 0 (Benign) | 0.97 | 0.99 | 0.98 | 71 |
| 1 (Malignant) | 0.98 | 0.95 | 0.96 | 43 |

- **Accuracy:** 0.97  
- **Macro Average:** Precision=0.97, Recall=0.97, F1-score=0.97  
- **Weighted Average:** Precision=0.97, Recall=0.97, F1-score=0.97  

### ROC-AUC Score:  
**0.9974** (Excellent classification capability)

### Confusion Matrix (Threshold = 0.6):

|          | Predicted 0 | Predicted 1 |
|----------|-------------|-------------|
| Actual 0 | 71          | 0           |
| Actual 1 | 2           | 41          |

---

## Visualizations

- Confusion matrix heatmap  
- ROC curve with AUC  
- Sigmoid function plot  

---

## Key Learnings

- Implementation of logistic regression for binary classification  
- Importance of data preprocessing: imputation and feature scaling  
- Evaluation using multiple metrics beyond accuracy  
- Understanding ROC curve and threshold tuning for real-world classification problems  
- Visualizing the logistic function for deeper model insight  

---
