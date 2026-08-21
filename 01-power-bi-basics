# Day 1 — Power BI Learning Notes

## 1. What is Power BI?

Power BI is a **Business Intelligence (BI) and data visualization tool** developed by Microsoft. It helps organizations connect to data, transform and analyze it, create interactive reports and dashboards, and generate insights that support better business decisions.

---

## 2. Power BI Main Views

### Report View

Report View is mainly used to **create interactive reports and dashboards**.

We can use different visualizations such as:

* Bar charts
* Column charts
* Line charts
* Pie/donut charts
* Cards
* Tables
* Slicers
* Maps

### Table/Data View

Table View allows us to **see and inspect the data** that has been loaded into Power BI.

We can:

* View rows and columns
* Check values
* Understand the structure of the data
* Check columns and data types

### Model View

Model View is used to **connect and manage relationships between different tables**.

It helps us understand how tables are connected and how data will interact when creating reports.

---

## 3. Fields/Data Pane, Visualizations and Filters

After loading data into Power BI, different panes are available on the right side.

### Data/Fields Pane

This shows the **tables and columns** that have been loaded into Power BI.

### Visualizations Pane

This contains different types of charts and visual elements that can be used to create reports.

### Filters Pane

The Filters pane allows us to **filter the data displayed in a visual, page, or entire report**.

For example, we can filter a sales chart by:

* Country
* Product
* Date
* Category

---

# 4. Getting Data

Power BI provides a **Get Data** option through which we can connect to different data sources such as Excel, CSV and databases.

After selecting and loading a data source, we generally have two choices:

### Load

Loads the data directly into Power BI.

### Transform Data

Opens the **Power Query Editor**, where we can clean and transform the data before loading it into the Power BI data model.

---

# 5. Power Query Editor

Power Query is used for **data cleaning and transformation** before the data is used for analysis and visualization.

The Power Query Editor provides many options for transforming data.

### Applied Steps

The **Applied Steps** section records the transformations performed on the data.

For example:

1. Changed data type
2. Removed columns
3. Removed duplicates
4. Filtered rows
5. Renamed columns

Each transformation becomes a step, and previous steps can be edited or removed if required.

### Query Pane

The left side shows the **queries/tables** that we are currently working with.

---

# 6. M Language

**M** is the language used by Power Query to perform data transformation and cleaning tasks.

When transformations are performed through the Power Query interface, Power BI generates the corresponding **M code** in the background.

M can also be used directly to create or modify transformation steps.

---

# 7. Basic Data Cleaning Techniques

Before creating visualizations, the data should be checked and cleaned properly.

### A. Check Headers

First, we should verify that:

* Column names are correct
* The correct row is being used as the header
* Headers are not duplicated or incorrect

If required, we can use **Use First Row as Headers**.

### B. Check Data Types

We should check whether each column has the correct data type.

Common data types include:

* Text
* Whole Number
* Decimal Number
* Date
* Date/Time
* True/False

Incorrect data types can cause problems during calculations and visualization.

### C. Transform Data Types

Power Query allows us to convert a column from one data type to another when required.

For example:

**Text → Date**

or

**Text → Whole Number**

### D. Remove Unwanted Columns

Columns that are not required for analysis can be removed to keep the dataset clean and efficient.

### E. Merge Columns

Multiple columns can be combined when required.

For example:

**First Name + Last Name → Full Name**

### F. Split Columns

A column can also be separated into multiple columns.

For example:

**Full Name → First Name + Last Name**

### G. Remove Duplicates

Duplicate records can be identified and removed when they are not required for analysis.

### H. Remove Unwanted Rows/Data

Rows that are irrelevant to the business problem can be filtered or removed.

This helps ensure that the final analysis is based only on relevant data.

---

# 8. Handling Null/Missing Values

Null or missing values should be checked before performing analysis.

There are generally two approaches:

### Option 1 — Fix/Replace the Missing Values

If the correct value can be identified, the missing value can be replaced appropriately.

For example:

* Replace missing category with a known category
* Replace missing numerical value using an appropriate business rule

### Option 2 — Remove the Records

If the missing information cannot be reasonably corrected and the records are not useful for analysis, the affected rows may be removed.

However, removing rows can result in **loss of data**, so the decision should be based on the business requirement and the reason for the missing values.

---

# Key Learning from Day 1

