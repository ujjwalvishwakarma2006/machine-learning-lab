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