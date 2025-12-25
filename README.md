# Machine Learning & Deep Learning for Data Science – Final Project

This repository contains the final project deliverable for the graduate-level course  
**Machine Learning and Deep Learning for Data Science**.

The assignment required identifying a real-world problem, sourcing a large dataset, and applying
machine learning techniques to build, validate, and compare predictive models.  
The project emphasizes **problem framing, model selection, validation rigor, and interpretation of results**.

---

## Project Context (STAR Framework)

### Situation
The rapid growth of AI-driven data centers is creating unprecedented electricity demand across North America. Policymakers and energy planners need to understand whether existing renewable energy infrastructure can realistically support this growth in the near future.

### Task
The objective of this project was to determine whether **North American renewable energy capacity can sustain projected data center electricity demand by 2028**, and if not, estimate the additional capacity required.

### Action
To address this problem, we:
- Sourced and curated a large, real-world dataset (>30,000 records) from the **Global Power Plant Database**
- Filtered and engineered plant-level features relevant to renewable generation
- Conducted exploratory data analysis and extensive preprocessing
- Trained and validated multiple supervised machine learning regression models
- Compared models using cross-validation and appropriate performance metrics
- Selected the most robust model to generate future (2028) capacity projections

### Result
The final model indicates that **current renewable capacity is insufficient** to meet projected data center demand by 2028, even under optimistic growth assumptions. The results quantify the expected shortfall and highlight where planning and investment gaps exist.

---

## Problem Definition

**Problem:**  
Can existing and projected renewable energy infrastructure in North America meet the electricity demands driven by AI and data center expansion by 2028?

**Why it matters:**  
Inaccurate capacity planning risks energy shortages, higher costs, and increased reliance on non-renewable sources. Reliable forecasting is essential for long-term infrastructure and policy decisions.

**What machine learning solves:**  
Machine learning models enable the prediction of future renewable energy generation based on plant-level characteristics such as capacity, age, and fuel type, capturing non-linear relationships that traditional forecasting approaches may miss.

---

## Dataset Overview

- **Source:** Global Power Plant Database (World Resources Institute)
- **Scope:** ~35,000 power plants globally  
- **Filtered to:** North American renewable energy plants
- **Final modeling dataset:** ~7,000 power plants
- **Features include:**
  - Installed capacity
  - Plant age
  - Fuel type
  - Historical and estimated generation
  - Engineered trend and efficiency features

---

## What This Repository Contains

- A **fully documented Jupyter notebook** showing:
  - Data sourcing, filtering, and preprocessing
  - Feature engineering and transformation
  - Exploratory data analysis and visualizations
  - Supervised learning model development
  - Cross-validation and hyperparameter tuning
  - Model comparison and evaluation
  - Scenario-based forecasting for 2028

> The written report and presentation were submitted separately for the course; this repository focuses on the analytical and modeling output.

---

## Modeling Approach

The project evaluated a broad range of regression models, including:

- Linear Regression (baseline)
- Lasso, Ridge, and Elastic Net
- Support Vector Regression (SVR)
- Decision Tree
- Random Forest
- Gradient Boosting

Models were compared using:
- **R² (coefficient of determination)**
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**

Repeated k-fold cross-validation was used to assess generalization and prevent overfitting.

---

## Key Findings

- **Gradient Boosting performed best**, achieving the highest R² (~0.98) and lowest prediction error.
- Non-linear models consistently outperformed linear approaches, indicating complex interactions in the data.
- Even under favorable assumptions, projected renewable generation **falls short of 2028 data center demand**.
- The estimated gap highlights the need for additional renewable capacity, efficiency gains, or alternative energy strategies.

---

## Why This Project Is Relevant

This project demonstrates the ability to:
- Frame ambiguous real-world problems for machine learning
- Engineer features from imperfect, large-scale datasets
- Apply and evaluate multiple ML models rigorously
- Use validation best practices to support defensible conclusions
- Translate model outputs into actionable insights for decision-makers

The workflow mirrors challenges commonly faced in **energy analytics, applied machine learning, and forecasting-focused data science roles**.

---
