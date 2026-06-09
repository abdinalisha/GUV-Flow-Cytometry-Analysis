# GUV Flow Cytometry Analysis

Custom Python pipeline for quantifying GUV aggregation using imaging flow cytometry data from the Amnis ImageStreamX Mk II.

## What it does
Classifies events as single-like or aggregate-like based on area and width of the Cy5 membrane signal, with thresholds calibrated automatically from the negative control of each experiment.

## Requirements
pip install pandas numpy matplotlib scipy

## How to use
1. Export your IDEAS data as .txt files (tab-separated, all Cy5 channel parameters)
2. Open `GUV_Flow_Analysis_Final.ipynb`
3. Edit Cell 2 — set your file paths and condition label
4. Run All Cells

## Output
- Classification scatter plots (area vs width)
- Cross-dataset aggregation index comparison
- Paired t-test statistics
- GraphPad-formatted summary CSV
