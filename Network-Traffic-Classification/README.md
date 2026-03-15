# Network Traffic Classification

## Project Overview
This project applies machine learning techniques to classify network traffic based on connection attributes. The objective is to distinguish between different types of network activity using predictive modelling.

## Dataset
The dataset contains network traffic observations with multiple connection features such as protocol type, packet statistics, and service type.

## Tools Used
Python  
pandas  
scikit-learn  
matplotlib  

## Workflow

1. Data cleaning and preprocessing  
2. Feature encoding and scaling  
3. Train/validation/test split  
4. Model training using multiple classifiers  
5. Model evaluation using accuracy and macro F1-score  

Models tested:

- k-Nearest Neighbours  
- Gaussian Naïve Bayes  
- Decision Tree  
- Random Forest  

## Results

Validation Accuracy ≈ 0.9919  
Cross-Validation Accuracy ≈ 0.9902  
Macro-F1 ≈ 0.9901  

Final selected model: **Decision Tree Classifier**
