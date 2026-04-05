# Sentiment Analysis on Product Reviews

## Problem Statement

This project aims to classify customer reviews into **Positive, Neutral, or Negative sentiment** using Natural Language Processing (NLP) techniques.

---

##  Dataset

* Flipkart Product Reviews dataset
* Features:

  * Review (text)
  * Rating (1–5)

---

##  Approach

### 1. Data Cleaning

* Converted ratings to numeric
* Handled missing values

### 2. Sentiment Creation

* Rating ≥ 4 → Positive
* Rating = 3 → Neutral
* Rating ≤ 2 → Negative

### 3. Text Preprocessing

* Lowercasing
* Removing special characters
* Tokenization
* Stopword removal

### 4. Feature Engineering

* TF-IDF Vectorization
* Used **n-grams (1,2)** for improvement

### 5. Model Building

* Logistic Regression
* Random Forest (for comparison)

### 6. Evaluation Metrics

* Accuracy
* Precision, Recall, F1-score
* Confusion Matrix

---

## Results

* Accuracy: ~95%
* Strong performance for Positive class
* Lower recall for Neutral and Negative classes

---

##  Key Observations

* Model is biased toward Positive class due to class imbalance
* n-grams improved context understanding but did not significantly improve minority class performance

---

## Future Improvements

* Handle class imbalance (SMOTE / class weights)
* Try advanced models (XGBoost, BERT)
* Use deep learning techniques

---

##  Use Cases

* Customer feedback analysis
* Product review monitoring
* Social media sentiment tracking

