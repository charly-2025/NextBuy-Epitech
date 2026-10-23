# NextBuy: from raw data to smart decisions

> Built at **Epitech Rennes** · B-DAT-201 · Data · March 2026

## Overview

Exploration of a real-world dataset of **millions of orders** placed by
thousands of online grocery customers. Each order contains products, products
are grouped into aisles, and aisles into departments. The goal is to turn this
raw data into meaningful indicators and actionable recommendations, then to
predict customer behavior.

## Questions answered

- What are the best and worst selling products and aisles?
- Who are the most valuable customers?
- Which days and hours are the busiest?
- Which products are added to the cart first, and which are reordered the most?
- How many customers order each day, and how many units of each product are sold?
- For each customer: why, when and how much do they buy, and what is their favorite product and moment?
- **Can we predict whether a product will be reordered?**

## Approach

1. **Data preparation**: merging the five datasets and setting optimized column types to handle millions of rows
2. **Exploratory analysis**: aggregations and visualizations answering each business question
3. **Customer profiles**: per-customer habits exported as JSON
4. **Machine learning**: a Random Forest classifier predicting reorders, evaluated with accuracy, ROC AUC, a classification report and a confusion matrix

## Getting started

The dataset is not versioned (it weighs several hundred MB). Place
`orders.csv`, `order_products.csv`, `products.csv`, `aisles.csv` and
`departments.csv` at the root of the repository, then:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt scikit-learn
jupyter notebook notebook.ipynb
```

## Tech stack

`Python` · `pandas` · `Jupyter` · `Matplotlib` · `Seaborn` · `scikit-learn`

---

More of my work on my [portfolio](https://charly-2025.github.io/myPortfolio/).
