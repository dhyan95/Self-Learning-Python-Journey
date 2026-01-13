# Python, NumPy, Pandas & Visualization — Applied Learning & Projects

This repository documents a **structured, first-principles self-learning journey** in **Python**, **NumPy**, **Pandas**, and **Data Visualization (Matplotlib / Seaborn)**, developed through applied, portfolio-grade projects.

The emphasis is on **mental models over memorization**, avoiding black-box abstractions, and writing **clear, explainable, production-style code**.
Each project mirrors real analytical and data-science workflows, focusing on *why systems behave the way they do*, not just *how to call an API*.

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

## 3. Cryptocurrency Market Structure Analysis (Linear Algebra + Visualization)

**(NumPy · pandas · Matplotlib · Seaborn)**

### Focus

* Analyze **cryptocurrency market structure** using **linear algebra**, **pivot tables**, and **correlation analysis**.
* Emphasis on understanding **matrix representations of financial time series**, eigen-structure intuition, and how high-dimensional data is visualized.
* Avoids black-box ML pipelines; all transformations are explicit and explainable.

---

### Problem Statement

* Given historical cryptocurrency price data, analyze:

  * How different coins **co-move** over time
  * Whether the market exhibits **shared latent structure**
  * Which assets behave similarly or independently
* Build intuition for concepts that later appear in **PCA, SVD, factor models, and risk analysis**.

---

### Dataset Overview

Source: Kaggle — *Cryptocurrency Price History*

Key fields used:

* Date
* Cryptocurrency name
* Close price

Derived features:

* Daily returns
* Standardized return matrix
* Correlation matrix

---

### Analytical Workflow

#### Data Reshaping & Matrix Construction

* Converted long-format price data into a **wide pivot table**:

  * Rows → Dates
  * Columns → Cryptocurrencies
* Cleaned missing values to ensure a valid numerical matrix.
* Extracted the underlying NumPy array for linear algebra operations.

This step establishes the **design matrix** used throughout the analysis.

---

#### Statistical Normalization

* Computed **daily returns** to remove price scale effects.
* Standardized returns using mean centering and variance normalization.
* Result: a matrix suitable for correlation analysis and eigen-based reasoning.

---

#### Correlation Structure Analysis

* Computed the **correlation matrix** across cryptocurrencies.
* Interpreted correlations as similarity in return behavior.
* Visualized relationships using:

  * **Seaborn heatmap** for dense relational insight
  * Explicit axis labeling to preserve semantic meaning

This step connects raw math to interpretable financial structure.

---

#### Visualization & Interpretation

* **Seaborn heatmap**

  * Encodes correlation values as color intensity
  * Reveals clusters, market-wide movement, and outliers
* **Matplotlib plots**

  * Used for precise control and transparency
  * Reinforces understanding of how data maps to visuals

Visualizations are treated as *diagnostic tools*, not presentation artifacts.

---

### Key Concepts Demonstrated

* Pivot tables as **matrix builders**
* Broadcasting and vectorized operations
* Correlation as a geometric similarity measure
* Separation of:

  * Numeric computation (`NumPy arrays`)
  * Semantic meaning (`column labels`)
* Visualization as a projection of mathematical structure

---

### Tools & Stack

* Python
* pandas (data reshaping, cleaning)
* NumPy (matrix operations)
* Matplotlib (low-level plotting)
* Seaborn (statistical visualization)

---

### Why This Project Matters

* Builds a **mental bridge** between:

  * pandas analytics
  * NumPy linear algebra
  * Future topics like PCA, SVD, and factor models
* Mirrors real workflows in:

  * Quantitative finance
  * Market risk analysis
  * Applied data science
* Demonstrates the ability to reason about **data as matrices**, not just tables.

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
