# customer-personality-eda
Exploratory Data Analysis of customer demographics, purchasing behavior, spending patterns, and campaign responses using Python.


# Customer Personality Analysis – Exploratory Data Analysis
### Overview

This project performs Exploratory Data Analysis (EDA) on the Customer Personality Analysis dataset to understand customer demographics, purchasing behavior, spending patterns, and campaign responses.

The project was completed as part of my Machine Learning internship at Unlox Academy.

### Objectives

The main objectives of this project are to:

- Understand the structure and characteristics of the dataset
- Clean and validate the data
- Identify and handle missing values and duplicate records
- Detect and handle numerical outliers
- Analyze relationships between numerical and categorical variables
- Engineer meaningful features
- Prepare categorical variables for predictive modeling

### Dataset

**Source:** Kaggle – Customer Personality Analysis

The dataset contains customer demographic information, purchasing behavior, campaign responses, and product spending information.

The raw dataset is not included in this repository. Please obtain it from the original source and place it in the project directory before running the notebook.

**Original Dataset:** 
[View the dataset - Customer Personality Analysis on Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

### Dataset File

The notebook expects the downloaded dataset to be named:

`marketing_campaign.csv`

Place it in the project directory before running the notebook.

### Business Questions
1. Does customer income affect spending behavior?
2. Which product category generates the highest revenue?
3. Do customers with children spend differently?
4. Which purchasing channel is most preferred?
5. What characteristics are common among customers who accepted marketing campaigns?
### Project Workflow
#### Phase 1 – Dataset Selection & Problem Definition
- Dataset source identification
- Dataset overview
- Data dictionary
- Business question formulation
#### Phase 2 – Data Cleaning and Integrity Checks
- Data type inspection
- Missing-value analysis
- Median imputation for missing Income values
- Duplicate detection and removal
- Date conversion
#### Phase 3 – Outlier Analysis
- Numerical feature identification
- Skewness analysis
- Box plot visualization
- IQR-based outlier detection
- Outlier capping using the Winsorization approach
#### Phase 4 – Bivariate & Multivariate Analysis
- Correlation heatmap
- Income vs Education analysis
- Income vs Marital Status analysis
- Product spending analysis
- Total Purchases vs Channel
- Campaign response analysis
- Correlation vs causation discussion
#### Phase 5 – Feature Engineering & Encoding

Created new features including:

- Age
- Total_Children
- Total_Spending

Categorical encoding:

- Label Encoding for the ordinal Education variable
- One-Hot Encoding for the nominal Marital_Status variable
### Key Findings
- Customer income shows positive relationships with several spending-related variables.
- Wine and meat products account for substantial customer spending.
- Customers with fewer children tend to show higher spending patterns.
- Purchasing behavior differs across customer groups.
- Higher income and spending are associated with greater campaign acceptance.
- Total_Spending is a useful engineered feature for future predictive modeling.
- Correlation between variables does not necessarily imply direct causation.
### Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
### Project Files
| File |	Description |
| :--- | :--- |
| `customer_personality_eda.ipynb`	| Complete EDA notebook |
| `EDA_Report.pdf` | Technical project report |
| `requirements.txt` | Python dependencies |
| `.gitignore` | Files excluded from version control|
### How to Run
1. Download the dataset from the original Kaggle source.
2. Place marketing_campaign.csv in the project directory.
3. Install the required Python packages.
4. Open customer_personality_eda.ipynb in Jupyter Notebook or JupyterLab.
5. Run the notebook cells sequentially.
### Future Improvements
Build a predictive model for campaign response.
Perform customer segmentation using clustering techniques.
Compare additional machine learning algorithms.
Develop an interactive dashboard for customer analysis.
