# Simple Explanation for Mazen

This is the version you can read before presenting the project.

## What is my project about?

My project predicts if a Titanic passenger survived or not.

The computer looks at passenger information like age, gender, ticket class, fare, and family members. Then it tries to learn patterns from that information.

## What is the dataset?

The dataset is basically a table.

- Each row = one passenger
- Each column = one detail about that passenger
- The answer column = whether they survived or not

## What are X and y?

- `X` means the information we give the model, like age, sex, class, and fare.
- `y` means the answer we want the model to predict, which is survival.

So basically:  
**X = clues**  
**y = final answer**

## Why did I split the data?

I used 80% of the data to train the model and 20% to test it.

This is important because I do not want the model to just memorize the data. I want to see if it can make good predictions on passengers it has not seen before.

## What models did I use?

I used four models in total:

1. **Logistic Regression** - a simple model for yes/no predictions.
2. **Random Forest** - many decision trees working together.
3. **KNN** - predicts by looking at similar passengers.
4. **Neural Network** - uses hidden layers to learn patterns.

## What do the scores mean?

**Accuracy** means how many predictions were correct overall.

**Precision** means: when the model predicted someone survived, how often was it right?

**Recall** means: out of all the people who actually survived, how many did the model find?

**F1-score** combines precision and recall into one score. I used it to choose the best model.

## What was the best model?

The best model was **Random Forest**.

It had the highest F1-score, so I chose it as the best model.

## Easy way to explain it to your teacher

You can say:

> I used the Titanic dataset to predict survival. First, I cleaned the data by filling missing ages and converting text columns into numbers. Then I split the data into training and testing sets. I trained Logistic Regression, Random Forest, KNN, and a simple neural network. After comparing accuracy, precision, recall, and F1-score, Random Forest was the best model in my results.

## One sentence summary

This project taught me that preparing the data and comparing models is just as important as training the model itself.