# Medical-Specialty-Classification-using-N-Grams-
This project classified medical transcriptions from 8 specialties using N-gram models. Uni-gram, bi-gram, and tri-gram models were tested using Naive Bayes, KNN, Decision Tree, and LSTM models built in Python.

## Introduction

This project classifies medical transcription data into different specialties using N-gram modeling and machine learning classifiers. The aim is to accurately categorize medical reports to improve healthcare efficiency and quality.

The models tested include Multinomial Naive Bayes, K-Nearest Neighbors, Decision Tree, and Long Short-Term Memory (LSTM) neural networks. The data is pre-processed and N-gram tokenized before training each model. 

## Data

The data consists of medical transcriptions from 8 specialties. As the data contains sensitive patient information, it was anonymized before use. 

Similar specialties were combined to increase samples per class. The text was cleaned, tokenized, and lemmatized. Class imbalance was corrected via up/downsampling.

t-SNE visualization ensured categories group similar samples. The data was split into train and test sets before N-gram tokenization.

## Methods

N-gram tokenization (uni-,bi-,trigrams) converted text into vector features.

The models were trained on the N-gram tokenized data and evaluated on accuracy, precision, recall, and F1 score.

5-fold cross-validation prevented overfitting and provided reliable performance estimates.

## Results

The bi-gram Naive Bayes model achieved the highest accuracy of 87.9%. The LSTM model performed comparably well.

Naive Bayes consistently outperformed KNN and Decision Tree models for this dataset and task.

## Conclusion

The results demonstrate N-gram modeling and Naive Bayes classification can accurately categorize medical transcriptions for improved healthcare services.

## Future Work

- Collect more data to increase model accuracy
- Test models on new datasets to evaluate generalizability 
- Explore other ML models and feature extraction techniques

## References

[1] S. S. Bhatia et al., "A Survey on Text Classification: From Traditional to Deep Learning Techniques"

[2] B. J. Marafino et al., "N-gram support vector machines for scalable procedure and diagnosis classification, with applications to clinical free text data from the intensive care unit" 

[3] T. Chen & C. Guestrin, "Xgboost: A scalable tree boosting system"

[4] H. Wang et al., "Bidirectional LSTM-CRF models for sequence tagging"
