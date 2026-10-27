# statistical-analysis-project

This project conducts a complete statistical analysis of the Metro Interstate Traffic Volume dataset: descriptive statistics, three visual models (histogram, boxplot, correlation heatmap), and a one-way ANOVA testing whether mean hourly traffic volume differs across weather conditions on I-94.

**Dataset:** [Metro Interstate Traffic Volume](https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume) (Hogue, 2019) — 48,204 hourly records of westbound I-94 traffic volume near Minneapolis-St Paul, merged with hourly weather observations.

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Running the notebook

```bash
source .venv/bin/activate
jupyter notebook analysis.ipynb
```

Run all cells from top to bottom to reproduce the descriptive statistics, visualizations, and hypothesis test. `build_notebook.py` is the script used to generate `analysis.ipynb` from scratch (run it, then `jupyter nbconvert --to notebook --execute --inplace analysis.ipynb` to re-execute).

## Report

`module_summary.pdf` is the written statistical analysis report (built from `module_summary.html` via WeasyPrint), covering methods, results, non-technical interpretation, limitations/bias, and references.
