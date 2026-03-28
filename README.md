# Duolingo Learning Behavior Analysis

## Overview
This project analyzes large-scale Duolingo learning data (~13M records) to understand how user recall probability changes over time and across different learning conditions.

The goal is to model learning behavior and identify key factors that influence retention, using statistical analysis and regression techniques.

---

## My Contribution
This repository is a cleaned showcase version of a team project. I focused on:

- Designing the data processing pipeline for large-scale learning data
- Building statistical models to analyze recall probability (p_recall)
- Investigating how time intervals and historical performance affect retention
- Interpreting results to uncover patterns in user learning behavior

---

## Data

The original dataset (Duolingo learning traces, ~13M rows) is not included due to size constraints.

### Data Processing
- Extracted key features: `p_recall`, `delta`, `learning_language`, `history_seen`, `history_correct`
- Processed large-scale data using chunked reading
- Cleaned missing values and standardized language labels
- Split dataset by language for analysis

---

## Methods

### Data Cleaning
- Used chunk-based processing to handle large datasets efficiently
- Filtered relevant features for modeling
- Generated language-specific subsets for deeper analysis

### Modeling & Analysis
- Explored relationship between recall probability (`p_recall`) and time gap (`delta`)
- Applied regression modeling to quantify learning decay patterns
- Analyzed the impact of historical performance (`history_correct`, `history_seen`)
- Compared behavioral patterns across different languages

---

## Key Insights

- Recall probability decreases as time intervals increase, consistent with forgetting curve patterns  
- Historical performance strongly influences future recall probability  
- Learning behavior varies across languages, indicating differences in difficulty and user interaction patterns  
- Data-driven modeling provides a quantitative view of user retention dynamics  

---

## Repository Structure

- `data_cleaning.py` – data preprocessing and feature extraction  
- `modeling.ipynb` – modeling, analysis, and visualization  

---

## Tech Stack

- Python (pandas, NumPy)
- Statistical Modeling & Regression Analysis
- Data Processing (large-scale data handling)
- Data Visualization

---

## Notes

This repository focuses on my individual contributions and is designed as a clean, presentation-ready version of a larger team project.

EDA work conducted by other team members is not included.
