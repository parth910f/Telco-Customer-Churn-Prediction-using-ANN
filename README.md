# 📞 Telco Customer Churn Prediction using ANN

## 📌 Overview  
This project uses an Artificial Neural Network (ANN) to predict customer churn from the **IBM Telco Customer Churn** dataset. The model helps identify customers who are likely to leave, enabling the telecom business to proactively implement **customer retention strategies**.

---

## 🔹 Objectives  
- ✅ Clean and preprocess the dataset  
- ✅ Perform Exploratory Data Analysis (EDA)  
- ✅ Build and evaluate an ANN model to predict churn  
- ✅ Visualize the result

---

## 📊 Dataset Information  

The dataset contains information about customer demographics, service subscriptions, and billing details. It includes:

| Column        | Description |
|---------------|-------------|
| `Churn`       | Target variable indicating if the customer left |
| `tenure`      | Number of months the customer has stayed |
| `Contract`    | Type of contract (Month-to-month, One year, etc.) |
| `PaymentMethod` | Customer's payment method |
| `MonthlyCharges` | Monthly billing amount |
| `TotalCharges` | Total billing amount |
| `gender`, `SeniorCitizen`, `Partner`, `Dependents` | Demographic details |
| `InternetService`, `TechSupport`, `StreamingTV`, etc. | Services used |

- 📁 **Rows:** 7,043  
- 📄 **Target Variable:** `Churn`  
- 🔗 [IBM Dataset Source](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113)

---

## 🔥 Key Features  

### 1️⃣ Data Cleaning & Preprocessing  
- Handled missing and inconsistent values (e.g., `TotalCharges`)
- Encoded categorical columns using label encoding and one-hot encoding  
- Normalized numerical features  
- Converted `Churn` column to binary labels (0 = No, 1 = Yes)

### 2️⃣ Exploratory Data Analysis (EDA)  
- Analyzed churn distribution by contract type, tenure, payment method, etc.  
- Identified high-risk segments  
- Visualized patterns using count plots, heatmaps, and bar charts

### 3️⃣ ANN Model for Churn Prediction  
- Built a sequential ANN model using **Keras** and **TensorFlow**  
- Optimized using activation functions and optimizers  
- Trained on 80% of the data and tested on 20%  
- Evaluated with accuracy, precision, recall, and F1-score

### 4️⃣ Data Visualization   
- Count plots and bar charts for categorical analysis  
- ROC curve & confusion matrix

---

## 📈 Results & Insights  

- 🎯 Model Accuracy: **80%** on Tesing Data &   **82%** on Tesing Data
- 📉 Month-to-month contracts had the highest churn rate  
- 📊 Lack of tech support and online security correlated with higher churn  
- 💸 Electronic check payment method linked to higher churn  

---

## 🛠️ Technologies Used  

- **Language**: Python  
- **Libraries**:  
  - Data Processing: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Modeling: `TensorFlow`, `Keras`, `sklearn`  

---

## 📂 Repository Structure  

```plaintext
📁 Telco-Customer-Churn-ANN/
├── customer_churn_ann.ipynb        # Jupyter notebook with full pipeline
├── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Dataset file
└── README.md                       # Project documentation
