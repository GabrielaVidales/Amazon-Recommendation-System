# 🛒 Amazon Recommendation System: Applied AI Project

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-data--analysis-150458.svg)](https://pandas.pydata.org/)
[![Scikit-Surprise](https://img.shields.io/badge/recommender-systems-orange.svg)]()
[![MIT Program](https://img.shields.io/badge/MIT-Applied%20AI%20Program-red.svg)]()

---

## 📋 Project Overview

This project was developed as part of the **MIT Professional Education – Applied AI & Data Science Program**, specifically within the **Elective Project: Recommendation Systems**.

The objective is to design, implement, and evaluate multiple recommendation system approaches using an Amazon product ratings dataset. The project demonstrates end-to-end data science skills, including data preprocessing, exploratory analysis, model development, evaluation, and interpretation.

---

## 🎯 Objective

To build a recommendation system capable of suggesting relevant products to users based on historical interactions, while addressing key challenges such as:

- Data sparsity  
- Popularity bias  
- Cold-start problem  

---

## 📊 Dataset

The dataset contains user-product interaction data with the following attributes:

| Feature | Description |
|--------|------------|
| `user_id` | Unique user identifier |
| `prod_id` | Unique product identifier |
| `rating` | Rating given by the user (1–5) |
| `timestamp` | Interaction time (not used) |

Due to its large size (~7.8 million records), filtering was applied.

### 🔗 Dataset Access

👉 [Download Dataset (Google Drive)](https://drive.google.com/file/d/1XahZcR287ke7j48I7-oj0KzmmwSSvA3Y/view?usp=sharing)

---

## 🧹 Data Preprocessing

To reduce sparsity and improve reliability:

- Removed users with fewer than **50 ratings**
- Removed products with fewer than **5 ratings**

This produced a more robust dataset for modeling.

---

## 🔍 Exploratory Data Analysis (EDA)

Key findings:

- Strong **positive bias** in ratings (dominance of 4–5 stars)
- Extremely **sparse user-item matrix (~99%)**
- Presence of **power users**
- Clear **long-tail distribution of products**
- Most items receive very few interactions

---

## 🤖 Models Implemented

### 📌 1. Rank-Based Recommendation
- Based on average rating and interaction thresholds
- Reliable but **non-personalized**
- Serves as baseline

---

### 👥 2. User-User Collaborative Filtering
- Similarity-based (KNN, cosine)
- Personalized recommendations
- Sensitive to sparsity

#### 🔧 Optimized Version
- Hyperparameter tuning (k, min_k, similarity)
- Improved Recall and F1-score

---

### 📦 3. Item-Item Collaborative Filtering
- Computes similarity between items
- More stable than user-user
- Better scalability

#### 🔧 Optimized Version
- GridSearchCV tuning
- Balanced performance improvements

---

### 🧮 4. Matrix Factorization (SVD)
- Learns latent factors (hidden features)
- Handles sparsity effectively
- Best RMSE performance

#### 🔧 Optimized Version
- Tuned parameters: `n_epochs`, `lr_all`, `reg_all`
- Best overall model

---

## 📈 Evaluation Metrics

- RMSE (Root Mean Squared Error)
- Precision@K
- Recall@K
- F1-score

---

## 📊 Visual Analysis

The project includes:

- Rating distributions  
- User activity analysis  
- Item popularity & long tail  
- Actual vs predicted ratings  
- Error distribution  
- Model behavior in rating–popularity space  

---

## ⚠️ Key Challenges

- High sparsity  
- Popularity bias  
- Cold-start problem  
- Limited user overlap  

---

## 🏆 Key Results

- Rank-based model provides a strong baseline  
- User-user improves personalization but struggles with sparsity  
- Item-item is more stable and scalable  
- SVD achieves the best performance overall  

---

## 📌 Conclusion

Matrix factorization (SVD) provides the most effective solution, balancing accuracy, robustness, and scalability in sparse environments.

---

## 🛠️ Technologies Used

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-surprise  


---

## 🚀 How to Use

1. Download dataset from the provided link  
2. Open the notebook or HTML file  
3. Run all cells sequentially  

---

## 🌟 Highlights

- End-to-end recommendation system pipeline  
- Advanced EDA (sparsity + long tail analysis)  
- Multiple model comparison  
- Hyperparameter tuning  
- Visual model evaluation  

---

## 👨‍💻 Author

Developed as part of the  
**MIT Professional Education – Applied AI & Data Science Program**

---

## 📄 License

This project is for educational purposes under the MIT Applied AI Program.
