# Assignment 2 — Text Classification

**Student:** Sadaf Sarbazi  
**Date:** Spring 2026  
**Dataset:** SASB-Aligned ESG Sentences  

---

## Overview

This project builds supervised machine learning models to classify ESG-related sentences into sustainability categories. The task is a **multiclass text classification problem**, where each sentence belongs to exactly one ESG category.

The goal is to compare multiple feature engineering approaches and machine learning algorithms to determine which model performs best for ESG sentence classification.

---

## Dataset Details

Dataset: **SASB-Aligned ESG Sentences**  
Source: https://www.kaggle.com/datasets/edwardjunprung/sasb-aligned-esg-sentences  

Dataset size: **6,460 sentences**

Target variable: **Parent Label**

Classes:

- Non-ESG  
- Environment  
- Human Capital  
- Social Capital  
- Business Model & Innovation  
- Leadership & Governance  

The dataset is **imbalanced**, with Non-ESG being the largest class and Business Model & Innovation being the smallest class.

---

## Best Model Results

Best model: **Tuned Logistic Regression + TF-IDF**

Performance on the test set:

| Metric | Score |
|------|------|
| Precision (weighted) | 0.7926 |
| Recall (weighted) | 0.7910 |
| F1 Score (weighted) | 0.7914 |

Training time: **~3–4 seconds**

The model exceeds the assignment performance requirement of **F1 ≥ 0.70**.

---

## Important Class

The smallest class in the dataset is **Business Model & Innovation**, so it was selected as the **important class**.

Rare classes are typically harder for models to predict accurately. Monitoring performance on this class helps ensure the model is not simply optimizing for the majority classes.

---

## Model Comparison

Models were compared using five criteria:

| Model | Features | Weighted F1 | Speed | Interpretability | Important Class Performance |
|------|------|------|------|------|------|
| Naive Bayes | CountVectorizer | Moderate | Very Fast | Medium | Lower |
| Logistic Regression | CountVectorizer | Good | Fast | High | Moderate |
| Logistic Regression (tuned) | TF-IDF | **Best (~0.79)** | Fast | High | Best overall |

Logistic Regression with TF-IDF provided the best balance of performance, speed, and interpretability.

---

## Custom Inference Summary

The final model was tested using **20 custom examples** designed to evaluate generalization.

Results:

**11 / 20 predictions matched the expected label (agreement rate = 0.55).**

Key findings:

- The model performs well on sentences that resemble ESG report language.
- Some errors occur between related ESG categories.
- Out-of-domain examples are more difficult for the model to classify correctly.

---

## Recommendation

The recommended model is **Tuned Logistic Regression with TF-IDF features**.

This model achieved the highest weighted F1 score while remaining computationally efficient and interpretable. Logistic Regression works well with sparse text features and allows inspection of model coefficients to understand which words influence predictions.

Although the model performs well on ESG-style language, additional training data could improve robustness and reduce errors on ambiguous or out-of-domain examples.

---

## Tools Used

- Python  
- Pandas  
- Scikit-learn  
- NLTK  
- Matplotlib  
- Seaborn  
- Jupyter Notebook
