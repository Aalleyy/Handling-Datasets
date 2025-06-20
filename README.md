
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
````

---

## Tools and Libraries

| Library      | Purpose                        |
| ------------ | ------------------------------ |
| `pandas`     | Data loading and summary stats |
| `matplotlib` | Plotting library (core)        |
| `seaborn`    | Statistical data visualization |

Install via pip if needed:

```bash
pip install pandas matplotlib seaborn
```

---

## Steps Performed

### 1. **Data Loading**

```python
df = sns.load_dataset('iris')
```

### 2. **Data Inspection**

```python
df.shape           # Dataset dimensions
df.columns         # Feature names
df.head()          # First 5 rows
df.info()          # Column info and types
df.describe()      # Statistical summary
```

### 3. **Data Visualization**

####  Pairplot (scatter plot for all feature combinations)

```python
sns.pairplot(df, hue="species")
```

####  Histograms (distribution of feature values)

```python
df.hist(figsize=(10, 8), edgecolor='black')
```

####  Box Plots (for identifying outliers)

```python
sns.boxplot(data=df)
```

Or per species:

```python
sns.boxplot(x='species', y='sepal_length', data=df)
```

---

##  Skills Demonstrated

*  Data loading & cleaning
*  Exploratory data analysis
*  Summary statistics
*  Multi-variate visualization
*  Outlier detection

---

##  Acknowledgements

* The Iris dataset is a classic dataset introduced by Sir Ronald Fisher in 1936.
* Thanks to the developers of `pandas`, `matplotlib`, and `seaborn`.


