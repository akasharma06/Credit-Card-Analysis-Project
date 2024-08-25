# Credit-Card-Analysis-Project

-- 0. Create a database
CREATE DATABASE ccdb;

-- 1. Use the database
USE ccdb;

-- 2. Create the 'cc_detail' table

CREATE TABLE cc_detail (
    Client_Num INT,
    Card_Category VARCHAR(20),
    Annual_Fees INT,
    Activation_30_Days INT,
    Customer_Acq_Cost INT,
    Week_Start_Date DATE,
    Week_Num VARCHAR(20),
    Qtr VARCHAR(10),
    current_year INT,
    Credit_Limit DECIMAL(10,2),
    Total_Revolving_Bal INT,
    Total_Trans_Amt INT,
    Total_Trans_Ct INT,
    Avg_Utilization_Ratio DECIMAL(10,3),
    Use_Chip VARCHAR(10),
    Exp_Type VARCHAR(50),
    Interest_Earned DECIMAL(10,3),
    Delinquent_Acc VARCHAR(5)
);

-- 3. Create the 'cust_detail' table

CREATE TABLE cust_detail (
    Client_Num INT,
    Customer_Age INT,
    Gender VARCHAR(5),
    Dependent_Count INT,
    Education_Level VARCHAR(50),
    Marital_Status VARCHAR(20),
    State_cd VARCHAR(50),
    Zipcode VARCHAR(20),
    Car_Owner VARCHAR(5),
    House_Owner VARCHAR(5),
    Personal_Loan VARCHAR(5),
    Contact VARCHAR(50),
    Customer_Job VARCHAR(50),
    Income INT,
    Cust_Satisfaction_Score INT
);

-- Data Import Instructions:
-- To load data into these tables, use the MySQL Workbench's 'Data Import Wizard':
-- 1. Right-click on the table (cc_detail or cust_detail) you want to load data into.
-- 2. Select 'Table Data Import Wizard'.
-- 3. Follow the prompts to select your CSV file and map the CSV columns to the table columns.
-- 4. Repeat this process for each table with the corresponding CSV file.

