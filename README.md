# Foundations of Data Science (FDS) — Comprehensive Case Studies

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12oGN-_mD7s1BDXXmQeC_afXthzv-dhE0?usp=sharing)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the complete implementation, exploratory analyses, visualizations, and comparative evaluations for two end-to-end Data Science case studies:

1. **Case Study 1: Market Basket Clustering & Transaction Pattern Mining** (Unsupervised Learning)
2. **Case Study 4: Predicting Student Dropout & Academic Success** (Supervised Machine Learning & Statistical Inference)

---

## 📑 Repository Structure

```text
fds-case-study/
│
├── FDS_Case_Study.ipynb    # Complete end-to-end Jupyter Notebook with all outputs & plots
├── README.md               # Project documentation and summary of findings
└── .gitignore              # Git ignore rules
```

---

## 🔬 Case Study 1: Market Basket Clustering & Pattern Mining

### 1. Objective
Perform unsupervised clustering and transaction pattern mining on retail transaction data to discover distinct customer purchasing behaviors, quantify basket sizes, identify frequently co-occurring items, and provide actionable business recommendations.

### 2. Methodology & Workflow
- **Data Preprocessing & Transaction Reconstruction**:
  - Filter cancellations, negative values, and missing customer IDs.
  - One-hot transaction encoding (Transaction × Item sparse feature vectors).
- **Exploratory Data Analysis (EDA)**:
  - Basket size distributions, log-log frequency curves, and Pareto 80/20 product analysis.
- **Dimensionality Reduction**:
  - Principal Component Analysis (PCA) applied to preserve variance while mitigating high dimensionality and sparsity.
- **Clustering Algorithms**:
  - **K-Means Clustering**: Optimal cluster determination using Elbow Method (Inertia) and Silhouette Analysis.
  - **Agglomerative Hierarchical Clustering**: Ward's linkage dendrogram and comparative partitions.
  - **DBSCAN**: Density-based clustering for outlier/anomaly detection.
- **Evaluation & Profiling**:
  - Silhouette Score, Davies-Bouldin Index, and Calinski-Harabasz Score.
  - Characteristic product profiling and strategic marketing recommendations per customer segment.

---

## 🎓 Case Study 4: Student Dropout & Academic Success Prediction

### 1. Objective
Formulate a predictive modeling framework using demographic, socioeconomic, and academic records to predict student outcomes (**Dropout**, **Enrolled**, **Graduate**), quantify primary risk indicators, and provide responsible intervention recommendations.

### 2. Methodology & Workflow
- **Data Understanding & Preprocessing**:
  - Clean feature types, handle missing values, and encode categorical descriptors.
  - Address class imbalance through stratified train-test splitting and appropriate evaluation metrics.
- **Statistical Hypothesis Testing**:
  - Chi-square tests of independence between categorical drivers (e.g., scholarship receipt, tuition status) and student outcome.
  - Two-sample t-tests and ANOVA on curricular unit evaluations and GPA.
- **Supervised Classification Modeling**:
  - **Multiclass Logistic Regression**: Multinomial logit formulation with balanced class weighting.
  - Cross-validation and evaluation across Precision, Recall, Macro F1-score, and Confusion Matrices.
- **Model Interpretation & Strategic Intervention**:
  - Feature coefficient odds-ratio analysis: Identifying early warning indicators (e.g., 1st & 2nd semester approved curricular units, tuition delinquency).
  - Ethical guidelines, algorithmic bias considerations, and targeted proactive academic counseling.

---

## 🚀 Getting Started

### Option A: Run in Google Colab (Recommended)
Click the badge below to open and execute directly in Google Colab with pre-configured dependencies:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12oGN-_mD7s1BDXXmQeC_afXthzv-dhE0?usp=sharing)

### Option B: Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/aneesh-379/fds-case-study.git
   cd fds-case-study
   ```
2. Install the required dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn scipy
   ```
3. Launch Jupyter:
   ```bash
   jupyter notebook FDS_Case_Study.ipynb
   ```

---

## 📊 Summary of Results

| Case Study | Primary Methodologies | Key Metric / Outcome |
| :--- | :--- | :--- |
| **Market Basket Clustering** | PCA + K-Means / Hierarchical / DBSCAN | Identifies core regular shoppers, bulk wholesalers, and seasonal gift buyers |
| **Student Academic Success** | Multiclass Logistic Regression + Hypothesis Testing | High recall on early-warning dropout risk; curricular success in Semester 1 & 2 is the single strongest retention predictor |

---

## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.
