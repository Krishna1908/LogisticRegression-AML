Logistic Regression — Algorithm 2 of 14 (IIT Kanpur AML)

This project demonstrates Logistic Regression — a fundamental supervised classification algorithm — as part of the Applied Machine Learning (AML) course from IIT Kanpur. This guide covers the intuition, math, real-world use cases, training process, and model evaluation.

Definition

Logistic Regression is a supervised learning algorithm used for binary classification problems. It estimates the probability that an input belongs to a certain class (0 or 1).

Unlike Linear Regression, which outputs continuous values, Logistic Regression outputs a probability between 0 and 1.

 Why Use Logistic Regression?

To solve problems where the target variable is categorical, especially binary:

Will a student pass or fail?

Is an email spam or not?

Will a customer buy a product or not?

Real-World Analogy

Imagine you’re a teacher predicting whether a student will pass based on study hours.

< 4 hours: mostly failed
6 hours: mostly passed

We don’t want to predict marks, we want to classify pass/fail. Logistic Regression gives a probability:

2 hours → 0.2 (20% pass)

6 hours → 0.85 (85% pass)

9 hours → 0.98 (almost surely pass)

Then we apply a threshold (like 0.5) to classify the result.

What It Predicts

Predicts P(Y = 1 | X)

“Given input X, what is the probability that Y is 1?”

Then converts it into a class using a threshold (e.g., 0.5)

How Logistic Regression Works

Compute a linear function:


Pass z into Sigmoid Function:

This outputs a probability between 0 and 1

Apply threshold:

If probability > 0.5 → predict class 1

Else → predict class 0

Σ Math (Simplified)

1. Sigmoid Function

Used to convert the output of linear equation to a value between 0 and 1:


2. Cost Function (Log Loss)


Where:

: actual label (0 or 1)

: predicted probability

: number of samples

3. Optimization (Gradient Descent)

Adjust weights to minimize the loss:



Training vs Prediction

Training: Learn the best weights (w) and bias (b) using training data

Prediction: Use learned weights to compute P(Y = 1) for new data

What You Get After Training

Final equation: ( \hat{y} = \sigma(wX + b) \ )

Accuracy of the model

Confusion Matrix

Precision, Recall, F1-score

ROC Curve (optional)

Real-Life Applications

Domain

Use Case

Health

Will patient have disease? (Yes/No)

Banking

Will loan default occur? (Yes/No)

Education

Will student pass? (Yes/No)

E-commerce

Will user buy product? (Yes/No)

 Logistic vs Linear Regression

Feature

Logistic Regression

Linear Regression

Target variable

Binary (0 or 1)

Continuous

Output

Probability (0 to 1)

Any real value

Function

Sigmoid

Straight Line

Use case

Classification

Prediction

Summary: Learning in Logistic Regression

Step

Description

Input

Training data (X and y)

Compute

Linear function wX + b

Predict

Apply sigmoid

Compare

Use Log Loss

Adjust

Update w and b using gradients

Repeat

Until loss is minimized

🎓 Author

Krishna Teja Reddy LingalaIIT Kanpur Certified | Applied Machine Learning (AML)

