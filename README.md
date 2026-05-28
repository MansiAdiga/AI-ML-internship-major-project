# Credit Card Fraud Detection using CTGAN

##  Project Overview

This project was developed as part of an internship at GNCIPL for the role of AI/ML Intern. The project uses Generative AI (CTGAN) to generate synthetic fraud samples and improve fraud detection performance on an imbalanced dataset.


##  Objectives

- Analyze and preprocess credit card transaction data
- Perform exploratory data analysis (EDA)
- Handle severe class imbalance
- Generate synthetic fraud data using CTGAN
- Train baseline and augmented machine learning models
- Compare model performances
- Deploy the final model using Streamlit
  

##  Dataset Description

The Kaggle dataset, 'creditcard.csv', contains transactions made by credit cards in September 2013 by European cardholders. 
Features:
- V1, V2,…,V28: The principal components obtained with PCA
- Time: The seconds elapsed between each transaction and the first transaction in the dataset
- Amount: The transaction amount
- Class: The target variable, which takes value 1 in case of fraud and 0 otherwise.
  

##  Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- CTGAN (SDV)
- Streamlit


##  Data Cleaning

- Checked for missing values
- Checked for duplicate values
- Dropped the duplicate values
- Verified data types
- Checked for unique values
- Checked class distribution 


##  Exploratory Data Analysis (EDA)

The following analyses and visualizations were performed:
- Class distribution analysis
- Transaction amount analysis
- Transaction amount distribution
- Correlation heatmap
- PCA visualization
- Class-wise amount distribution
- Boxplots and distribution plots


##  Generative AI Using CTGAN

CTGAN was used to generate realistic synthetic fraud samples by learning the distribution of fraudulent transactions.
Steps performed:
- Extracted fraud transactions
- Generated metadata using SDV
- Trained CTGAN model
- Generated synthetic fraud samples
- Augmented training dataset


##  Model Training and Evaluation

###  1. Baseline Model

A Random Forest classifier was trained on the original imbalanced dataset.
Results:
- Precision: 0.96
- Recall: 0.78
- F1-score: 0.86

###  2. Augemented Model

Synthetic fraud data generated using CTGAN was added to the training dataset.
Results:
- Precision: 0.88
- Recall: 0.80
- F1-score: 0.83


##  Key Insights

- Synthetic data augmentation improved fraud detection capability
- Excessive augmentation caused high false positives
- Moderate augmentation produced balanced performance


## Deployment

The final model was deployed using Streamlit as an interactive web application.  
Deployment link:  
https://ai-ml-internship-major-project-8nsepyknvttcrzappjg9eub.streamlit.app/


## Conclusion

This project successfully applied Generative AI techniques for improving credit card fraud detection. CTGAN-generated synthetic data helped address the class imbalance problem and improved the model’s ability to identify fraudulent transactions. The project also demonstrated that careful tuning of synthetic data quantity is essential to maintain balanced model performance. The final augmented model achieved improved recall while maintaining high precision, making it suitable for practical fraud detection applications. Additionally, deployment using Streamlit converted the trained model into a real-time interactive application, demonstrating the end-to-end implementation of an AI-powered fraud detection system.


## Author

Mansi Adiga  
AI/ML Intern Project — GNCIPL


