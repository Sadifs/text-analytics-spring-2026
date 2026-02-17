# Assignment 1 – Sentiment Analysis

**Course:** Text Mining & Social Media Analytics  
**Semester:** Spring 2026  
**Instructor:** Dr. Ace Vo  
**Student:** Sadaf Sarbazi  

---

## Project Overview

This assignment applies sentiment analysis techniques to real-world text data using three pretrained approaches: VADER, TextBlob, and a Transformer-based model. The objective is to compare these models in terms of performance, interpretability, and limitations, and to evaluate their suitability for different text analytics scenarios.

The project emphasizes both technical execution and critical evaluation of model behavior, along with transparent documentation of AI-assisted development.

---

## Dataset Description

- **Dataset:** IMDB 50K Movie Reviews  
- **Source:** Kaggle  
  https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews  
- **Text Type:** Long-form movie reviews  
- **Original Labels:** Positive / Negative  

**Rationale for dataset selection:**  
The IMDB dataset provides a balanced and well-studied benchmark for sentiment analysis. Its review length and expressive language make it suitable for evaluating differences between rule-based, statistical, and transformer-based sentiment models.

---

## Methodology Overview

The analysis follows the structured pipeline specified in the assignment instructions:

1. Data loading and exploratory analysis  
2. Text cleaning and preprocessing with validation examples  
3. Model-specific tokenization and feature handling  
4. Sentiment inference using VADER, TextBlob, and a Transformer model  
5. Manual labeling of a 100-review sample to establish ground truth  
6. Quantitative and qualitative comparison of model performance  

---

## Key Findings Summary

- **VADER** performed best on expressive reviews and handled capitalization and punctuation effectively.  
- **TextBlob** handled simple negation reasonably well but showed less consistency across samples.  
- **The Transformer model** captured richer emotional nuance but required additional processing to map emotion outputs to sentiment categories and incurred higher computational cost.  

Overall, model effectiveness depends on text length, domain, and performance constraints.

---

## Results and Visualizations

The notebook includes the following results and visual outputs:

- Text length distribution histogram during exploratory analysis  
- Comparison of sentiment label distributions across models  
- Accuracy comparison table based on the manually labeled 100-review sample  
- Success and failure case examples for each model  

All visualizations are embedded directly in the notebook output cells.

---

## How to Run

1. Open the main notebook: **[Sentiment Analysis Notebook](Anotebooks/Sentiment_Analysis.ipynb)**
2. Ensure the following Python libraries are installed:
- pandas, numpy  
- nltk  
- textblob  
- transformers  
- torch  
- matplotlib, seaborn  
3. Run the notebook cells sequentially from top to bottom.
