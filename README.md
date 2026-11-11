# 📊 Sales Prediction Using Machine Learning

### A Machine Learning Project Using Python and Linear Regression

## 📌 Project Overview

This project focuses on analysing historical online retail transaction data and predicting sales using Machine Learning.

The main goal is to understand sales patterns, identify top-selling products, analyse country-wise sales and study monthly sales trends.

A Linear Regression model is developed using Python to estimate monthly sales.

## 🎯 Project Objectives

- Understand and explore the online retail dataset.
- Clean and preprocess raw transaction data.
- Identify missing values and duplicate records.
- Calculate total sales.
- Analyse product-wise and country-wise sales.
- Visualize monthly sales trends.
- Build a Linear Regression model.
- Evaluate model performance using regression metrics.

## 📂 Dataset Information

**Dataset Name:** Online Retail Dataset  
**Dataset Source:** UCI Machine Learning Repository  
**Original Dataset Size:** 541,909 Rows × 8 Columns

### Dataset Columns

| Column | Description |
|---|---|
| InvoiceNo | Invoice number |
| StockCode | Product code |
| Description | Product name |
| Quantity | Number of products purchased |
| InvoiceDate | Transaction date |
| UnitPrice | Price per unit |
| CustomerID | Customer identification |
| Country | Customer country |

## 🧹 Data Cleaning & Preprocessing

The following operations were performed:

1. Loaded the dataset using Pandas.
2. Removed 5,268 duplicate records.
3. Removed rows with missing CustomerID and Description.
4. Removed records with zero or negative quantities.
5. Removed records with zero or negative unit prices.
6. Created a new Sales column.
7. Converted InvoiceDate into datetime format.
8. Extracted monthly sales information.

**Sales Calculation:**

`Sales = Quantity × UnitPrice`

After duplicate removal, the dataset contained 536,641 rows, before the remaining filtering operations.

## 📈 Exploratory Data Analysis

Three major analyses were performed:

### 1. Product-Wise Sales Analysis
Identified the top 10 products based on total sales using a bar chart.

### 2. Country-Wise Sales Analysis
Analysed the top 10 countries based on total sales using a bar chart.

### 3. Monthly Sales Analysis
Created a line chart to understand monthly sales trends.

## 🤖 Machine Learning Model

**Algorithm:** Linear Regression  
**Learning Type:** Supervised Learning  
**Problem Type:** Regression

### Feature Selection

- Input Feature (X): Month
- Target Variable (Y): Sales

### Train-Test Split

- Total Monthly Observations: 13
- Training Records: 10
- Testing Records: 3
- Test Size: 20%
- Random State: 42

The Linear Regression model was trained using Scikit-learn.

## 📊 Prediction Results

| Test Record | Actual Sales | Predicted Sales |
|---|---:|---:|
| 1 | 1,156,205.610 | 730,653.129 |
| 2 | 950,690.202 | 688,474.631 |
| 3 | 570,422.730 | 498,671.392 |

## 📉 Model Evaluation

| Evaluation Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 253,173.13 |
| Mean Squared Error (MSE) | 85,000,057,976.79 |
| Root Mean Squared Error (RMSE) | 291,547.69 |
| R-Squared Score (R²) | -0.4434 |

### Model Performance

The model currently has weak predictive performance.

The negative R-squared score indicates that the model performed worse than predicting the average sales value of the test records.

The model uses only 13 monthly observations and one input feature. Therefore, more data and better features are required to improve prediction performance.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- VS Code

## 📁 Project Structure

```text
Sales-Prediction-Using-Machine-Learning/
│
├── Dataset/
│   └── Online Retail.xlsx
│
├── Notebooks/
│   └── Sales_Prediction.ipynb
│
├── Visualizations/
│   ├── Top_10_Products.png
│   ├── Top_10_Countries.png
│   └── Monthly_Sales_Trend.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

## ▶️ How to Run This Project

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### Step 2: Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn openpyxl jupyter
```

### Step 3: Download the Dataset

Download the Online Retail dataset from the UCI Machine Learning Repository.

Place the Excel file inside the `Dataset` folder.

### Step 4: Open the Notebook

Open `Sales_Prediction.ipynb` using Jupyter Notebook or VS Code.

### Step 5: Run the Code

Execute all notebook cells to perform data cleaning, analysis, visualization, model training and prediction.

## 🚀 Future Improvements

- Use more historical sales records.
- Apply chronological train-test splitting.
- Include previous-month sales as additional features.
- Analyse seasonal sales patterns.
- Compare different Machine Learning algorithms.
- Improve prediction performance.

## 👨‍💻 Author

**Almubeen**

BCA Graduate | Aspiring Data Analyst | Machine Learning Learner

- **GitHub:** https://github.com/almubeen-official
- **LinkedIn:** https://www.linkedin.com/in/almubeen-i/

---

⭐ If you find this project useful, feel free to explore the repository!
