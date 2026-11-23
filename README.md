# Customer and Insurance Dataset — Exploratory Data Analysis

A notebook-based exploratory data analysis project examining customer demographics, driving history, credit scores, annual mileage, and insurance-claim outcomes.

## Overview

The analysis uses a publicly hosted customer dataset and follows a structured EDA workflow: data inspection, missing-value treatment, descriptive statistics, univariate analysis, relationship analysis, and grouped comparisons of claim outcomes.

## Questions Explored

- How are customers distributed across income and education categories?
- What do credit-score and annual-mileage distributions look like?
- How do annual mileage and speeding violations relate?
- How are selected driving-history variables correlated?
- How do mileage and credit-score distributions differ by claim outcome?
- How do income, education, gender, and family status compare across claim outcomes?

These are exploratory questions; observed associations should not be interpreted as causal relationships.

## Analysis Workflow

1. Load the CSV dataset with Pandas.
2. Inspect shape, columns, types, summary statistics, and missing values.
3. Impute missing credit scores using income-group means.
4. Impute missing annual mileage using the overall mean.
5. Remove identifier and postal-code columns from the analysis.
6. Create univariate plots, scatter plots, correlation heatmaps, box plots, and pivot-table visualizations.
7. Derive a binary claim-rate field for grouped comparisons.

## Technology

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook

## Repository Contents

```text
.
├── customer_analysis.ipynb
└── README.md
```

## Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Nuaima/-Customer-Dataset-Exploratory-Data-Analysis-EDA-.git
   cd -Customer-Dataset-Exploratory-Data-Analysis-EDA-
   ```
2. Install the required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Launch Jupyter and open `customer_analysis.ipynb`.
4. Run the notebook cells in order. The notebook reads the dataset from an external raw GitHub CSV URL, so an internet connection is required.

## Data and Interpretation Notes

- The source dataset is referenced externally and is not included in this repository.
- Mean imputation can change distributions and correlations; the notebook's choices are intended for an exploratory exercise.
- The analysis is observational. It does not establish that demographic or driving variables cause insurance claims.
- Validate missing-data assumptions and check for outliers before using this workflow for any formal modelling or business decision.