Today I learned the basic structure and workflow of Power BI:

**Get Data → Transform/Clean Data → Load Data → Create Model → Create Visualizations → Apply Filters → Build Reports**

I also learned about:

* Power BI as a Business Intelligence tool
* Report View
* Table/Data View
* Model View
* Data/Fields pane
* Visualizations pane
* Filters pane
* Get Data
* Load vs Transform Data
* Power Query Editor
* Applied Steps
* M language
* Data types
* Headers
* Merging and splitting columns
* Removing duplicates and unwanted data
* Handling null/missing values

**Main takeaway:** Good dashboards depend on good-quality data. Before creating visualizations, the data should be properly checked, cleaned, transformed, and modeled.




# Day 1 — Power BI Learning Notes (Continued)

## 9. Handling Null/Missing Values

When we find null or missing values, we generally have two approaches:

1. **Remove the records containing missing values**
2. **Fix or replace the missing values**

The correct approach depends on the **dataset size, percentage of missing values, and business importance of the affected data**.

### Scenario 1 — Large Dataset + Few Null Values

If the dataset is very large and the percentage of null values is very small, for example **less than 1%**, we may consider removing those records if doing so does not affect the analysis.

**Example:**

A dataset contains 1,000,000 records, but only 5,000 records have missing values.

If those records are not important to the business analysis, removing them may have very little overall impact.

### Scenario 2 — Small Dataset + Many Null Values

If the dataset is small and a significant percentage of values are missing, simply deleting those records can cause substantial data loss.

In this situation, it may be better to **investigate and replace/impute the missing values** where a valid business rule exists.

Possible methods include:

* Mean
* Median
* Mode
* Business-rule-based replacement
* Other appropriate statistical imputation methods

### Important Consideration — Data Bias

Replacing missing values can also introduce **bias** if the replacement method is inappropriate.

Therefore, before deciding whether to remove or replace missing values, we should consider:

* How much data is missing?
* Why is the data missing?
* Is the column important?
* How will removing the records affect the analysis?
* Is there a reliable method for estimating the missing values?

**Key principle:**

> Do not automatically remove or replace missing data. Choose the method based on the data and business requirement.

---

# 10. Removing Duplicate Data

Duplicate records can affect analysis and lead to incorrect results.

For example, if the same transaction appears twice, total sales or order counts may become incorrect.

### Removing Duplicate Rows

If complete rows are duplicated, we can select the appropriate option in **Power Query** to remove duplicate rows.

This keeps only one occurrence of the duplicate record.

### Removing Duplicate Values from a Column

If we need to identify unique values in a particular column:

1. Select the column.
2. Right-click the column header.
3. Select **Remove Duplicates**.

Power Query will retain the first occurrence and remove subsequent duplicate values according to the selected column(s).

**Important:** We should only remove duplicates when we are sure they are actual duplicates. Two rows having the same value in one column does not necessarily mean the entire records are duplicates.

---

# 11. Checking Data Quality

Power Query provides useful tools for checking the quality of columns.

In the **View** tab, we can enable **Column Quality**.

Column Quality provides information such as:

* **Valid** — values that meet the expected requirements
* **Error** — values that contain errors
* **Empty** — missing/null values

This helps us quickly identify data-quality problems before performing analysis.

---

# 12. Changing Data Types

Every column should have an appropriate data type.

For example:

| Column        | Appropriate Data Type |
| ------------- | --------------------- |
| Customer Name | Text                  |
| Quantity      | Whole Number          |
| Price         | Decimal Number        |
| Order Date    | Date                  |
| Revenue       | Decimal Number        |
| Delivered     | True/False            |

We can change a column's data type by selecting the column and using the **data type option in Power Query**.

Correct data types are important because they affect:

* Calculations
* Sorting
* Filtering
* Date analysis
* DAX calculations
* Visualizations

For example, if a date column is incorrectly stored as text, Power BI may not be able to perform proper date-based analysis.

---

# Key Learning

Today I learned that data cleaning is not simply about deleting incorrect data.

Before removing or fixing data, we should understand **how much data is affected and why it is missing or incorrect**.

A basic decision process is:

**Identify problem → Measure impact → Understand the reason → Choose Remove or Fix → Validate the result**

This helps maintain data quality while reducing the risk of unnecessary data loss or bias.

