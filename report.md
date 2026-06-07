# Titanic Machine Learning Capstone Project

**Student Name:** Mazen  
**Course:** Machine Learning, Deep Learning & NLP Applications  
**Dataset:** Titanic Dataset

## 1. Introduction

For my capstone project, I worked on the Titanic dataset. I picked this dataset because the idea is easy to understand: we are trying to predict whether a passenger survived or not based on their information.

I liked this dataset because it is not just numbers with no meaning. Each row is a real passenger, so it was easier for me to understand what the model was learning.

## 2. Dataset Description

The dataset has 891 passengers. The main column I wanted to predict is `Survived`. A value of 1 means the passenger survived, and 0 means the passenger did not survive.

I used columns that I could explain clearly, such as ticket class, sex, age, number of family members, fare, and where the passenger got on the ship. Before training the models, I checked the missing values. Some ages were missing, so I filled them using the median age instead of deleting many rows.

I also changed text columns like `Sex` and `Embarked` into numbers, because machine learning models cannot understand words directly.

## 3. Models Used

I trained three normal machine learning models first:

- Logistic Regression
- Random Forest
- KNN

I compared them using accuracy, precision, recall, and F1-score. I did not only look at accuracy, because accuracy can sometimes be misleading. F1-score is helpful because it balances precision and recall.

## 4. Neural Network

After that, I trained a simple neural network. I kept it simple because this is my first capstone project, and I wanted to understand what was happening instead of just making the code look complicated.

The neural network tries to learn patterns from the passenger data using hidden layers. I compared it with the other models using the same scores.

## 5. Results and Comparison

In my results, the best model was **Random Forest** with an F1-score of **0.752**.

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Random Forest | 0.816 | 0.781 | 0.725 | 0.752 |
| KNN | 0.816 | 0.800 | 0.696 | 0.744 |
| Logistic Regression | 0.804 | 0.793 | 0.667 | 0.724 |
| Neural Network | 0.771 | 0.741 | 0.623 | 0.677 |

Random Forest performed the best overall. I think this makes sense because Random Forest combines many decision trees, so it can catch more patterns than a very simple model.

The neural network was not the best model. This showed me that neural networks are not always automatically better. For a small dataset like Titanic, a model like Random Forest can work really well.

## 6. What I Learned

I learned that machine learning is not only about training the model. A lot of the work happens before that, like cleaning the data, filling missing values, and choosing the right columns.

I also learned that we should compare more than one model before deciding which one is best. Before doing this project, I thought the most advanced model would always win, but the results showed me that simpler models can sometimes be better.

The main thing I learned is that understanding the steps matters more than just running the code.