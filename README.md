---

# Python, NumPy & Pandas — Applied Learning & Projects

This repository documents my structured self-learning journey in **Python**, **NumPy**, and **pandas**, built through applied, portfolio-grade projects.
The emphasis is on **first-principles understanding**, avoiding black-box abstractions, and writing **clear, explainable, production-style code**.
Each project mirrors real analytical workflows and focuses on *why* things work, not just *how* to use them.

---

## 📝 Projects

### 1. Customer Transactions Analysis

**(Pandas Mastery Project)**

#### Focus

* End-to-end data analysis using **pandas only**, from raw CSV ingestion to advanced analytics.
* Designed to systematically master pandas APIs used in real-world data analyst and analytics engineering roles.

#### Problem Statement

* Analyze a synthetic customer transactions dataset to understand **customer behavior**, **spending patterns**, and **temporal trends**.
* Build analytical intuition while progressing from basic operations to time-series and window-function analysis.

#### Dataset Overview

* Customer ID
* Name, Surname
* Gender
* Birthdate
* Transaction Amount
* Transaction Date
* Merchant Name
* Category

#### Key Steps

* **Data Ingestion & Validation**

  * CSV loading with dtype control, datetime parsing, duplicate detection, and missing-value handling.
* **Data Cleaning & Feature Engineering**

  * Boolean masking for invalid transactions, string normalization, categorical optimization, and age derivation.
* **Aggregations & Analytics**

  * Customer-level and category-level metrics using `groupby`, `agg`, `size`, and `value_counts`.
* **Time-Series Analysis**

  * Daily, weekly, and monthly resampling to analyze trends and seasonality.
* **Rolling & Window Functions**

  * Rolling spend, cumulative sums, per-customer rankings, and SQL-style analytics using pandas.

#### Pandas Concepts Demonstrated

* Indexing and boolean masking
* GroupBy (split–apply–combine)
* `.size()` vs `.count()` vs `.value_counts()`
* Datetime operations (`.dt`, `resample`, rolling windows)
* Window functions (`rank`, `cumsum`, `transform`)
* MultiIndex handling and pivot tables
* Memory optimization using categorical dtypes

#### Tools & Stack

* Python
* pandas (only)

#### Why This Project Matters

* Demonstrates the ability to **think in pandas idioms**, not loops.
* Handles realistic transactional data with production-style workflows.
* Relevant for data analyst, analytics engineer, and data engineering roles.

---

### 2. Credit Risk Scoring Using NumPy

#### Focus

* Statistical analysis and numerical linear algebra using **pure NumPy**, without black-box ML libraries.
* Emphasis on understanding numerical behavior and stability in real datasets.

#### Problem Statement

* Build an end-to-end credit risk scoring system to study **correlated financial features** and **numerical instability**.
* Analyze how risk estimation changes under collinearity and ill-conditioned matrices.

#### Key Steps

* **Data Preparation**

  * NaN handling, Z-score normalization, and percentile-based outlier clipping.
* **Statistical Analysis**

  * Covariance and correlation matrices to identify feature collinearity.
* **Risk Scoring**

  * Expert-defined weighted scores using matrix–vector multiplication.
* **Data-Driven Modeling**

  * Learned optimal weights using `np.linalg.lstsq`, with residual and singular value analysis.
* **Numerical Stability**

  * Diagnosed instability using SVD and applied truncated SVD to remove redundant directions.
* **Validation**

  * Achieved high correlation (~0.95) between expert-defined and data-learned risk scores.

#### Key Concepts Demonstrated

* Numerical linear algebra: least squares, SVD, conditioning
* Statistical reasoning: covariance, correlation, normalization
* Pure NumPy implementation without scikit-learn

#### Tools & Stack

* Python
* NumPy (`linalg`, statistics, matrix operations)

#### Why This Project Matters

* Reflects real **quantitative finance and fintech** workflows.
* Focuses on *why models fail numerically*, not just how to fit them.
* Relevant for quant, applied math, data engineering, and research roles.

---

### 3. Python Self-Learning Journal

#### Focus

* Learning Python from **first principles**, reinforced through continuous hands-on practice.
* Acts as both a learning timeline and a personal knowledge base.

#### Description

* A continuously updated notebook (`python_journal.ipynb`) covering:

  * Core Python syntax
  * Data structures
  * Control flow
  * Functions
  * NumPy and pandas fundamentals

#### Workflow

* Iterative learning using Jupyter Notebook / Google Colab.
* Regular commits pushed to GitHub to track progress.
* Strong emphasis on clarity, consistency, and conceptual understanding.

---

## 🚀 How to Use This Repository

* Open notebooks using **Jupyter Notebook** or **Google Colab**.
* Each project notebook is **self-contained and fully runnable**.
* The Python Journal serves as a long-term reference and learning archive.

---

## 📌 Key Takeaways

* Strong foundations in Python, NumPy, and pandas.
* Demonstrates applied numerical reasoning and analytical thinking.
* Avoids black-box abstractions in favor of explainable logic.
* Highlights a structured, engineering-driven self-learning approach.

---
