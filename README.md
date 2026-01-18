This repository contains machine learning implementations written from scratch with minimal LLM assistance. The code progresses from fundamental concepts to more complex algorithms, with each notebook building on previous work.

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
Implements a `DecisionTree` class from scratch for categorical data classification using entropy and information gain.

**Requirements:**
- Understanding of entropy and information gain concepts
- Familiarity with recursive algorithms
- Prerequisites: Lab 2 (preprocessing)

**Performance:** Achieves ~0.99 accuracy on test data.

**Current status:** Working implementation with room for optimization.