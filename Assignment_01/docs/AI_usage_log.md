# AI Usage Log – Assignment 1: Sentiment Analysis

**Course:** Text Mining & Social Media Analytics  
**Semester:** Spring 2026  
**Instructor:** Dr. Ace Vo  
**Student:** Sadaf Sarbazi  

---

## Overview

AI tools (ChatGPT) were used to assist with clarifying assignment requirements, debugging code, restructuring workflow, organizing the GitHub repository, and improving documentation clarity. All final decisions regarding preprocessing, manual labeling, model evaluation, interpretation of results, and conclusions were completed independently.

---

## Interaction 1: Assignment Requirement Clarification

**Date:** February 2026  
**Time Spent:** ~15 minutes  

**What I Was Trying to Do:**  
Understand evaluation requirements, expected deliverables, and grading emphasis for the assignment.

**AI Prompt:**  
"Can you help clarify the evaluation requirements and expected deliverables for this sentiment analysis assignment?"

**AI Response:**  
The AI summarized the assignment pipeline, explained required model outputs, highlighted the 100-sample manual labeling requirement, and noted the expectation for a comparison table with at least five criteria.

**What I Modified:**  
I cross-referenced the AI’s explanation with the official assignment instructions and reorganized my notebook to emphasize evaluation and comparison sections.

**Why I Modified It:**  
I wanted strict alignment with the professor’s written instructions rather than relying on a summarized interpretation.

**What I Learned:**  
The evaluation section is a core grading component.  
The transformer model outputs emotions rather than direct sentiment labels.

**AI Errors / Limitations Found:**  
The AI initially treated evaluation as one step among many. I identified its greater grading importance and adjusted my workflow accordingly.

---

## Interaction 2: Transformer Runtime Issue

**Date:** February 2026  
**Time Spent:** ~20 minutes  

**What I Was Trying to Do:**  
Run transformer-based inference efficiently without freezing the notebook.

**AI Prompt:**  
"Why is my transformer model freezing when running inference, and how can I fix it?"

**AI Response:**  
The AI suggested running inference on the full dataset.

**What I Modified:**  
I restricted transformer inference to the 100 manually labeled review sample instead of the full dataset (~50,000 rows).

**Why I Modified It:**  
Full-dataset inference caused excessive runtime and was unnecessary for the assignment’s evaluation requirements.

**What I Learned:**  
Neural network models are computationally expensive.  
Implementation scope should be guided by assignment objectives.

**AI Errors / Limitations Found:**  
The AI suggested full-dataset inference without considering computational cost or assignment constraints. I corrected this by scoping inference appropriately.

---

## Interaction 3: Mapping Emotion Outputs to Sentiment Categories

**Date:** February 2026  
**Time Spent:** ~15 minutes  

**What I Was Trying to Do:**  
Resolve transformer emotion outputs into positive, neutral, and negative sentiment categories.

**AI Prompt:**  
"How can I convert emotion outputs from a transformer model into sentiment categories?"

**AI Response:**  
The AI suggested the following mapping:
- joy, love → positive  
- sadness, anger, fear → negative  
- surprise → neutral  

**What I Modified:**  
I documented this mapping as an analytical design choice and justified it explicitly in the analysis.

**Why I Modified It:**  
Emotion-to-sentiment mapping is subjective and must be transparently explained.

**What I Learned:**  
Model outputs may require interpretation layers.  
Design choices must be justified rather than assumed.

**AI Errors / Limitations Found:**  
The AI presented the mapping as a straightforward solution without emphasizing subjectivity. I framed it as an analytical assumption.

---

## Interaction 4: Code Debugging and Execution Order

**Date:** February 2026  
**Time Spent:** ~20 minutes  

**What I Was Trying to Do:**  
Fix execution issues and ensure the notebook ran cleanly from top to bottom.

**AI Prompt:**  
"Can you help debug my notebook and identify why it is not running correctly?"

**AI Response:**  
The AI identified missing imports, duplicate imports, incorrect CSV loading logic, and execution-order issues.

**What I Modified:**  
I cleaned imports, corrected file paths, ensured the correct manually labeled CSV was used, and reordered cells for consistent execution.

**Why I Modified It:**  
Proper execution order and clean imports improve reproducibility and prevent runtime errors.

**What I Learned:**  
Notebook execution order matters.  
Clean imports improve readability and reduce confusion.

**AI Errors / Limitations Found:**  
Some AI suggestions assumed variables persisted across cells. I corrected this by enforcing explicit execution order.

---

## Interaction 5: Final Analysis and Comparison Drafting

**Date:** February 2026  
**Time Spent:** ~15 minutes  

**What I Was Trying to Do:**  
Structure the final comparison table, recommendations, and limitations clearly.

**AI Prompt:**  
"How should I structure the final comparison and recommendation section?"

**AI Response:**  
The AI suggested using a comparison table with five or more criteria, followed by a recommendation and limitations discussion.

**What I Modified:**  
I revised the wording to reflect actual results rather than generic phrasing.

**Why I Modified It:**  
Conclusions must be data-driven and reflect observed model behavior.

**What I Learned:**  
Clear structure aids communication, but conclusions must remain grounded in analysis.

**AI Errors / Limitations Found:**  
None significant in this interaction.

---

## Interaction 6: README and GitHub Repository Structure

**Date:** February 2026  
**Time Spent:** ~15 minutes  

**What I Was Trying to Do:**  
Organize the GitHub repository and prepare a README that satisfies the assignment submission checklist.

**AI Prompt:**  
"What should be included in an assignment README, and how should a GitHub repository be structured for clarity and grading?"

**AI Response:**  
The AI suggested organizing the repository using separate folders for notebooks, data, and documentation, and including README sections for project overview, dataset description, key findings, execution instructions, results, and links to files.

**What I Modified:**  
I aligned the README explicitly with the assignment checklist and adjusted wording to accurately reflect my analysis. Final folder naming and file placement decisions were made independently.

**Why I Modified It:**  
The README and repository structure needed to map directly to grading criteria rather than follow a generic template.

**What I Learned:**  
Clear repository organization improves reproducibility, grading transparency, and interpretability.

**AI Errors / Limitations Found:**  
The AI initially suggested a generic project README. I refined it to meet assignment-specific requirements.

---

## Reflection on AI Use

AI was used as a clarification, debugging, documentation, and structural support tool. All manual labeling, evaluation decisions, interpretation of results, and final conclusions were completed independently. AI suggestions were reviewed critically, and limitations were identified and corrected where necessary.
