# MLM-Project-Individual
# ReadMe: Supervised Learning Report

## Overview

This document provides an in-depth analysis of supervised machine learning techniques applied to an import-export dataset. The goal was to classify shipping methods using various models and evaluate their performance based on accuracy, runtime, and interpretability.

### Contents

1.  **Data Preprocessing**
    
2.  **Supervised Learning Models**
    
3.  **Performance Comparisons**
    
4.  **Managerial Insights and Recommendations**
    

----------

## 1. Data Preprocessing

The dataset was preprocessed to ensure compatibility with machine learning algorithms:

-   **Missing Data:** The dataset contained no missing values, so no imputation was necessary.
    
-   **Encoding:** Ordinal encoding was applied to categorical variables.
    
-   **Scaling:** Min-Max scaling normalized numerical features to the range [0, 1].
    
-   **Data Split:** A 70:30 split was used for training and testing datasets.
    

----------

## 2. Supervised Learning Models

The following models were evaluated:

-   **Logistic Regression (LR):**
    
    -   Accuracy: 32.38%
        
    -   Fast runtime, suitable for quick analysis.
        
-   **Support Vector Machine (SVM):**
    
    -   Accuracy: 34.51%
        
    -   Slightly better accuracy but computationally expensive.
        
-   **Decision Tree (DT):**
    
    -   Accuracy: 32.31%
        
    -   Offers interpretability and moderate performance.
        
-   **K-Nearest Neighbors (KNN):**
    
    -   Accuracy: 34.51%
        
    -   Good for capturing proximity-based patterns, faster than DT.
        
-   **Random Forest (RF):**
    
    -   Accuracy: 34.58%
        
    -   Most accurate but computationally intensive.
        

----------

## 3. Performance Comparisons

-   Logistic Regression is preferred for scenarios requiring speed and simplicity.
    
-   Support Vector Machine and Random Forest excel in accuracy but demand more computational resources.
    
-   KNN strikes a balance between runtime and performance, especially for smaller datasets.
    
-   Decision Tree is interpretable and useful for understanding decision pathways but may underperform compared to ensemble methods.
    

----------

## 4. Managerial Insights and Recommendations

### Key Insights:

-   **Feature Importance:** Variables such as Country, Product, Quantity, Value, and Shipping Method significantly influenced classification accuracy.
    
-   **Class Imbalance:** Address imbalances using techniques like oversampling or SMOTE.
    
-   **Correlation Analysis:** Low correlations between numerical variables indicate potential independence.
    

### Recommendations:

1.  **Model Selection:**
    
    -   Use Logistic Regression for quick, interpretable results.
        
    -   Choose Random Forest for high accuracy on complex datasets.
        
    -   Leverage SVM for capturing intricate patterns.
        
2.  **Data Enhancements:**
    
    -   Incorporate additional features like shipping distance or seasonality.
        
    -   Regularly update models with new transaction data.
        
3.  **Operational Use Cases:**
    
    -   Automate shipping method predictions to improve logistics.
        
    -   Use feature importance to refine supply chain strategies.
        

----------

## Usage

This report can guide data scientists, analysts, and decision-makers in:

-   Selecting appropriate machine learning models for classification tasks.
    
-   Understanding the trade-offs between accuracy, runtime, and interpretability.
    
-   Implementing actionable strategies based on model insights.
