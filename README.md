# Machine Learning Algorithms Using Python

A hands-on machine learning project implementing **Regression, Classification, Clustering, and Association Rule Mining** on an e-commerce dataset using Python and Jupyter Notebook.

## 📌 Project Overview

This project demonstrates the implementation of multiple machine learning techniques to analyze e-commerce customer data, predict customer spending scores, classify customer churn, identify customer segments, and discover product purchase associations.

The project is designed to build practical understanding of machine learning workflows, including data preparation, model training, prediction, evaluation, clustering, and association rule generation.

## 🎯 Objectives

- Implement regression to predict customer spending scores.
- Apply classification to predict customer churn status.
- Segment customers using the K-Means clustering algorithm.
- Discover frequently purchased product combinations using the Apriori algorithm.
- Generate association rules using support, confidence, and lift.
- Export analysis results to CSV files.

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- MLxtend

## 📂 Project Structure

```text
Machine-Learning-Algorithms/
│
├── README.md
├── ML_Algorithms.ipynb
├── ecommerce_multitask_dataset.csv
├── Updated_Ecommerce_data_with_clusters.csv
├── Association_report.csv
└── requirements.txt
```

*Note: The CSV output files are generated when the relevant notebook cells run. Include the dataset only if you are permitted to share it.*

## 📊 Machine Learning Algorithms

### 1. Regression — Polynomial Regression

**Objective:** Predict the customer spending score using customer-related features.

**Implementation:**
- Select input features such as age, annual income, total purchases, and total spent.
- Generate polynomial features of degree 2.
- Split the data into training and testing sets.
- Train a Linear Regression model.
- Evaluate the predictions using the R² score.

**Libraries:** Scikit-learn, Pandas, NumPy, Seaborn.

### 2. Classification — Customer Churn Prediction

**Objective:** Predict customer churn status using customer behavior and spending information.

**Implementation:**
- Select customer features and the churn status target.
- Split the dataset into training and testing sets.
- Build a Scikit-learn pipeline with StandardScaler and RandomForestClassifier.
- Train the classification model.
- Evaluate the predictions using accuracy score.

**Algorithm:** Random Forest Classifier.

### 3. Clustering — Customer Segmentation

**Objective:** Group customers into three clusters based on their characteristics and purchasing behavior.

**Implementation:**
- Select age, annual income, spending score, total purchases, and total spent.
- Apply the K-Means clustering algorithm with three clusters.
- Assign cluster labels to the dataset.
- Visualize the clusters using a scatter plot.
- Export the updated dataset to CSV.

**Algorithm:** K-Means Clustering.

**Output file:** `Updated_Ecommerce_data_with_clusters.csv`

### 4. Association Rule Mining — Apriori Algorithm

**Objective:** Discover frequent product combinations and relationships between items purchased by customers.

**Implementation:**
- Extract purchased items from the `ItemsBought` column.
- Convert transactions into a one-hot encoded format using TransactionEncoder.
- Identify frequent itemsets using the Apriori algorithm with a minimum support of 0.04.
- Generate association rules using a confidence threshold of 0.1.
- Analyze support, confidence, and lift.
- Export the association rules to CSV.

**Libraries:** MLxtend and Pandas.

**Output file:** `Association_report.csv`

## 📐 Evaluation Metrics

| Technique | Metric / Parameter |
|---|---|
| Regression | R² score |
| Classification | Accuracy score |
| Clustering | Number of clusters and visual inspection |
| Association Rule Mining | Support, confidence, and lift |

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or a compatible Python version
- Jupyter Notebook or JupyterLab
- Required Python libraries

### 1. Clone the repository

```bash
[git clone https://github.com/YOUR_USERNAME/Machine-Learning-Algorithms.git](https://github.com/karan-codes45/Machine-Learning-Algorithms.git)
```

### 2. Navigate to the project directory

```bash
cd Machine-Learning-Algorithms
```

### 3. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn mlxtend notebook
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `ML_Algorithms.ipynb` and execute the cells in order.

### 5. Configure the dataset path

Update the dataset loading cell to use a relative path if the CSV file is included in the repository:

```python
df = pd.read_csv("ecommerce_multitask_dataset.csv")
```

Make sure the CSV filename and location match your actual dataset.

## 📁 Generated Outputs

| File | Description |
|---|---|
| `Updated_Ecommerce_data_with_clusters.csv` | Customer dataset with assigned cluster labels |
| `Association_report.csv` | Generated association rules with support, confidence, and lift |

## 💡 Key Learning Outcomes

- Understanding supervised and unsupervised machine learning.
- Implementing regression and classification models with Scikit-learn.
- Building machine learning pipelines.
- Performing customer segmentation using K-Means.
- Applying association rule mining to transaction data.
- Evaluating model predictions and interpreting association metrics.
- Exporting machine learning results for further analysis.

## 🚀 Future Improvements

- Compare multiple regression and classification algorithms.
- Evaluate classification using precision, recall, F1-score, and a confusion matrix.
- Scale features before K-Means clustering and assess cluster quality.
- Tune hyperparameters using cross-validation.
- Visualize association rules and frequent itemsets.
- Add a customer analytics dashboard using Power BI.

## 👨‍💻 Author

**Karan Pawar**

Aspiring Data Analyst | Python | SQL | Power BI | Machine Learning

GitHub: https://github.com/karan-codes45

---

⭐ If you find this project useful, consider starring the repository.
