# 🍷 Wine Quality Prediction — Machine Learning Project

## 📋 Project Overview
This project aims to **predict wine quality** based on its physicochemical properties using **machine learning techniques**.  
We explore multiple models, apply clustering for segmentation, and finally deploy an optimized **Stacking Classifier** for production.

Dataset used: [UCI Wine Quality - Red Wine](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv)

---

## 🧠 Objectives
- Explore and clean the dataset  
- Perform feature scaling and clustering (Agglomerative & KMeans)  
- Build and evaluate multiple ML models for classification  
- Implement a **Stacking Ensemble** combining Logistic Regression, Gradient Boosting, and SVM  
- Select and save the best-performing model for deployment  

---

## 📊 Dataset Description
**File:** `winequality-red.csv`  
**Samples:** 1599  
**Features:** 11 chemical properties + 1 target variable (`quality`)

| Feature | Description |
|----------|--------------|
| fixed acidity | concentration of nonvolatile acids |
| volatile acidity | concentration of acetic acid |
| citric acid | fixed acid enhancing freshness |
| residual sugar | amount of sugar left after fermentation |
| chlorides | salt content |
| free sulfur dioxide | SO₂ that prevents microbial growth |
| total sulfur dioxide | total SO₂ content |
| density | density of the wine |
| pH | acidity level |
| sulphates | wine stabilization agent |
| alcohol | percentage of alcohol |
| quality | sensory score (0–10) |


## 🔍 Methods and Models

### 🧩 Clustering
- **Agglomerative Hierarchical Clustering (AHC)** using *Manhattan distance*  
- **KMeans (k=2)** for comparison  
- Visualized dendrogram and confusion matrix between clustering methods  

### 🤖 Classification Models
| Model | Description |
|--------|-------------|
| Logistic Regression | Simple, interpretable baseline |
| Gradient Boosting Classifier | Powerful tree-based ensemble |
| SVM (RBF kernel) | Captures non-linear relationships |
| **Stacking Classifier** | Combines all models using Logistic Regression as meta-learner |

---

## 🏆 Model Performance

| Metric | Score |
|--------|--------|
| **Accuracy** | **0.9937** |
| Precision | 0.99 |
| Recall | 1.00 / 0.95 |
| F1-Score | 0.99 |
| Macro Avg | 0.99 |

✅ The **Stacking Classifier** outperformed all base models and was selected for deployment.




