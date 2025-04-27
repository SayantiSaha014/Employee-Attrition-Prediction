

<h1 align="center">  📊Employee Attrition Prediction📊</h1>
  <div align="center">
</div>

<div align="center">
  <img src="Attrition logo.jpeg" width='200'>
</div>

---


## 📜 Introduction
In this project , the goal is to predict employee attrition, by using Logistic Regression model trained on the HR Analytics Employee Attrition dataset and which will help HR teams to take proactive measures to improve retention. The dataset contains various features related to employee demographics, job satisfaction, work-life balance, and more. Visualization of the insights is done on a PowerBI dashboard.


## Dataset Name: HR Employee Attrition & Performance

## 📜 **Link of the Dataset**
https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

Description: It includes information on employee satisfaction, income, seniority, demographics, and other relevant attributes.

**Rows**

- Each Row Represents a Single Customer: 1470 numbers

Every row corresponds to an individual employee with their unique Employee_number(EmployeeID) .

**Columns**

- The dataset comprises Columns: 35 numbers

Named

- Age: Employee's age
- Attrition: Whether the employee left the company (Yes/No)
- Business Travel: Frequency of business travel
- Daily Rate
- Department
- Distance From Home
- Education: Education level (1-5)
- Education Field
- EmployeeCount: (Always 1)
- Employee Number: Employee ID
- Environment Satisfaction: Satisfaction with the work environment (1-4)
- Gender: Employee's gender
- Hourly Rate: Hourly rate of pay
- Job Involvement: Level of job involvement (1-4)
- Job Level
- Job Role
- Job Satisfaction: Satisfaction with the job (1-4)
- Marital Status
- Monthly Income
- Monthly Rate: Monthly rate of pay
- NumCompaniesWorked: Number of companies worked for
- Over18: Whether the employee is over 18 (always 'Y')
- OverTime: Whether the employee works overtime (Yes/No)
- Percent Salary Hike 
- Performance Rating: Performance rating (1-4)
- Relationship Satisfaction: Satisfaction with relationships at work (1-4)
- Standard Hours: Standard hours worked (always 80)
- Stock Option Level
- Total Working Years
- Training Times Last Year
- WorkLifeBalance: Work-life balance (1-4)
- Years At Company
- Years In Current Role
- Years Since Last Promotion
- Years With CurrManager: Years with the current manager


## 📂 Employee Attrition Dashboard
The Employee Attrition Dashboard is a data analytics project designed using PowerBI to empower organizations with insights into employee attrition trends. This dashboard consolidates key performance indicators (KPIs) and visualizations to facilitate a deep understanding of workforce dynamics. Employee_attrition_prediction.pbix

##  📂 **About the Design of the project**
### Google Collab code Workflow
The code follows these steps:

1. Data Loading and Initial Exploration

- Import necessary libraries (NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn).
- Load the dataset (HR-Employee-Attrition.csv) using pd.read_csv().
- Explore the dataset using df.info() to check data types and missing values and df.head() to view the first five rows.
- Get the shape (rows and columns) of the dataset using df.shape.

2. Data Preprocessing

- Handling Missing Values: Check for missing values in each column using df.isnull().sum() and there are no missing values.
- Encoding Categorical Features: Identify categorical columns using df.select_dtypes(include=['object']).columns and apply one-hot encoding using pd.get_dummies() with drop_first=True to avoid multicollinearity.
- Scaling Numerical Features: Identify numerical columns using df_encoded.select_dtypes(include=['int64', 'float64']).columns .
- Apply standard scaling using StandardScaler() to ensure features have similar ranges.

3. Model Training

- Data Splitting: Split the data into training and testing sets using train_test_split() with a test_size of 0.2 and random_state of 42.
- Model Initialization: Initialize a Logistic Regression model using LogisticRegression().
- Model Training: Train the model using lr.fit() with the training data (x_train, y_train).

4. Model Evaluation

- Predictions: Predictions on the test data using lr.predict() and predict probabilities using lr.predict_proba().
- Performance Metrics: Calculation of evaluation metrics such as accuracy, precision, recall, F1 score, confusion matrix, and ROC-AUC score .
- Visualization: Create visualizations like the ROC curve and confusion matrix using Matplotlib and Seaborn to understand the model's performance.


## 🚀**Installation and Setup**

 **Clone the repository:**
  ```bash
  git clone (https://github.com/SayantiSaha014/Employee-Attrition-Prediction.git)
```
