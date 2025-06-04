Finding Donors for CharityML
Project Overview
This project uses supervised machine learning algorithms to predict whether an individual makes more than $50,000 annually, helping CharityML identify potential donors. The model analyzes U.S. Census data from 1994 to make accurate income predictions.
Dataset

Source: UCI Machine Learning Repository (donated by Ron Kohavi and Barry Becker)
Based on: "Scaling Up the Accuracy of Naive-Bayes Classifiers: A Decision-Tree Hybrid"
Target Variable: Income (>$50K or ≤$50K)
Features: 13 features including age, education, occupation, marital status, and more

Key Features
Data Preprocessing

Feature Transformation: Log transformation for skewed features (capital-gain, capital-loss)
Normalization: MinMax scaling for numerical features
Encoding: One-hot encoding for categorical variables

Model Evaluation

Primary Metric: F₀.₅ score (emphasizes precision over recall)
Rationale: Precision is crucial for CharityML to avoid misidentifying non-donors as potential donors
Baseline: Naive predictor for performance comparison

Project Structure
├── finding_fonors.ipynb    # Main project notebook
├── census.csv                            # Dataset
└── README.md                            # This file

Getting Started
Prerequisites

Python 3.x
Jupyter Notebook
Required libraries: pandas, numpy, scikit-learn, matplotlib

Open the Jupyter notebook: jupyter notebook Finding_Donors_for_CharityML.ipynb
Follow the implementation sections marked with "TODO"
Answer the questions in the designated sections

Methodology

Data Exploration: Analyze dataset distribution and feature characteristics
Data Preprocessing: Transform, normalize, and encode features
Model Selection: Compare multiple supervised learning algorithms
Performance Evaluation: Use F₀.₅ score to evaluate model effectiveness
Optimization: Fine-tune the best performing algorithm

Key Insights

Dataset is imbalanced (most individuals earn ≤$50K)
Precision is prioritized over recall for business requirements
Feature engineering is crucial for model performance
