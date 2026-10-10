# K-Means Clustering for Customer Segmentation

An unsupervised machine learning project demonstrating **K-Means Clustering** to segment mall customers based on their annual income and spending score using **Scikit-Learn**.

---

## 📌 Project Overview

Customer segmentation is an essential marketing strategy that divides a broad target market into subsets of consumers who share common characteristics. Because customer labels are unavailable beforehand, this is solved using **Unsupervised Learning**.

This project implements:
1. **Exploratory Data Analysis (EDA)**: Visualizing distributions of customer Age, Annual Income, and Spending Score.
2. **Feature Extraction**: Identifying optimal feature pairs for meaningful business clustering.
3. **Elbow Method (WCSS)**: Finding the optimal number of clusters ($K$) by computing Within-Cluster Sum of Squares.
4. **2D Cluster Visualization**: Plotting customer segments and their respective centroids.

---

## 🔬 Mathematical Formulations

### 1. K-Means Objective Function (Inertia / WCSS)
$$J = \sum_{j=1}^{k} \sum_{i=1}^{n} \| x_i^{(j)} - c_j \|^2$$
* Where $k$ is the number of clusters, $n$ is the number of cases, and $c_j$ is the centroid for cluster $j$.

### 2. Centroid Update Rule
$$c_j = \frac{1}{|S_j|} \sum_{x_i \in S_j} x_i$$
* Iteratively recalculates the mean of all points assigned to cluster $S_j$ until convergence.

---

## 📊 Dataset

* **File**: `shopping_data.csv`
* **Features**:
  * `CustomerID`: Unique identifier for each customer.
  * `Genre`: Gender (Male / Female).
  * `Age`: Age of the customer.
  * `Annual Income (k$)`: Annual income in thousands of dollars.
  * `Spending Score (1-100)`: Score assigned by the mall based on customer behavior and purchasing data.

---

## 🛠️ Tech Stack & Requirements

* **Python 3.x**
* **Scikit-Learn**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

Install dependencies with:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/RishiRaj1112/K-Means-Customer-Segmentation.git
   cd K-Means-Customer-Segmentation
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open the Jupyter Notebook:**
   ```bash
   jupyter notebook KMeans_Customer_Segmentation.ipynb
   ```

---

## 📈 Identified Customer Segments

The analysis typically reveals distinct behavioral groups:
* **Careful Customers**: High annual income, low spending score.
* **Standard Customers**: Average income and average spending score.
* **Target / VIP Customers**: High annual income and high spending score.
* **Careless Customers**: Low annual income but high spending score.
* **Sensible Customers**: Low annual income and low spending score.

---

## 👤 Author
* **Rishi Raj Talari** - [GitHub Profile](https://github.com/RishiRaj1112)
