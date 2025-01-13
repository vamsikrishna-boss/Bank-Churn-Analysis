

# Project : Bank-Churn-Analysis
## 1. Interduction
**Objective:**

  The project aims to analyze customer churn data, identify key factors contributing to customer attrition, and provide insights to improve retention strategies.

**Scope:**

  This analysis focuses on active and inactive customers, credit card holders, and key demographic data (gender, geography) to uncover patterns and trends influencing churn.

## 2. Dataset Overview
**Data Sources:**
The project leverages the following tables:

    **Active_Customers :** Tracks active customer details.

    **Bank_Churn :** Core dataset containing customer attributes like age, balance, credit score, and churn status.

    **Credit_Card :** Details of credit card ownership.

    **CustomerInfo :** Personal details of customers.

    **Date Master :** Date-related dimensions for time-based analysis.

    **Exit_Customer :** Records of customers who churned.

    **Gender :** Gender classification.

    **Geography :** Geographical locations.

    **Calculations :** Derived metrics for advanced analysis.

## Key Columns :

    **CustomerId:** Unique identifier for customers.

    **IsActiveMember:** Status indicating whether a customer is active.

    **CreditType:** Type of credit used by the customer.

    **Exited:** Indicator of churned customers (1 = churned, 0 = retained).

     EstimatedSalary, Balance, Age: Key attributes for demographic and financial insights.

## 3. Data Model
**Relationships:**

    Bank_Churn is the central table, connected to:

    Date Master (on Date fields)

    Gender (on GenderID)

    Geography (on GeographyID)

    Credit_Card (on CreditID)

    Exit_Customer (on ExitID)

    One-to-many relationships exist between master tables and fact tables to ensure accurate slicing and dicing of data.

**Key Measures and Calculations:**

    Total Customers: COUNT(CustomerId)

    Churn Rate: (SUM(Exited) / COUNT(CustomerId)) * 100

    Active vs Inactive Customers: Segmentation by IsActiveMember.

##  <p align="center">
    <img src='https://github.com/user-attachments/assets/9794b51d-82f5-4222-bdbd-b89e39d201a8' height="400">
## </p>    

  ![image](https://github.com/user-attachments/assets/9794b51d-82f5-4222-bdbd-b89e39d201a8)

    
## 4. Dashboard Overview
**Main Pages:**

Homepage:
**
KPIs:**

    Displays Total Customers, Active Customers, Inactive Customers, Credit Card Holders, Exit Customers, and Retained Customers.

    **Bar Chart:** Yearly analysis of customers by active/inactive status.

    **Line Chart:** Monthly trend of churned customers.

    **Pie Chart:** Distribution of churn based on credit card ownership.

    **Bar Chart:** Exit customers by credit type and gender.

**Churn% Page:**

    Detailed analysis of churn percentages by various dimensions, including geography, gender, and product usage.

    **Interactivity:**

    Filters for Year, Month, Geography, Exit Category, Gender, and Active Status.

  ![image](https://github.com/user-attachments/assets/a701d463-fa99-48f9-8953-8f983f7b2b2a)
  ![image](https://github.com/user-attachments/assets/4615f5b4-8f3e-400d-bee9-40196cfd23d6)


## 5. Insights & Observations
**Key Insights:**

    Majority of churned customers are non-credit card holders.

    Significant churn peaks observed in specific months (e.g., October and December).

    Customers with low credit scores are more likely to churn.

    Gender and geography play a crucial role in churn patterns.

**Correlation Analysis:**

    Active members are more likely to be retained compared to inactive members.

## 6. Technical Details

**Tools Used:**

    **Power BI:** For creating interactive dashboards and visualizations.
    **SQL Server:** For managing and querying data.
    **Excel:** For initial data cleaning and exploration.

**Data Transformation:**

    Applied Power Query transformations to clean and preprocess the data.
    Created DAX measures for advanced calculations.
## 8. Conclusion

    The "Customer Churn Analysis" dashboard provides actionable insights into churn patterns, helping businesses focus on retention strategies. By implementing data-driven decisions, customer satisfaction and loyalty can be enhanced.

  Project link:


    


    
    

