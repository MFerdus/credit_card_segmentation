 
# 📊 Credit Card Customer Segmentation

This project focuses on **customer segmentation for credit card users** using **unsupervised machine learning** techniques. The objective is to identify distinct customer groups based on spending behavior and usage patterns, enabling data-driven decision-making for marketing, customer retention, and financial strategy.

---

## 📑 Table of Contents

1. [Project Overview](#-project-overview)
2. [Business Problem](#-business-problem)
3. [Dataset Description](#-dataset-description)
4. [Methodology](#-methodology)
5. [Clustering Results & Visualizations](#-clustering-results--visualizations)
6. [Key Findings & Insights](#-key-findings--insights)
7. [How to Run the Project](#-how-to-run-the-project)
8. [Tools & Technologies](#-tools--technologies)
9. [Future Improvements](#-future-improvements)

---

## 🚀 Project Overview

Customer segmentation is a crucial analytical task for financial institutions. By grouping customers based on behavioral similarity, banks and credit card companies can:

* Design personalized marketing campaigns
* Improve customer engagement and retention
* Identify high-value and high-risk customers
* Optimize product offerings

This project uses **K-Means clustering** combined with **dimensionality reduction** to uncover meaningful customer segments.

📌 **Notebook:**
[credit_card_segmentation.ipynb](credit_card_segmentation.ipynb)

---

## 🎯 Business Problem

Credit card customers exhibit diverse spending behaviors. Treating all customers the same results in:

* Ineffective marketing
* Poor customer satisfaction
* Missed revenue opportunities

The goal is to **segment customers into distinct groups** so business strategies can be customized per segment.

---

## 📂 Dataset Description

The dataset contains behavioral attributes related to credit card usage, such as:

* Average balance
* Purchase amounts and frequencies
* Cash advance behavior
* Credit limit
* Payments and minimum payments
* Tenure

These features capture **financial habits and risk profiles** of customers.

---

## 🧪 Methodology

### 1️⃣ Data Preprocessing

* Missing values handled using statistical techniques
* Features standardized using **scaling**
* Highly correlated or redundant variables analyzed

---

### 2️⃣ Dimensionality Reduction

* **Principal Component Analysis (PCA)** used to:

  * Reduce dimensionality
  * Improve clustering performance
  * Enable 2D visualization of clusters

---

### 3️⃣ Clustering

* **K-Means Clustering**
* Optimal number of clusters determined using:

  * Elbow Method
  * Silhouette Score
* Final clusters trained on transformed data

---

## 📈 Clustering Results & Visualizations

### 🔹 Elbow Method

Determines the optimal number of clusters by analyzing inertia.

📷 **Screenshot Placeholder**

```markdown
![Elbow Method](images/elbow_method.png)
![Elbow Method](https://github.com/MFerdus/credit_card_segmentation/blob/main/elbow.JPG)
```

---

### 🔹 PCA Cluster Visualization

Visualizes customer clusters in 2D space.

📷 **Screenshot Placeholder**

```markdown
![PCA Clusters](images/pca_clusters.png)
```

---

### 🔹 Cluster Profiles

Each cluster represents a distinct customer behavior pattern.

📷 **Screenshot Placeholder**

```markdown
![Cluster Profiles](images/cluster_profiles.png)
```

📌 *Tip:*
Create an `images/` folder and save plots from your notebook using:

```python
plt.savefig("images/pca_clusters.png")
```

---

## 🧠 Key Findings & Insights

### 🔍 Cluster Interpretation

Based on the analysis, customers can be broadly grouped into:

* **High-Value Customers**

  * High spending
  * Frequent purchases
  * Strong repayment behavior
    📈 *Ideal targets for premium products*

* **Moderate / Regular Users**

  * Balanced spending
  * Consistent usage
  * Lower risk
    📊 *Good candidates for loyalty programs*

* **Cash-Advance-Heavy Users**

  * Frequent cash advances
  * Higher financial risk
    ⚠️ *Require risk monitoring*

* **Low-Usage Customers**

  * Minimal spending
  * Infrequent transactions
    📢 *Potential upsell opportunities*

---

### 📌 Business Impact

* Enables **data-driven marketing**
* Improves **customer lifetime value**
* Supports **risk-aware decision making**

---

## ▶️ How to Run the Project

```bash
# Clone the repository
git clone https://github.com/MFerdus/credit_card_segmentation.git

# Navigate to project
cd credit_card_segmentation

# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook
```

Open:

```
credit_card_segmentation.ipynb
```

---

## 🛠 Tools & Technologies

* Python
* Jupyter Notebook
* pandas, numpy
* scikit-learn
* matplotlib, seaborn

---

## 🔮 Future Improvements

* Try **DBSCAN / Hierarchical Clustering**
* Automate cluster labeling
* Deploy clustering model via **API**
* Apply model to **real-time transaction data**

---

⭐ *This project demonstrates practical application of unsupervised learning for real-world financial analytics.*
