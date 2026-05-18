# Factor of Safety (FoS) Variance Data Pipeline (SOL-05)

This project focuses on tracking the statistical variance of the **Factor of Safety (FoS)** under cyclic operational loads to identify structural reliability risks that traditional scalar design methods miss.

##  Features
- **Robust Automated Ingestion:** Features a localized `try-except` framework to securely parse messy data-logging logs without runtime execution crashes.
- **Data Integrity Cleansing:** Automates duplicate removal, enforces strict column data types, and resolves empty missing metrics cells using median imputation.
- **Vectorized Analytics Engine:** Utilizes memory-contiguous NumPy structures to execute fast statistical calculations (Central tendencies, Variance, Pearson's Skewness).
- **Automated Outlier Sweeps:** Employs Interquartile Range ($IQR$) filtering ($1.5 \times \text{IQR}$) to isolate extreme localized anomalies and stress concentrations.
- **Multi-Dimensional Visualization:** Automatically renders publication-grade static charts (`.png`) alongside interactive, time-series web animations (`.html`) tracking degradation trends over extended operating cycles.

## Tech Stack & Dependencies
- **Core Environment:** Python 3.10+
- **Data Processing:** Pandas, NumPy
- **Visual Synthesis Engines:** Matplotlib, Seaborn, Plotly Express

## Setup
git clone "your-repository-url"
cd "repository-folder"
