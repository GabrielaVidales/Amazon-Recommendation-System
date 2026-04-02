# 🛒 Amazon Recommendation System: Applied AI Project

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-data--analysis-150458.svg)](https://pandas.pydata.org/)
[![Scikit-Surprise](https://img.shields.io/badge/recommender-systems-orange.svg)]()
[![MIT Program](https://img.shields.io/badge/MIT-Applied%20AI%20Program-red.svg)]()

---

## 📋 Project Overview

This project was developed as part of the **MIT Professional Education – Applied AI & Data Science Program**, specifically within the **Elective Project: Recommendation Systems**.

The objective is to design, implement, and evaluate multiple recommendation system approaches using an Amazon product ratings dataset.

---

## 🎯 Objective

To build a recommendation system capable of suggesting relevant products while addressing:

- Data sparsity  
- Popularity bias  
- Cold-start problem  

---

## 📊 Dataset

| Feature | Description |
|--------|------------|
| `user_id` | Unique user identifier |
| `prod_id` | Unique product identifier |
| `rating` | Rating (1–5) |
| `timestamp` | Not used |

🔗 Dataset:  
👉 https://drive.google.com/file/d/1XahZcR287ke7j48I7-oj0KzmmwSSvA3Y/view

---

## 🧹 Data Preprocessing

- Users ≥ 50 ratings  
- Products ≥ 5 ratings  

➡️ Reduced sparsity and improved reliability

---

## 🔍 Exploratory Data Analysis

### ⭐ Rating Distribution
![Rating Distribution](images/Distribution%20of%20Product%20Ratings.png)

### 👤 User Activity
![User Activity](images/User%20Activity%20Distribution.png)

### 📦 Item Popularity
![Item Popularity](images/Item%20Popularity%20Distribution.png)

### 📉 Long Tail Distribution
![Long Tail](images/Long%20Tail%20Distribution%20of%20Products.png)

### 🔝 Top Users
![Top Users](images/Top%2010%20Users%20by%20Number%20of%20Ratings.png)

---

## 🤖 Models Implemented

### 📌 Rank-Based Model
- Non-personalized baseline  

### 👥 User-User Collaborative Filtering
- Cosine similarity  
- Personalized  

### 📦 Item-Item Collaborative Filtering
- More stable than user-user  

### 🧮 Matrix Factorization (SVD)
- Handles sparsity effectively  
- Best performance  

---

## 📈 Model Comparison

| Model           | RMSE | Precision | Recall | F1 |
|----------------|------|----------|--------|----|
| UU Baseline    | 1.001 | 0.855 | 0.867 | 0.861 |
| UU Optimized   | 0.953 | 0.847 | 0.894 | 0.870 |
| II Baseline    | 0.995 | 0.851 | 0.870 | 0.860 |
| II Optimized   | 0.958 | 0.839 | 0.880 | 0.859 |
| SVD Baseline   | 0.888 | 0.853 | 0.880 | 0.866 |
| SVD Optimized  | **0.882** | **0.860** | **0.900** | **0.879** |

---

## 📊 Model Performance Visualization

### 🔥 Heatmap
![Heatmap](images/Model%20Performance%20Heatmap%20(Green%20=%20Better).png)

### 📊 Precision & Recall
![Precision Recall](images/Precision@10%20and%20Recall@10%20—%20All%20Models.png)

### 📉 RMSE Comparison
![RMSE](images/RMSE%20Comparison%20—%20All%20Models.png)

---

## 📊 Prediction Analysis

### 📉 Error Distribution (All Models)
![Errors](images/Prediction%20Error%20Distributions%20—%20Model%20Comparison.png)

### 📍 SVD Predictions
![SVD](images/Actual%20vs%20Predicted%20Ratings%20—%20SVD%20Models.png)

### 📍 User-User Predictions
![UU](images/Actual%20vs%20Predicted%20Ratings%20(User-User%20Baseline).png)

### 📊 Error (User-User)
![UU Error](images/Distribution%20of%20Prediction%20Errors%20—%20User-User%20Baseline.png)

---

## 📍 Recommendation Behavior

![Scatter](images/Recommended%20Items%20in%20Rating–Popularity%20Space.png)

---

## ⚠️ Key Challenges

- High sparsity (~99%)  
- Popularity bias  
- Cold-start problem  

---

## 🏆 Key Results

- Rank-based model provides a strong baseline  
- KNN improves personalization but struggles with sparsity  
- Item-item is more stable  
- SVD achieves the best overall performance  

---

## 📌 Conclusion

Matrix factorization (SVD) provides the best balance between:

- Accuracy  
- Robustness  
- Scalability  

---

## 🛠️ Technologies

- Python  
- Pandas / NumPy  
- Matplotlib / Seaborn  
- Scikit-surprise  

---

## 🌟 Highlights

- End-to-end recommendation system pipeline  
- Advanced EDA  
- Model comparison  
- Hyperparameter tuning  
- Visual evaluation  

---

## 👨‍💻 Author

Developed as part of the  
**MIT Professional Education – Applied AI & Data Science Program**

---

## 📄 License

Educational use only
