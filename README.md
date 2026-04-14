# Iris_ML_Project

# Iris Flower Classification \- Machine Learning Project

# Project Overview

This project implements a machine learning classification system to predict the species of Iris flowers based on their sepal and petal measurements. The dataset contains 150 flower samples with 4 numerical features and 3 target classes.

# Dataset Description

Source: Iris Flower Dataset (Classic UCI Machine Learning Repository)  
Samples: 150 iris flowers  
Features: 4 numerical attributes  
  \- Sepal Length (cm)  
  \- Sepal Width (cm)  
  \- Petal Length (cm)  
  \- Petal Width (cm)

Target Classes: 3 species  
  \- Setosa (50 samples)  
  \- Versicolor (50 samples)  
  \- Virginica (50 samples)

# Data Exploration Results

Statistical Summary  
  \- Mean sepal length: 5.84 cm (range: 4.3 \- 7.9 cm)  
  \- Mean sepal width: 3.06 cm (range: 2.0 \- 4.4 cm)  
  \- Mean petal length: 3.76 cm (range: 1.0 \- 6.9 cm)  
  \- Mean petal width: 1.20 cm (range: 0.1 \- 2.5 cm)

Data Quality  
  \- No missing values  
  \- Perfectly balanced dataset (50 samples per class)  
  \- Data types: Float64 (features), Categorical (species)

# Models Implemented

Three classification algorithms were trained and evaluated:

1\. Logistic Regression  
Accuracy: 96.67%  
  \- Fast training and inference  
  \- Good baseline model performance  
  \- Linear decision boundaries

2\. Random Forest Classifier  
Accuracy: 90.00%  
  \- Ensemble learning approach  
  \- Non-linear decision boundaries  
  \- Provides feature importance insights

3\. K-Nearest Neighbors (K=5) \- BEST MODEL  
Accuracy: 100.00%  
  \- Instance-based learning  
  \- Perfect classification on test set  
  \- Most suitable for this balanced, well-separated dataset

# Model Evaluation Metrics

Best Model (KNN K=5) Performance:  
  \- Overall Accuracy: 100% (30/30 test samples)  
  \- Precision: 1.00 (all classes)  
  \- Recall: 1.00 (all classes)  
  \- F1-Score: 1.00 (all classes)

Confusion Matrix Results:  
All predictions were correct across all three classes:  
  \- Setosa: 10/10 correct  
  \- Versicolor: 10/10 correct  
  \- Virginica: 10/10 correct

# Feature Importance Analysis

(Random Forest Model)

Ranking of features by importance for classification:  
  1\. Petal Width: 43.72% \- Most important  
  2\. Petal Length: 43.15% \- Second most important  
  3\. Sepal Length: 11.63% \- Moderately important  
  4\. Sepal Width: 1.50% \- Least important

Insight: Petal measurements are far more discriminative for species classification than sepal measurements.

# Key Findings

1\. Dataset Quality: The Iris dataset is well-structured with balanced classes and clear feature distributions, making it ideal for classification tasks.

2\. Model Performance: All three models achieved high accuracy (\>90%), demonstrating that the features are highly predictive of species.

3\. Best Algorithm: K-Nearest Neighbors achieved 100% accuracy on the test set, making it the most suitable model for this dataset.

4\. Feature Relevance: Petal measurements (especially petal width and length) are the primary discriminators between species, accounting for \~87% of feature importance.

5\. Data Separability: The perfect accuracy suggests that the three iris species are well-separated in feature space, making classification straightforward.

# Technical Implementation

Libraries Used:  
  \- pandas: Data manipulation and analysis  
  \- numpy: Numerical computations  
  \- scikit-learn: Machine learning algorithms and evaluation metrics  
  \- matplotlib: Data visualization  
  \- seaborn: Statistical data visualization

Workflow:  
  1\. Data loading and preprocessing  
  2\. Exploratory data analysis (EDA)  
  3\. Data visualization (pair plots, distributions)  
  4\. Train-test split (80-20 ratio, stratified)  
  5\. Model training on three algorithms  
  6\. Model evaluation and comparison  
  7\. Feature importance analysis

# Visualizations Generated

  1\. Pair Plot: Relationship matrix between all features, colored by species  
  2\. Confusion Matrix: Shows prediction accuracy across all classes for best model  
  3\. Model Performance Comparison: Bar chart comparing accuracy of all three algorithms  
  4\. Feature Importance Chart: Horizontal bar chart showing feature contributions in Random Forest model

# Conclusions

This project successfully demonstrates the application of machine learning classification techniques to a real-world dataset. The K-Nearest Neighbors model achieved perfect classification, proving that the Iris species can be accurately predicted from botanical measurements. The analysis reveals that petal characteristics are far more important than sepal characteristics for distinguishing between the three species.
