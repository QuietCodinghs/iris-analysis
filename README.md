# Iris Dataset: Descriptive and Inferential Statistical Analysis

A reproducible analysis of Fisher's Iris dataset using Python, SciPy, Matplotlib and Jupyter Notebook.

## What this project does
- **Descriptive statistics:** summary measures (mean, median, std, IQR, skewness, kurtosis, CV), per-species summaries and correlation matrices.
- **Visual analytics (Matplotlib):** histograms, box plots, violin plots, scatter plots, scatter-plot matrix, correlation heatmap, confidence-interval plot and regression diagnostics.
- **Inferential statistics:** Shapiro-Wilk normality, Levene test, one-way ANOVA and Kruskal-Wallis (with eta-squared), Tukey HSD post-hoc tests, Welch t-test / Mann-Whitney with Cohen's d, 95% confidence intervals, correlation tests and simple linear regression.

## Repository structure
```
iris-analysis/
├── iris_analysis.ipynb   # analysis and narrative (outputs included)
├── data/iris.csv         # dataset (150 rows, 4 features + species)
├── figures/              # charts saved by the notebook
├── requirements.txt
├── .gitignore
└── README.md
```

## How to run
```bash
git clone https://github.com/QuietCodinghs/iris-analysis.git
cd iris-analysis
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook iris_analysis.ipynb
```
Then choose **Kernel → Restart & Run All** to regenerate all tables and figures.

## Key results
- All three species differ significantly on every feature (ANOVA and Kruskal-Wallis, p < 0.001).
- Petal length and petal width are the most discriminating features (species explains about 94% and 93% of their variance).
- Petal length and petal width are strongly correlated (r = 0.96), but largely because of differences between species.

## Data source
The Iris dataset (Fisher, 1936), as distributed with scikit-learn.
