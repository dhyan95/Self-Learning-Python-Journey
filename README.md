Python, NumPy & Pandas — Applied Learning & Projects

This repository documents my structured self-learning journey in Python along with portfolio-grade applied projects built from first principles.
The focus is on understanding fundamentals deeply, avoiding black-box abstractions, and writing clear, explainable, production-style code.

📝 Projects
1. Customer Transactions Analysis (Pandas Mastery Project)
Focus

End-to-end data analysis using pandas only, progressing from basics to advanced time-series and window-function analytics.

Problem Statement

Analyze a synthetic customer transactions dataset to understand customer behavior, spending patterns, and temporal trends while systematically mastering pandas APIs used in real analytics workflows.

Dataset Overview

Customer ID

Name, Surname

Gender

Birthdate

Transaction Amount

Transaction Date

Merchant Name

Category

Key Steps

Data Ingestion & Validation:
CSV loading with dtype control, datetime parsing, duplicate detection, missing-value handling.

Data Cleaning & Feature Engineering:
Boolean masking for invalid transactions, string normalization, categorical optimization, age derivation from birthdate.

Aggregations & Analytics:
Customer-level and category-level metrics using groupby, agg, size, and value_counts.

Time-Series Analysis:
Daily / weekly / monthly resampling, trend and seasonality analysis.

Rolling & Window Functions:
Rolling transaction sums, cumulative spend, transaction ranking per customer, SQL-style analytics using pandas.

Pandas Concepts Demonstrated

Indexing & boolean masking

GroupBy (split–apply–combine)

.size() vs .count() vs .value_counts()

Datetime operations (.dt, resample, rolling windows)

Window functions (rank, cumsum, transform)

MultiIndex handling & pivot tables

Memory optimization using categorical dtypes

Tools & Stack

Python, pandas (only)

Why This Project Matters

This project demonstrates the ability to:

Think in pandas idioms, not loops

Handle realistic transactional data

Apply advanced analytics patterns without external libraries

Suitable for data analyst, data engineering, and analytics-heavy roles.

2. Credit Risk Scoring Using NumPy
Focus

Statistical analysis, numerical linear algebra, and numerical stability — no black-box ML.

Problem Statement

Built an end-to-end credit risk scoring system to understand how correlated financial features affect risk estimation and how numerical instability arises in real-world datasets.

Key Steps

Data Preparation:
NaN handling, Z-score normalization, percentile-based outlier clipping.

Statistical Analysis:
Covariance and correlation matrices, identification of feature collinearity.

Risk Scoring:
Expert-defined weighted risk scores using matrix–vector multiplication.

Data-Driven Modeling:
Learned optimal weights using np.linalg.lstsq, analyzed residuals and singular values.

Numerical Stability:
Diagnosed instability using SVD, applied truncated SVD to remove redundant directions.

Validation:
High correlation (~0.95) between expert-driven and data-learned risk scores.

Key Concepts Demonstrated

Numerical linear algebra: least squares, SVD, conditioning

Statistical reasoning: covariance, correlation, normalization

Pure NumPy implementation (no scikit-learn)

Tools & Stack

Python, NumPy (linalg, statistics), matrix operations

Why This Project Matters

This mirrors real quantitative finance and fintech workflows, emphasizing why models fail numerically, not just how to fit them.
Relevant for quant, applied math, data engineering, and research roles.

3. Python Self-Learning Journal
Focus

Learning Python from first principles, reinforced through hands-on experimentation.

Description

A continuously updated notebook (python_journal.ipynb) documenting:

Core Python syntax

Data structures

Control flow

Functions

NumPy and pandas fundamentals

Serves as a personal knowledge base and learning timeline.

Workflow

Learning done iteratively in Jupyter / Google Colab

Regular commits pushed to GitHub

Emphasis on consistency, clarity, and concept-building

🚀 How to Use This Repository

Open notebooks in Google Colab or Jupyter Notebook

Each project notebook is self-contained and runnable

Python Journal acts as a reference and learning archive

📌 Takeaways

Demonstrates strong Python foundations

Shows applied understanding of NumPy, pandas, and numerical reasoning

Avoids black-box abstractions

Highlights structured self-learning and engineering mindset
