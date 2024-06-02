# PCSE24-19

# Credit Card Fraud Detection Using SMOTE

## Overview

This project focuses on detecting credit card fraud by addressing class imbalance in the dataset using oversampling techniques, particularly the Synthetic Minority Over-sampling Technique (SMOTE). Class imbalance is a common issue in fraud detection where fraudulent transactions are significantly fewer than legitimate ones.

## What is Oversampling?

Oversampling is a technique used to balance imbalanced datasets by increasing the number of minority class instances. This can be achieved by duplicating existing samples (Random Oversampling) or creating new synthetic samples (SMOTE).

### Types of Oversampling

1. **Random Oversampling**
   - Duplicates examples from the minority class.
   - Simple but can lead to overfitting.

2. **SMOTE (Synthetic Minority Over-sampling Technique)**
   - Creates synthetic samples by interpolating between existing minority class instances.
   - Reduces overfitting and improves classifier performance.

## SMOTE: Synthetic Minority Over-sampling Technique

SMOTE generates synthetic samples by interpolating between existing minority class instances, thus helping to balance the class distribution without simply duplicating existing data.

### How SMOTE Works

1. **Identify Neighbors**: For each minority class instance, find its \( k \)-nearest neighbors.
2. **Random Selection**: Randomly select one or more of these neighbors.
3. **Generate Synthetic Samples**: Create new instances by interpolating between the selected neighbors and the original instance.

### Benefits of SMOTE

- **Reduces Overfitting**: Produces unique synthetic samples.
- **Improves Performance**: Balances class distribution for better classifier performance.

### Limitations of SMOTE

- **Class Overlap**: May introduce samples that overlap with the majority class.
- **Computational Cost**: Can be computationally intensive for large datasets.

## Project Implementation

In this project, SMOTE is applied to the European Cardholder Dataset of 2013 to balance the dataset by generating synthetic samples for fraudulent transactions. This balanced dataset is then used to train machine learning models to detect credit card fraud more effectively.

## Conclusion

Using SMOTE to handle class imbalance in fraud detection improves model performance and reduces overfitting, making it a valuable technique for detecting credit card fraud.

## References

- Final project report with detailed implementation and results.

## Dataset

- https://drive.google.com/file/d/1Tt2SxZaHkpCkNTBCzgMrP6LkHcmcD7GO/view?usp=sharing
