
---

## 📝 Projects

### 1. Credit Risk Scoring Using NumPy
**Focus:** Statistical analysis, linear algebra, and numerical stability (no black-box ML).  

**Problem Statement:**  
Built an end-to-end credit risk scoring system to understand how correlated financial features impact risk estimation and how numerical instability arises in real-world data.

**Key Steps:**
- **Data Preparation:** Handled NaNs, Z-score normalization, percentile-based outlier clipping.  
- **Statistical Analysis:** Covariance/correlation matrices, identified feature collinearity.  
- **Risk Scoring:** Expert-driven weighted scores and linear risk function using matrix–vector multiplication.  
- **Data-Driven Modeling:** Learned optimal weights with `np.linalg.lstsq`, analyzed residuals and singular values.  
- **Numerical Stability:** Diagnosed instability with SVD, applied truncated SVD to remove redundant directions.  
- **Validation:** Correlated expert-defined and data-learned risk scores (~0.95 agreement).

**Key Concepts Demonstrated:**  
- Numerical linear algebra: least squares, SVD, conditioning  
- Statistical reasoning: covariance, correlation, normalization  
- Pure NumPy implementation (no scikit-learn)

**Tools & Stack:**  
Python, NumPy (linalg, stats), matrix operations, numerical analysis

**Why This Project Matters:**  
This project mirrors workflows used in finance and fintech, demonstrating understanding of **why models fail numerically**, not just how to fit them. Suitable for **quantitative, data engineering, or applied math roles**.  

---

### 2. Python Journal
**Focus:** Self-learning Python from scratch through structured exercises and notes.  

**Description:**  
- Daily learning journal tracking Python syntax, data structures, functions, control flow, libraries like NumPy & Pandas, and applied exercises.  
- Organized by topic in a single notebook (`python_journal.ipynb`) for easy reference.  
- Useful to demonstrate **continuous learning, problem-solving, and coding discipline**.

**Workflow:**  
- Updated regularly in Google Colab.  
- Commits pushed to GitHub to maintain version history and showcase learning progress.  

---

## 🚀 How to Use This Repo
- Open notebooks in **Google Colab** or **Jupyter**.  
- Credit Scoring project notebook is self-contained and can be run end-to-end with minimal setup.  
- Python Journal notebook serves as a reference for learning concepts and exercises.

---

## 📌 Takeaways
- Demonstrates applied Python skills, statistical reasoning, and numerical analysis.  
- Shows ability to build **portfolio-quality projects** without relying on pre-built ML libraries.  
- Highlights continuous learning and structured problem-solving approach.

---

