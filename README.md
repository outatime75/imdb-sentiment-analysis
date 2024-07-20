# **IMDb-sentiment-analysis**

## Overview

This repository contains my completed coursework for the CIS5231 - Topics in Applied Data Science module, as part of my Masters in Data Science course, focusing on Sentiment Analysis. The project involved exploring various Natural Language Processing (NLP) techniques and machine learning classifiers to analyze sentiment in a large dataset of IMDb movie reviews.

## Submission Details 📋

### Jupyter Notebook
I submitted a Jupyter notebook containing all the code and results. The code was well-commented for clarity, and I set a random seed to ensure reproducibility.

### Dataset 🎬

- **Source**: IMDb movie reviews dataset (233,600 reviews)
- **Format**: Each line contains a review and an integer rating [1-4] for negative and [7-10] for positive sentiment.

### Tasks and Methodology 🛠️

1. **Initial Data Exploration**
   - I inspected the dataset to understand its structure and preprocessing needs. I checked if any preprocessing had been done and assessed how this might affect future processing steps.

2. **Data Processing**
   - I created four processed data variants using Pandas DataFrames:
     1. Tokenized text with only alphabetic words.
     2. Tokenized text with stop word removal.
     3. Tokenized text with lemmatization.
     4. Tokenized text with both lemmatization and stop word removal.
   - I transformed the ratings into a binary scale (-1 for negative, +1 for positive) for easier classification.

3. **Class Balance Analysis**
   - I analyzed the balance between positive and negative reviews and discussed the potential impact of class imbalance on classifier performance.

4. **Classification**
   - I applied Naïve Bayes and Support Vector Machine (SVM) classifiers to each of the four datasets.
   - For each run, I recorded the accuracy, precision, recall, F1 score, and confusion matrices. I used a 70% training and 30% testing split with 5,000 features, ensuring the data was stratified.

5. **Results Observation**
   - I evaluated the impact of different preprocessing steps on classification performance. Additionally, I reran one dataset with inverted class labels and analyzed the confusion matrix to gain further insights.

6. **Handling Class Imbalance**
   - I employed random undersampling to balance the dataset.
   - I applied the classifiers to the balanced datasets and recorded the same metrics as before. I compared these results to those from the unbalanced dataset and discussed scenarios where each approach might be preferable.

7. **Feature Expansion**
   - I selected the best-performing run and increased the feature set to 10,000. I evaluated the impact on model performance and runtime, noting any significant changes.

8. **Evaluation of Related Work**
   - I reviewed and critiqued the evaluation metrics and methodology used in the referenced paper by Nguyen et al. (2014). I provided my thoughts on their evaluation criteria and suggested possible improvements.

## References

- [IMDb Movie Reviews Dataset](https://github.com/daiquocnguyen/SAR14?tab=readme-ov-file)
- Nguyen, D. Q., Nguyen, D. Q., Vu, T., & Pham, S. B. (2014). Sentiment classification on polarity reviews: An empirical study using rating-based features. In Proceedings of the 5th Workshop on Computational Approaches to Subjectivity, Sentiment and Social Media Analysis, pp. 128-135.

---


