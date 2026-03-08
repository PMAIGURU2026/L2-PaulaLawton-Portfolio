# October 2025 — Exploratory Data Analysis

**Month:** October 2025  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

This project focuses on Exploratory Data Analysis (EDA) — the critical first step in any data science workflow. Using real-world datasets, the work involved cleaning messy data, uncovering patterns, generating hypotheses, and communicating findings through visualizations.

## Topics Covered

- Data wrangling with `Pandas` (handling missing values, type casting, merging datasets)
- Statistical summaries: mean, median, standard deviation, correlations
- Data visualization with `Matplotlib` and `Seaborn`
- Identifying and handling outliers
- Feature engineering basics

## Project Highlights

- **NYC Open Data Analysis:** Analyzed a publicly available dataset of NYC service requests (311 data) to identify the most common complaint types by borough and time of year.
- **Correlation Heatmaps:** Generated correlation matrices to identify relationships between numeric features.
- **Distribution Plots:** Explored feature distributions to inform preprocessing decisions for later modeling.

## Skills Demonstrated

- End-to-end EDA pipeline from raw CSV to polished visuals
- Writing reusable data cleaning functions
- Storytelling with data — annotating charts and writing interpretive summaries

## How to Run

```bash
pip install pandas matplotlib seaborn jupyter

jupyter notebook
```

## Key Takeaways

Good EDA prevents poor models. Spending time understanding the data before modeling uncovered several data quality issues that would have silently hurt model performance. Visualization is not just for presentations — it is a debugging tool.
