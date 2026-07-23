# Customer Segmentation Using RFM Analysis and Clustering

## 📌 Project Overview

Customer segmentation helps businesses understand different groups of customers based on their purchasing behavior. This project applies **RFM (Recency, Frequency, Monetary)** analysis combined with clustering algorithms to identify meaningful customer segments for targeted marketing and business decision-making.

The project follows a complete data science workflow, including data preprocessing, feature engineering, clustering, model evaluation, and business interpretation.

---

## 🎯 Business Problem

Businesses often treat all customers the same, resulting in ineffective marketing campaigns and poor customer retention.

The goal of this project is to answer the following question:

> **Can we group customers with similar purchasing behavior to enable personalized marketing strategies?**

---

## 📊 Dataset

This project uses the **Online Retail II** dataset containing transactional records from an online retail store.

The dataset includes information such as:

- Customer ID
- Invoice Date
- Quantity
- Unit Price
- Country

From these transactions, RFM features were created.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📈 Project Workflow

### 1. Data Cleaning

- Removed missing values
- Removed cancelled transactions
- Removed duplicate records
- Converted invoice dates to datetime format

### 2. Feature Engineering

Generated the three RFM metrics:

- **Recency** – Days since the customer's last purchase
- **Frequency** – Number of purchases
- **Monetary** – Total amount spent

### 3. Data Preprocessing

- Log transformation
- Feature scaling
- Outlier analysis

### 4. Customer Segmentation

The following clustering algorithms were evaluated:

- K-Means
- Gaussian Mixture Model (GMM)
- DBSCAN

### 5. Model Evaluation

Models were compared using the **Silhouette Score**.

| Algorithm | Silhouette Score |
|-----------|-----------------:|
| K-Means | 0.438 |
| Gaussian Mixture Model | 0.289 |
| DBSCAN | 0.595 |

Although DBSCAN achieved the highest silhouette score, it produced one dominant cluster and only detected two outlier customers. Therefore, **K-Means was selected for customer segmentation because it generated more interpretable customer groups suitable for business decision-making.**

---

## 📊 Customer Segments

The final clustering model identifies different customer groups such as:

- VIP Customers
- Loyal Customers
- Regular Customers
- At-Risk Customers
- Lost Customers

These segments can help businesses:

- Personalize marketing campaigns
- Improve customer retention
- Increase customer lifetime value
- Reward loyal customers
- Re-engage inactive customers

---

## 📁 Repository Structure

```
customer-segmentation-clustering/
│
├── data/
├── notebooks/
│   └── customer_segmentation.ipynb
├── images/
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 How to Run the Project

Clone the repository:

```bash
git clone https://github.com/brandonmutua/customer-segmentation-clustering.git
```

Navigate into the project directory:

```bash
cd customer-segmentation-clustering
```


Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run all cells.

---

## 📌 Key Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- RFM Analysis
- Feature Scaling
- Unsupervised Machine Learning
- K-Means Clustering
- Gaussian Mixture Models
- DBSCAN
- Hyperparameter Tuning
- Cluster Evaluation
- Business Insight Generation

---

## 📚 Future Improvements

- Deploy the model as a Streamlit web application.
- Automate customer segmentation for new data.
- Compare additional clustering algorithms such as Agglomerative Clustering and Spectral Clustering.
- Build an interactive customer segmentation dashboard.

---

## 👤 Author

**Brandon Mutua**

Aspiring Data Scientist & Machine Learning Engineer

GitHub: https://github.com/brandonmutua

---

## ⭐ If you found this project useful, consider giving it a star!
