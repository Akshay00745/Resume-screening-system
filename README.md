# 📄 Resume Screening System using NLP & Machine Learning

## 📌 Project Overview

This project builds an intelligent Resume Screening System that automatically classifies resumes into job categories using Natural Language Processing (NLP) and Machine Learning.

The goal is to help HR teams and recruiters quickly shortlist resumes based on job roles, reducing manual effort and improving hiring efficiency.

---

## 📂 Dataset Description

The dataset contains:

- `Resume_str` → Raw resume text
- `Category` → Job category label (24 different job domains)

Total resumes: ~2500  
Number of categories: 24  

Some categories include:
- INFORMATION-TECHNOLOGY
- BUSINESS-DEVELOPMENT
- FINANCE
- ENGINEERING
- HR
- AVIATION
- SALES
- HEALTHCARE
- etc.

---

## 🔍 Exploratory Data Analysis (EDA)

### 1️⃣ Category Distribution
- Dataset is relatively balanced across 24 job categories.
- Most frequent categories:
  - Information Technology
  - Business Development
  - Finance
  - Advocate
  - Accountant

### 2️⃣ Resume Length Distribution
- Most resumes fall between **3000–6000 characters**
- Some outliers exceed 20,000+ characters
- Slight right-skewed distribution

### 3️⃣ Most Frequent Words in Resumes
Common terms found:
- state
- city
- company
- management
- skills
- experience
- project
- development
- marketing

This indicates resumes commonly focus on:
✔ Skills  
✔ Experience  
✔ Management  
✔ Project work  

---

## ⚙️ Data Preprocessing

- Converted text to lowercase
- Removed punctuation
- Removed stopwords
- Applied TF-IDF Vectorization
- Label Encoding of categories
- Train-Test split (80/20)

---

## 🤖 Models Used

### 1️⃣ Naive Bayes
Accuracy: **55.9%**

### 2️⃣ Logistic Regression
Accuracy: **64.7%**

Logistic Regression performed better due to:
- Multi-class handling
- Better separation in TF-IDF space

---

## 📊 Model Evaluation (Logistic Regression)

Overall Accuracy: **56% (classification report sample split)**

- Some categories perform well (precision > 0.80)
- Some categories underperform due to:
  - Similar vocabulary across roles
  - Limited sample size per category

Macro Avg F1 Score: 0.48  
Weighted Avg F1 Score: 0.54  

This indicates room for improvement with:
- Hyperparameter tuning
- More data
- Advanced models (SVM, XGBoost, BERT)

---

---

## 🚀 Future Improvements

- Use Word2Vec / FastText embeddings
- Try Support Vector Machine (SVM)
- Use deep learning (LSTM / BERT)
- Deploy using Streamlit
- Add confidence score to predictions

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- NLP (TF-IDF)

---

## 🎯 Business Impact

This system can:

✔ Automate resume shortlisting  
✔ Reduce HR screening time  
✔ Improve hiring efficiency  
✔ Maintain unbiased filtering  

---

## 📌 Conclusion

The Resume Screening System demonstrates how NLP and Machine Learning can be applied to real-world HR automation problems.

Although baseline accuracy is moderate, this project provides a strong foundation for building AI-powered recruitment tools.

---

⭐ Part of my 30 Days Data Science Challenge
