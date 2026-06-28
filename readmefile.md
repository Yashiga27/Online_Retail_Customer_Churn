# 🛒 Online Retail Customer Churn Prediction using Machine Learning

An end-to-end Machine Learning project that predicts customer churn for an online retail business. This project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, performance evaluation, and business insights to help improve customer retention.

---

# 📁 Project Structure

```text
Online-Retail-Customer-Churn/
│
├── Online Retail Customer Churn.ipynb    # Main Jupyter Notebook
├── online_retail.csv                     # Dataset
└── README.md                             # Project Documentation
```

---

# 📖 Notebook Overview

| Section | Description |
|----------|-------------|
| 1 | Import Libraries |
| 2 | Load Dataset |
| 3 | Data Exploration |
| 4 | Exploratory Data Analysis (EDA) |
| 5 | Data Preprocessing |
| 6 | Model Training & Evaluation |
| 7 | Hyperparameter Tuning |
| 8 | Model Comparison |
| 9 | Final Results Summary |
| 10 | Business Insights & Recommendations |

---

# 🚀 Getting Started

## Option A – Run Locally

### Step 1 – Clone or Download the Project

Using Git:

```bash
git clone https://github.com/Yashiga27/Online_Retail_Customer_Churn.git
cd Online-Retail-Customer-Churn
```
Or download the ZIP file and extract it.

---

### Step 2 – Install Python

Download Python 3.10 or later from:

https://www.python.org/downloads/

Run the installer.

✅ Important: Check the box "Add Python to PATH" during installation.

Verify installation:

```bash
python --version
```

---

### Step 3 – Install Jupyter Notebook

```bash
pip install jupyter
```

Launch Jupyter:

```bash
jupyter notebook
```

---

### Step 4 – Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
```

---

### Step 5 – Place the Dataset

Ensure your dataset is inside the project folder.

- Download the datadet and upload it. 

Example:

```text
Online-Retail-Customer-Churn/
│
├── Online Retail Customer Churn.ipynb
├── online_retail.csv
└── README.md
```

---

### Step 6 – Run the Notebook

Open

```
Online Retail Customer Churn.ipynb
```

Run all cells from top to bottom.

---

# ☁️ Option B – Run on Google Colab (No Installation Required)

Google Colab allows you to run Jupyter notebooks directly in your web browser without installing Python or Jupyter Notebook on your computer.

---

## Step 1 – Open Google Colab

Go to:

https://colab.research.google.com/

Sign in using your Google account if prompted.

---

## Step 2 – Upload the Notebook

1. Click **File** → **Upload Notebook**.
2. Browse to your project folder.
3. Select:

```
Online Retail Customer Churn.ipynb
```

The notebook will open in a new Colab tab.

---

## Step 3 – Upload the Dataset

Since Google Colab does not permanently store your files, you need to upload the dataset every time you start a new session.

1. On the left sidebar, click the **📁 Files** icon.
2. Click **Upload**.
3. Select your dataset file (for example, `online_retail_customer.csv`).
4. Wait until the upload is complete.

Your uploaded dataset should now appear in the Files panel.

> **Note:** If your notebook uses a different dataset filename, upload that file instead.

---

## Step 4 – Install Required Libraries

Some libraries may already be installed in Google Colab. To ensure compatibility, add a new code cell at the top of the notebook and run:

```python
!pip install xgboost imbalanced-learn
```

If your notebook requires additional packages, install them here as well.

---

## Step 5 – Update the Dataset Path (If Needed)

If your notebook reads the dataset using a local path, modify it to use the uploaded file.

Example:

```python
import pandas as pd

df = pd.read_csv("online_retail.csv")
```

Since the dataset is uploaded into Colab's working directory, you usually only need the filename.

---

## Step 6 – Run the Notebook

Run the notebook from top to bottom.

You can either:

- Click **Runtime → Run all**, or
- Run each cell individually by pressing **Shift + Enter**.

Allow each cell to finish executing before running the next one.

---

## Step 7 – View the Results

After execution, the notebook will display:

- Data exploration outputs
- Charts and visualizations
- Model training progress
- Performance metrics
- Confusion matrix
- Classification report
- Final model comparison
- Business insights and conclusions

---

## Important Notes

- Google Colab sessions are temporary.
- Any uploaded datasets will be deleted when the runtime disconnects.
- You must upload the dataset again whenever you start a new Colab session.
- If you modify the notebook, remember to download it using **File → Download → Download .ipynb** to save your changes.

---

# 📊 Machine Learning Pipeline

## Phase 1 – Data Loading

- Import required libraries
- Load the retail dataset
- Display dataset dimensions
- Inspect data types
- Identify missing values

---

## Phase 2 – Exploratory Data Analysis (EDA)

The notebook explores the customer dataset by:

- Understanding customer behaviour
- Checking feature distributions
- Detecting missing values
- Identifying outliers
- Visualizing important variables
- Exploring churn distribution

---

## Phase 3 – Data Preprocessing

The preprocessing stage includes:

- Removing unnecessary columns
- Handling missing values
- Encoding categorical variables
- Feature scaling
- Train-Test Split
- Preparing data for machine learning models

---

## Phase 4 – Model Training

Several classification models are trained and evaluated, including:

### Logistic Regression

- Simple baseline classifier
- Fast training
- Easy interpretation

### Random Forest

- Ensemble learning model
- Handles nonlinear relationships
- Feature importance analysis

### XGBoost

- Gradient Boosting model
- High predictive performance
- Optimized using hyperparameter tuning

---

## Phase 5 – Hyperparameter Tuning

The notebook improves model performance using:

- Grid Search
- Cross Validation
- Parameter optimization

This helps identify the best-performing model configuration.

---

## Phase 6 – Model Evaluation

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

The models are compared to determine the best overall performer.

---

## Phase 7 – Model Comparison

Performance comparison charts are generated to compare:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

These visualizations make it easier to identify the strongest model.


---
# 📊 Model Performance Summary

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------|---------:|----------:|--------:|---------:|--------------|
| Logistic Regression | 51.00% | 51.21% | 55.24% | 54.21% | 47.80 %| 
| Random Forest | 47.50% | 50.00% | 52.38% | 51.16% | 48.44% |
| XGBoost | 49.00% | 51.15% | 63.81% | 56.78% | 47.92% |
---
**Best Model:** XGBoost was selected as the final model because it achieved the highest Recall (63.81%) and F1-Score (56.78%). In customer churn prediction, correctly identifying customers who are likely to leave is more valuable than maximizing overall accuracy, making XGBoost the most suitable model for this project.
## Phase 8 – Business Insights

The project concludes with business recommendations based on model findings.

Possible insights include:

- Identify customers at high risk of churn.
- Improve customer retention strategies.
- Target customers with personalized promotions.
- Reduce revenue loss from customer attrition.
- Support data-driven marketing decisions.

---

# 📦 Required Libraries

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
imbalanced-learn
```

Install everything using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
```

---

# 📈 Project Workflow

```text
Load Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Engineering
      │
      ▼
Data Preprocessing
      │
      ▼
Train-Test Split
      │
      ▼
Model Training
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Model Evaluation
      │
      ▼
Business Insights
```

---

# 🎯 Project Objective

The objective of this project is to develop a machine learning model capable of predicting customer churn in an online retail business. By identifying customers who are likely to leave, businesses can implement targeted retention strategies, improve customer satisfaction, and increase long-term profitability.

---

# 👨‍💻 Author

Machine Learning Group Project

Course: Machine Learning

Topic: Online Retail Customer Churn Prediction