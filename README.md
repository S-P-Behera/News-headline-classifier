# News-headline-classifier
## Project Overview

The News Headline Classifier is an end-to-end Natural Language Processing (NLP) project that automatically categorizes news headlines into predefined categories using Machine Learning. The project demonstrates the complete lifecycle of a text classification solution—from data collection and preprocessing to feature engineering, model development, evaluation, sensitivity analysis, and prediction.

Multiple classification algorithms were trained and compared to identify the most effective model for news categorization. The final solution achieved 93% classification accuracy, with Random Forest outperforming other traditional machine learning models.

## 🎯 Business Problem

With thousands of news articles published every day, manually organizing headlines into categories is time-consuming and inconsistent. News organizations and digital platforms require an automated classification system to accurately categorize articles, improve content management, enhance searchability, and deliver personalized news recommendations.

## 🎯 Objectives
Build an automated news headline classification system using Natural Language Processing.
Transform textual headlines into machine-readable features using TF-IDF.
Train and compare multiple Machine Learning algorithms.
Identify the best-performing classification model.
Analyze model robustness through sensitivity analysis.
Generate performance visualizations for business interpretation.

## 🧠 Technologies Used
Category	              Technologies
Programming Language	   Python
Machine Learning	       Scikit-learn
Data Processing	         Pandas, NumPy
NLP	                     TF-IDF Vectorization
Visualization	           Matplotlib, Seaborn
Development Environment	 Jupyter Notebook
Data Format	             CSV, JSON

## 📂 Dataset

The project uses a labeled dataset consisting of news headlines belonging to four major categories:

🏛 Politics
💼 Business
⚽ Sports
🎬 Entertainment

Each headline is paired with its corresponding category, enabling supervised machine learning for multi-class text classification.

## ⚙️ Project Workflow
### 1️⃣ Data Collection
Imported structured news headline dataset.
Loaded headlines and category labels.
Validated missing values and dataset consistency.
### 2️⃣ Text Preprocessing

Raw text was transformed into machine-readable format by:

Converting text to lowercase
Removing punctuation
Removing special characters
Eliminating unnecessary whitespace
Cleaning noisy text

This preprocessing improves feature quality and model performance.

### 3️⃣ Feature Engineering

The cleaned headlines were converted into numerical vectors using:

TF-IDF (Term Frequency – Inverse Document Frequency)

Feature extraction included:

Unigram representation
Bigram representation
Vocabulary size optimization
Feature scaling based on word importance
### 4️⃣ Model Development

Five supervised Machine Learning algorithms were trained and evaluated.

Model	Accuracy
Logistic Regression	87.2%
Naïve Bayes	88.4%
Linear SVM	86.0%
Decision Tree	87.2%
Random Forest	93.0%

Random Forest produced the highest overall performance across all evaluation metrics.

## 📊 Model Evaluation

The best-performing Random Forest model achieved:

Metric	Score
Accuracy	93.0%
Precision	94.5%
Recall	93.0%
F1 Score	93.2%

Performance was validated using:

Confusion Matrix
Precision
Recall
F1 Score
Accuracy
## 📈 Sensitivity Analysis

To evaluate model stability, multiple experiments were performed.

Vocabulary Size

Different TF-IDF vocabulary sizes were tested.

Finding

Performance increased as vocabulary expanded.
Accuracy stabilized after approximately 500 features, indicating diminishing returns with larger vocabularies.
N-gram Analysis

Different n-gram combinations were evaluated.

Tested:

(1,1)
(1,2)
(1,3)
(2,2)
(2,3)

Finding

Unigrams and bigrams provided the best balance between performance and computational efficiency.

Regularization Analysis

Different regularization strengths were analyzed.

Finding

Moderate regularization produced the most stable and accurate predictions while reducing overfitting.

Train-Test Split Analysis

Multiple train-test ratios were evaluated.

Finding

The model maintained strong performance across different splits, demonstrating good generalization capability.

## 📉 Performance Visualization

The project includes comprehensive visual analysis including:

Model Accuracy Comparison
Confusion Matrix
Vocabulary Sensitivity Analysis
N-gram Performance Analysis
Regularization Analysis
Train-Test Split Sensitivity
Overall Performance Metrics Dashboard

These visualizations provide an intuitive understanding of model performance and parameter optimization.

## 🔍 Key Insights
Random Forest achieved the highest classification accuracy (93%).
TF-IDF proved highly effective for representing textual features.
Increasing vocabulary beyond 500 features provided minimal additional benefit.
Moderate regularization improved model stability.
The classifier demonstrated strong generalization across different train-test splits.
Sports and Entertainment headlines showed the highest classification accuracy, while Business and Politics exhibited minor overlap due to similar vocabulary patterns.
