# Titanic Machine Learning Capstone Project

**Student Name:** Mazen  
**Course:** Machine Learning, Deep Learning & NLP Applications  
**Dataset:** Titanic Dataset

## Project Overview

This project predicts Titanic passenger survival using machine learning models. The analysis includes data preprocessing, model training, and comprehensive performance evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Models Used](#models-used)
- [Results and Comparison](#results-and-comparison)
- [Key Learnings](#key-learnings)
- [Requirements](#requirements)

## Introduction

This capstone project uses the Titanic dataset to predict whether a passenger survived or not based on their information. The dataset contains real passenger data, making it easier to understand what the model learns.

## Dataset Description

- **Total Passengers:** 891
- **Target Variable:** `Survived` (1 = survived, 0 = did not survive)
- **Features Used:** Ticket class, sex, age, number of family members, fare, port of embarkation

### Data Preprocessing

- Missing ages filled using median value
- Text columns (Sex, Embarked) converted to numeric format
- Unnecessary columns removed for model training

## Models Used

1. **Logistic Regression** - Simple model for binary classification
2. **Random Forest** - Ensemble of decision trees
3. **KNN** - Instance-based learning approach
4. **Neural Network** - Deep learning approach with hidden layers

## Results and Comparison

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Random Forest | 0.816 | 0.781 | 0.725 | **0.752** |
| KNN | 0.816 | 0.800 | 0.696 | 0.744 |
| Logistic Regression | 0.804 | 0.793 | 0.667 | 0.724 |
| Neural Network | 0.771 | 0.741 | 0.623 | 0.677 |

**Best Model:** Random Forest with F1-score of 0.752

## Key Learnings

- Data preprocessing and feature engineering are crucial steps in machine learning
- It's important to compare multiple models before selecting the best one
- More complex models (like neural networks) aren't always better for smaller datasets
- F1-score is a better metric than accuracy alone for imbalanced datasets
- Understanding the data matters more than just running code

## Requirements

See `requirements.txt` for all dependencies:

```
pandas
numpy
matplotlib
scikit-learn
jupyter
```

## Installation

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open Jupyter notebook and run the analysis

## Usage

Run the analysis in Jupyter:

```bash
jupyter notebook
```

Then execute the cells to:
1. Load and explore the data
2. Preprocess the data
3. Train all models
4. Compare results
5. View visualizations

---

**Note:** This project demonstrates that understanding the problem, preparing the data well, and comparing multiple approaches is just as important as implementing sophisticated algorithms.