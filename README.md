# Machine Learning Lab Spring 2026

This repository contains machine learning implementations written from scratch with minimal LLM assistance. 
The code progresses from fundamental concepts to more complex algorithms, with (almost) each notebook building on previous work.

**Prerequisites:** Basic Python knowledge is assumed.

## Recommended Reading Order

### 1. [Essential Libraries for Machine Learning](/ML_Lab_01_jan_02.ipynb)
Introduction to core libraries: `numpy`, `pandas`, and `scipy` with practical examples.

### 2. [Data Preprocessing](/ML_Lab_02_jan_09.ipynb)
Demonstrates a complete preprocessing workflow using a benign vs. defacement URLs dataset.

**Topics covered:**
- Data cleaning and feature engineering
- Regular expressions with pandas
- Train-test split

**Note:** Includes a linear regression example in a separate section.

### 3. [Decision Tree](/ML_Lab_03_jan_16.ipynb)
Implements a `DecisionTree` class from scratch only for categorical data classification using entropy and information gain.

**Requirements:**
- Understanding of entropy and information gain concepts
- Familiarity with recursive algorithms
- Prerequisites: Lab 2 (preprocessing)

**Performance:** Achieves 98 percent accuracy on test data.

**Current status:** Working implementation with room for optimization.

### 4. [Bias and Variance](/ML_Lab_04_jan_23.ipynb)
Uses a very simple dataset [`./Salary.csv`](./Salary.csv) having only two columns to train three different models to demonstrate underfitting, overfitting and a neutral between them. Visualizes the $\text{Bias}^2 + \text{Variance}$ vs $\text{Model Complexity}$ plot.

Requirements:
- Concept of Overfitting
- Concepts of Bias and Variance and their calculation
- Bootstrap Sampling

### 5. [Variation of Confidence Interval Size](/ML_Lab_05_jan_30.ipynb)
Analyzes how confidence intervals change under different conditions using linear regression on synthetic noisy data.

**Experiments:**
1. **Varying noise σ:** Higher noise → larger confidence intervals
2. **Varying dataset size:** More data → smaller confidence intervals  
3. **Varying confidence level:** Higher confidence → wider intervals

**Confidence Interval Formula:**

$$\text{CI} = \bar{x} \pm z \left( \frac{\sigma}{\sqrt{n}} \right)$$

**Requirements:**
- Understanding of confidence intervals and z-scores
- Familiarity with statistical uncertainty quantification

> ### [Side Quest 01 - Polynomial Regression](/SQ_01_Polynomial_Regression.ipynb)
> Implements a `PolynomialRegressor` class from scratch for `pd.DataFrame` objects using `numpy` and visualizes the working on a synthetic data with synthetic noise.
> 
> **Requirements:**
> - Knowledge of Gradient Descent Algorithm
> - Familiarity with Normalization/Standardization and advantages

### 6. [Logistic Regression](/ML_Lab_06_feb_06.ipynb)
Implements a `LogisticRegression` class froms scratch and visualizes working on a synthetic data.

**Requirements:**
- Understanding of Logistic Regression Algorithm
- The sigmoid function and its usage in Logistic Regression
- Gradient Ascent Algorithm (opposite of Gradient Descent)

### 7. [Support Vector Machines (SVMs)](/ML_Lab_07_feb_13.ipynb)
Implements a `SVM` class from scratch on top of the `cvxopt` library. Covers both hard-margin and soft-margin SVMs and visualizes the decision boundary, margin boundaries, and support vectors on synthetic data.

**Requirements:**
- Differences between SVM and Logistic Regression
- Relationship between the primal and dual forms of a constrained optimization problem
- Lagrangian multipliers and KKT conditions
- Quadratic Programming (QP) and how `cvxopt` maps to the dual SVM formulation

### 8. [SVM - Class-Specific Margins](/ML_Lab_08_feb_27.ipynb)
Extends the SVM implementation to give each class its own margin — because apparently treating both classes equally was too mainstream (classism). Visualizes the decision boundary, class-specific margin boundaries, and support vectors on synthetic data.

**Requirements:**
- Everything from the last lab
- A mild curiosity about what happens if you just... tweak one thing

> ### [Side Quest 02 - Approximating a Diagonal via Decision Tree](/SQ_02_Diagonal_Approximation.ipynb)
> Fitting a decision tree on a dataset that is separable by a diagonal line. Decision trees really have no business doing this, but here we are. Spoiler: it works, kind of.
> 
> **Requirements:**
> - Decision Trees
> - Low expectations

### 9. [Artificial Neural Networks from Scratch](/ML_Lab_09_mar_20.ipynb)
Implements the `Layer`, `Dense`, `Dropout`, and `ANN` classes entirely from scratch (in the hopes that one day these machines might become as intelligent as us humans). Includes an empirical comparison between L2-regularization and dropout for mitigating overfitting. [Remaining: Adaptive learning rates]

**Requirements:**
- Gradient Descent and the Chain Rule
- Object-Oriented Programming in Python (Classes and inheritance)
- Neural Network theory, including forward and backward propagation (the notebook includes mathematical derivations along with the code, but a prior formal understanding is recommended)

## Contribution
No hard rules. If you've got something worth sharing, open a PR. Just make sure you include the math behind it — don't drop a black box and disappear. If it uses a niche library or some non-obvious syntax, add comments and a markdown section explaining what's going on. Future readers shouldn't have to reverse-engineer your thought process. If possible, share the resources explaining the mathematics behind that. 