# Assignment 1 – Sentiment Analysis

**Course:** Text Mining & Social Media Analytics  
**Semester:** Spring 2026  
**Instructor:** Dr. Ace Vo  
**Student:** Sadaf Sarbazi  

---

## Project Overview

This assignment examines sentiment analysis on real-world text data using three pretrained approaches:

- VADER  
- TextBlob  
- Transformer-based model (DistilBERT)

The goal is to compare these models in terms of accuracy, interpretability, speed, and limitations, and to evaluate their suitability for different text analytics scenarios. The project emphasizes both technical implementation and critical evaluation of model behavior.

All work is completed individually, with transparent documentation of AI assistance as required by the assignment.

---

## Dataset

- **Dataset:** IMDB 50K Movie Reviews  
- **Source:** Kaggle  
  https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews  
- **Text Type:** Long-form movie reviews  
- **Sentiment Labels:** Positive / Negative  

**Dataset justification:**  
The IMDB dataset is well suited for sentiment analysis due to its balanced labels and rich textual content, allowing for meaningful comparison of rule-based, statistical, and transformer-based sentiment models.

---

## Methodology

The analysis follows the structured pipeline specified in the assignment instructions:

1. **Data Loading and Exploration**
   - Dataset structure and metadata inspection  
   - Text length statistics and visualizations  
   - Initial observations of language patterns and noise  

2. **Text Cleaning and Preprocessing**
   - Removal of HTML tags, URLs, and special characters  
   - Lowercasing and whitespace normalization  
   - Explicit handling of contractions  
   - Before-and-after examples to validate cleaning decisions  

3. **Tokenization and Feature Handling**
   - Separate preprocessing pipelines tailored to each model  
   - Consideration of model-specific requirements  

4. **Sentiment Modeling**
   - VADER: rule-based sentiment scoring  
   - TextBlob: polarity and subjectivity scoring  
   - Transformer: emotion classification using a pretrained DistilBERT model  

5. **Evaluation and Comparison**
   - Manual labeling of a 100-sample subset to establish ground truth  
   - Resolution of model outputs into Positive, Neutral, and Negative categories  
   - Accuracy comparison across models  
   - Success and failure case analysis  
   - Multi-criteria model comparison  

---

## Key Findings (Summary)

- VADER performed best on expressive text and handled capitalization and punctuation effectively.  
- TextBlob handled simple negation reasonably well but showed less consistency overall.  
- The transformer model captured richer emotional nuance but required additional processing and higher computational cost.  

Model selection depends on text length, domain, and performance constraints.
