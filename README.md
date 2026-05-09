# Customer Segmentation using K-Means Clustering

A machine learning project that segments mall customers into distinct groups based on their **Annual Income** and **Spending Score** using the K-Means clustering algorithm.

---

## Dataset

**Mall_Customers.csv** — contains 200 customer records with the following features:

| Column | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Genre | Gender of the customer |
| Age | Age of the customer |
| Annual Income (k$) | Annual income in thousands |
| Spending Score (1-100) | Score assigned by the mall based on spending behavior |

---

## Objective

Group customers into **5 segments** to help the mall understand their customer base and make targeted marketing decisions.

---

## 🔧 Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and exploration |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `scikit-learn` | KMeans clustering model |

---

## Approach

### 1. Exploratory Data Analysis
- Checked dataset shape, data types, and null values
- Selected `Annual Income` and `Spending Score` as features

### 2. Elbow Method
Used WCSS (Within-Cluster Sum of Squares) to find the optimal number of clusters.

### 3. K-Means Clustering
- Algorithm: `k-means++`
- Number of clusters: **5**
- `random_state=0` for reproducibility

---

## Results

5 distinct customer segments identified:

| Cluster | Annual Income | Spending Score | Profile |
|---|---|---|---|
| Customer 1 (Blue) | Medium | Medium | Average customers |
| Customer 2 (Red) | High | High | Top spenders |
| Customer 3 (Green) | High | Low | High income, careful spenders |
| Customer 4 (Purple) | Low | Low | Low income, low spenders |
| Customer 5 (Brown) | Low | High | Low income, high spenders |

---

## Project Structure

```
Customer-Segmentation/
│
├── Customer_Segmentation.ipynb   # Main notebook
├── Mall_Customers.csv            # Dataset
└── README.md                     # Project documentation
```

---

## 👤 Author

Made with ❤️ — feel free to fork and star ⭐ if you found it useful!
