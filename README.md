# Data-Transformation-Modeling-PowerBI-ASSIGN-1# Power BI Project: Data Transformation & Data Modeling

## 📌 Project Overview

This project is part of my **Data Analytics (DA) – Module 2, Power BI Assignment 1**. The objective is to prepare, clean, transform, and model e-commerce sales data using **Microsoft Power BI and Power Query Editor**.

As an aspiring Data Analyst, I am building my portfolio by applying practical data preparation and data modeling techniques to business datasets. This project demonstrates how raw data can be transformed into a structured and reliable data model for business analysis.

## 🎯 Project Objectives

- Import multiple CSV datasets into Power BI.
- Clean and transform data using Power Query Editor.
- Apply appropriate data types and text formatting.
- Create custom and conditional columns using business logic.
- Merge related datasets using Order ID.
- Identify and handle missing values and duplicate records.
- Sort, filter, group, and aggregate data.
- Establish relationships between tables using Manage Relationships.
- Prepare a structured data model for further analysis.

## 📂 Datasets Used

This project uses three e-commerce datasets:

| Dataset | Description |
|---|---|
| List of Orders | Contains order information, customer names, locations, categories, amounts, and profits. |
| Order Details | Contains order IDs, categories, sub-categories, quantities, amounts, and profits. |
| Sales Target | Contains categories, order months, and sales targets. |

### Key Attributes

**List of Orders**
- Order ID
- Order Date
- Customer Name
- City
- State
- Category
- Amount
- Profit

**Order Details**
- Order ID
- Category
- Sub-Category
- Quantity
- Amount
- Profit

**Sales Target**
- Category
- Month of Order Date
- Target

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop** – Data modeling and report development environment
- **Power Query Editor** – Data cleaning and transformation
- **Power Query M** – Data transformation logic
- **GitHub** – Project documentation and portfolio management

## 🔄 Data Transformation & Cleaning

The following transformation tasks are included in the assignment.

### 1. Data Import
- Imported the three CSV datasets into Power BI.
- Opened the datasets in Power Query Editor for preparation.

### 2. Row Limiting and Data Types
- Restricted the List of Orders table to the first 500 rows.
- Converted Order Date to the Date data type.
- Set Amount and Target to Fixed Decimal Number where appropriate.

### 3. Text Formatting
- Applied Proper Case formatting to Customer Name to maintain consistent capitalization.

### 4. Custom Column Creation

**Location**

Combined City and State into a single column in the format:

`City, State`

**Profit Margin**

Calculated the profit margin using:

`Profit Margin = (Profit / Amount) × 100`

This helps evaluate the profitability of sales relative to the amount.

Note: Rows with missing or zero Amount values require appropriate handling to avoid invalid calculations.

### 5. Conditional Column

Created a column named **Profit Status** based on profit values:

| Condition | Profit Status |
|---|---|
| Profit < 0 | Loss |
| Profit = 0 | Break-Even |
| Profit > 0 | Profit |

This classification helps distinguish profitable, loss-making, and break-even transactions.

### 6. Data Merging
- Merged List of Orders and Order Details using Order ID.
- Named the merged output **Orders Data**.
- Used the appropriate join type based on the assignment requirements and the intended analysis.

### 7. Missing Values and Duplicate Records
- Identified missing values in the datasets.
- Evaluated whether missing values should be replaced, retained, or removed.
- Checked for duplicate rows.
- Considered business logic before removing records to avoid losing valid transactions.

### 8. Sorting and Filtering
- Sorted Orders Data by Order Date in descending order.
- Applied filters to analyze orders from a selected state, such as Tamil Nadu.

### 9. Grouping and Aggregation

Created duplicate/reference working queries as required and performed the following aggregations:

**Order Details**
- Count of Order ID
- Average Profit by Category
- Total Amount by Sub-Category

**Sales Target**
- Total Target by Month of Order Date

These aggregations help summarize sales performance and category-level results.

## 🧩 Data Modeling

The assignment includes relationships between the datasets to support consistent data analysis.

### Relationships

1. **List of Orders ↔ Order Details**
   - Relationship column: Order ID

2. **Order Details ↔ Sales Target**
   - Relationship column: Category

The relationships were intended to be configured and checked in **Model View / Manage Relationships** to ensure they are active and correctly defined.

**Modeling consideration:** Relationship cardinality must be validated against the actual data. If Order ID appears multiple times in both tables, or Category repeats in both tables, a direct many-to-many relationship may cause ambiguous or duplicated calculations. A suitable unique-key dimension or bridge table may be required for a reliable model.

## 📊 Expected Business Value

This project demonstrates how data preparation and modeling support business analysis by helping to:

- Understand sales and profit patterns.
- Identify loss-making and profitable transactions.
- Compare performance across product categories and sub-categories.
- Review monthly sales targets.
- Analyze orders by geographical location.
- Prepare structured data for future reports and dashboards.

These are the intended analytical uses of the prepared datasets, rather than claims of specific findings.

## 📸 Screenshots

Add screenshots from your own Power BI project to document your work.

Suggested folder structure:

```text
Power-BI-Data-Transformation-Modeling/
│
├── README.md
├── Data Transformation and modeling.pbix
│
└── Screenshots/
    ├── 01_Data_Import.png
    ├── 02_Power_Query_Transformations.png
    ├── 03_Custom_Columns.png
    ├── 04_Merged_Orders_Data.png
    ├── 05_Grouping_and_Aggregation.png
    └── 06_Data_Model_Relationships.png
```

Replace the example screenshot names with the actual images you capture. Do not include screenshots for steps you have not completed.

## 📁 Project Deliverables

- Power BI `.pbix` file containing the imported datasets, transformation steps, and data model.
- README documentation describing the project workflow.
- Screenshots demonstrating the transformation and modeling process.
- PDF report explaining the transformation decisions and showing the data model.

## 📚 Key Learnings

Through this assignment, I am developing practical skills in:

- Data import and preparation
- Data cleaning and validation
- Data type conversion and text formatting
- Custom and conditional column creation
- Data merging and integration
- Handling missing values and duplicates
- Grouping and aggregation
- Relationship management and data modeling
- Project documentation using GitHub

## 🚀 Conclusion

This project is an important step in my Data Analytics learning journey. It helps me understand how raw e-commerce data can be cleaned, transformed, integrated, and modeled using Power BI.

I will continue expanding my portfolio with projects involving data analysis, visualization, dashboards, and business insights as I develop my skills as a Data Analyst.

## 👤 About Me

I am an **Aspiring Data Analyst** interested in data cleaning, data transformation, business analysis, and data visualization.

I am building this GitHub portfolio to document my learning journey and showcase my practical projects using analytics tools.

**Tools I am learning:** Excel, Power BI, SQL, and data visualization.

---

*Project: Data Analytics – Module 2, Power BI Assignment 1*  
*Topic: Data Transformation & Data Modeling*
