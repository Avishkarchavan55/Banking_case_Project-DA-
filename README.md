# Banking Domain Analytics Project
## Project Overview
Problem Statement
The goal of this project is to develop a practical understanding of risk analytics in the banking and financial services sector. The objective is to use available customer data to minimize the risk of financial loss due to lending by identifying patterns and indicators of repayment behavior. This enables financial institutions to make informed decisions on loan approvals, reducing default rates.

## Solution Approach
The project is structured into two major components:

1. Exploratory Data Analysis (EDA) using Python in a Jupyter Notebook (Project_file.ipynb) to identify trends, patterns, and correlations among variables related to customer financial behavior.

2. Power BI Dashboarding, where the insights derived from the analysis are visualized for business users. These dashboards assist decision-makers in quickly assessing applicant profiles and determining loan eligibility.

The Python notebook serves as the analytical foundation, transforming raw banking data into meaningful features and statistical evidence. These insights are then utilized to build interactive dashboards that reflect income segmentation, credit usage, demographic trends, and behavioral risk indicators.

## About the Dataset
The dataset used in this project consists of detailed client-level information and is structured across multiple interrelated tables. These include:

* Banking Relationship: Contains data related to customer deposits, savings, loans, superannuation accounts, and credit card balances.

* Client-Banking: Demographic information such as nationality, gender, income, age, and loyalty classification.

* Investment Advisor: Details of advisory assignments and relationship managers.

* Period Table: Time-related attributes for trend and behavior tracking.

* Other Metadata Tables: Including Gender, Risk Weighting, Fee Structure, Occupation, and Properties Owned.

The dataset uses primary and foreign keys to maintain relational integrity across tables. This structure allows for complex joins and comprehensive analysis.

## Breakdown of Jupyter Notebook (Project_file.ipynb)
### 1. Data Loading and Initialization
* Imported standard Python libraries: pandas, numpy, seaborn, and matplotlib.

* Loaded the dataset into a DataFrame.

* Assessed initial shape and structure using .shape, .info(), and .describe().

## 2. Data Cleaning and Feature Engineering
* Created a new column, Income Band, by segmenting Estimated Income into three ranges:

* Low: 0 to 100,000

* Medium: 100,000 to 300,000

* High: Above 300,000

This feature was designed to simplify income-based segmentation and support visual grouping in Power BI.

## 3. Univariate Analysis
* Conducted frequency analysis on key categorical attributes:

* GenderId, BRId, IAId, Nationality, Occupation, Properties Owned, Loyalty Classification, Fee Structure, and Risk Weighting.

* Visualized using count plots and bar charts to understand the distribution of categorical variables.

## 4. Bivariate Analysis
* Investigated the relationship between categorical variables by segmenting count plots with the Nationality variable.

* This helped identify demographic skew or associations between nationality and financial behavior.

## 5. Numerical Data Profiling
* Plotted histograms and boxplots for continuous variables such as:

* Superannuation Balance, Savings Balance, Checking Balance, Bank Loans, Credit Card Balance, and Estimated Income.

* Evaluated distribution skews, outliers, and variance in financial assets and liabilities.

## 6. Correlation and Heatmap Analysis
* Generated a correlation matrix across all numerical variables.

* Used a heatmap to visually identify strong or weak linear relationships among variables.

#### Key observations included:

* High correlation between deposits and savings account balances.

* Moderate correlation between estimated income and other balances.

* Weak correlation between property ownership and other financial indicators.


## Power BI Dashboard Summary
The Power BI dashboard was developed to visually interpret and analyze customer banking data for effective credit risk assessment. The key components and insights included are:

* Visualized loan distribution by gender, highlighting financial behavior differences.

* Segmented customers based on income bands (Low, Medium, High) to identify major contributors to loan value.

* Analyzed branch-wise performance (BRId) to understand regional loan disbursement trends.

* Explored nationality-based segmentation to determine customer concentration and loan patterns.

* Presented occupation-wise loan distribution, identifying top professions associated with higher loan amounts.

## Key Insights
* Customers with higher income levels generally hold higher balances in savings, superannuation, and checking accounts.

* Bank Deposits and Savings Balances show high interdependence, suggesting overlapping behavior or product bundling.

* Property ownership does not show a strong direct correlation with liquid financial indicators, implying external influences such as inheritance or location.

* Business Lending activity is only moderately correlated with personal Bank Loans, indicating a separation of business and personal banking behavior for most clients.

* Tracked loan activity over time (2017–2021) to observe trends in customer engagement and lending growth.




