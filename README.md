# Mall Spending Clustering Model

A customer segmentation project using K-Means clustering to analyze mall customer spending and income patterns. This repository demonstrates how to preprocess customer data, determine the optimal number of clusters, visualize customer segments, and classify new customers into behavior-based groups.

## Project Contents

- `customer_model.ipynb` - Jupyter notebook containing data loading, preprocessing, clustering, visualization, cluster profiling, and a prediction helper function.
- `Mall_Customers.csv` - Dataset with customer demographic and spending data.

## Dataset

The data is based on mall customers and includes the following features:

- `CustomerID`
- `Gender`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

## Key Steps

1. Load and inspect the dataset
2. Select `Annual Income (k$)` and `Spending Score (1-100)` for clustering
3. Scale features using `StandardScaler`
4. Use the elbow method to choose the number of clusters
5. Apply K-Means clustering to segment customers
6. Visualize the cluster groups and centroids
7. Analyze cluster profiles by average age, income, spending score, and customer count
8. Predict the cluster for a new customer sample

## How to Run

1. Open `customer_model.ipynb` in Jupyter Notebook or JupyterLab.
2. Run each cell sequentially to reproduce the analysis.

If you prefer a command-line environment, you can also convert the notebook to a Python script or run the analysis in a Python environment that supports the required libraries.

## Dependencies

The notebook uses standard Python data science libraries:

- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Install dependencies using pip if needed:

```bash
pip install pandas scikit-learn matplotlib seaborn
```

## Cluster Profiles

The current model segments customers into five groups, with example labels such as:

- Steady Middle (Average Income/Spend)
- Stars (High Income, High Spend)
- Impulse Buyers (Low Income, High Spend)
- Sensible Spenders (High Income, Low Spend)
- Budget Conscious (Low Income, Low Spend)

## Notes

- The segmentation is based only on income and spending score.
- Additional features like age or gender can be included for richer customer profiling.
- The cluster labels are descriptive and may be adjusted based on business context.

## License

This repository is for educational and exploratory use. Adapt the code and analysis for your own clustering experiments.
