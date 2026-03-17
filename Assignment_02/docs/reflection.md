# Reflection — Custom Inference Evaluation

**Student:** Sadaf Sarbazi  
**Course:** BSAN 6200 — Text Analytics  
**Assignment:** Text Classification  
**Date:** Spring 2026  

---

## Overview

To evaluate how well the final model generalizes beyond the training dataset, I created a set of **20 custom inference examples**. These examples included a mixture of:

- clear ESG statements
- ambiguous or “tricky” examples
- sentences outside the ESG reporting domain

This evaluation helps assess whether the model can correctly interpret new text and how robust it is when encountering unfamiliar language.

---

## Prediction Agreement

Out of the 20 custom examples, the model correctly predicted **11 out of 20 labels**, resulting in an **agreement rate of 0.55**.

This indicates that while the model performs reasonably well on structured ESG-style sentences, its performance decreases when encountering unfamiliar wording or ambiguous contexts.

---

## Observations

Several patterns emerged when reviewing the predictions:

**1. Strong performance on ESG-style language**

The model performed well when sentences closely resembled the language commonly found in ESG reports. Examples related to environmental impact, governance policies, or employee initiatives were generally classified correctly.

**2. Confusion between related ESG categories**

Some errors occurred between categories with overlapping themes, particularly between **Human Capital** and **Social Capital**. Both categories frequently involve language related to employees, community engagement, and stakeholder relationships, which can make them difficult to distinguish.

**3. Difficulty with out-of-domain examples**

Sentences that did not resemble typical ESG reporting language were more likely to be misclassified. This suggests that the model has learned patterns specific to the training dataset but may struggle when applied to different types of text.

---

## Interpretation

The model demonstrates reasonable predictive ability within the ESG domain but shows limitations in generalization. Because the training data primarily consists of structured ESG report sentences, the model may rely heavily on vocabulary patterns associated with those documents.

When the input text deviates from this style, classification accuracy declines.

---

## Potential Improvements

Several improvements could strengthen the model:

- Expanding the training dataset with more diverse examples  
- Adding additional labeled ESG sentences from different industries  
- Incorporating more advanced NLP techniques such as contextual embeddings  
- Increasing the number of examples for minority classes  

These changes could help the model better capture variations in ESG language and improve its ability to classify unfamiliar sentences.

---

## Conclusion

Overall, the model performs well when classifying sentences similar to those found in ESG reports but has difficulty with ambiguous or out-of-domain text. The results suggest that the model captures meaningful ESG vocabulary patterns but would benefit from additional training data and broader coverage of ESG-related language.
