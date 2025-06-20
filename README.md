# Iris Dataset Exploratory Data Analysis (EDA)

This project demonstrates how to load, inspect, and visualize the **Iris dataset** to understand data trends, feature distributions, and outliers. The dataset is a classic in machine learning and contains measurements of three species of Iris flowers.

---

##  Objective

Learn and apply fundamental data analysis techniques using `pandas`, `matplotlib`, and `seaborn`:

- Load and inspect datasets using pandas.
- Generate descriptive statistics.
- Visualize data using scatter plots, histograms, and box plots.
- Understand relationships between features and identify potential outliers.

---

##  Dataset

- **Name:** Iris Dataset  
- **Format:** CSV / Seaborn built-in  
- **Features:**
  - `sepal_length` (cm)
  - `sepal_width` (cm)
  - `petal_length` (cm)
  - `petal_width` (cm)
  - `species` (Setosa, Versicolor, Virginica)

The dataset can be loaded directly via Seaborn:
```python
import seaborn as sns
df = sns.load_dataset('iris')
