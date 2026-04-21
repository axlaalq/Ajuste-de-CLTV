# 🏥 CLTV Adjustment with Clinical Conditions

## 📌 Overview

This project focuses on improving Customer Lifetime Value (CLTV) estimation by incorporating clinical conditions into the analysis.

Starting from a baseline CLTV calculated using probabilistic models (BG/NBD), we develop an adjusted CLTV metric that controls for confounding variables such as customer behavior and service mix.

The main objective is to produce a more accurate and interpretable metric for decision-making in healthcare environments.

---

## 🧠 Problem Statement

Traditional CLTV aggregation by cohorts (e.g., patients with a specific condition) can be biased due to:

- Differences in recency, frequency, and monetary value
- Behavioral heterogeneity
- Service consumption mix

This project addresses these issues by proposing a **confounder-controlled adjustment**.

---

## 📊 Dataset

The dataset includes:

- Precomputed CLTV values (MXN)
- Behavioral variables (recency, frequency, expected purchases)
- Monetary proxies
- Service mix indicators (laboratory vs imaging)
- Demographic segmentation (age group, gender)
- Clinical flags:
  - Type 2 Diabetes
  - Breast Cancer
  - General condition indicator

---

## ⚙️ Methodology

### 1. Data Audit & Preparation
- Missing values analysis
- Outlier detection
- Consistency checks
- Circularity risk identification

### 2. Baseline Analysis
- Cohort-based CLTV aggregation
- Identification of biases due to confounders

### 3. CLTV Adjustment

We define a new variable:
