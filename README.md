# 📊 Power BI Dashboard

> An interactive and professional **Power BI Dashboard** built for data analysis, business intelligence, KPI monitoring, and data-driven decision making.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge\&logo=powerbi\&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Analysis-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 📌 About The Project

This repository contains a **Power BI Dashboard project** created to convert raw data into meaningful and interactive business insights.

The dashboard uses **Power Query, Data Modeling, DAX, KPI Cards, Charts, Slicers, Filters, and Interactive Visualizations** to provide a complete analytical view of the dataset.

### 🔄 Project Workflow

```text
Raw Data
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
Data Modeling
   ↓
DAX Calculations
   ↓
Interactive Dashboard
   ↓
Business Insights
```

---

# 🎯 Objectives

The main objectives of this project are:

* Analyze raw business data
* Clean and transform data using Power Query
* Create an optimized data model
* Develop meaningful DAX measures
* Create interactive KPI cards
* Build professional Power BI visualizations
* Add slicers and filters for dynamic analysis
* Identify trends and patterns
* Generate actionable business insights
* Present data in an easy-to-understand format

---

# 🛠️ Tools & Technologies

| Technology                | Purpose                        |
| ------------------------- | ------------------------------ |
| 🟨 **Microsoft Power BI** | Dashboard & Visualization      |
| 🔄 **Power Query**        | Data Cleaning & Transformation |
| 🧮 **DAX**                | Measures & Calculations        |
| 📊 **Excel / CSV**        | Data Source                    |
| 🗂️ **GitHub**            | Project Repository             |

---

# 📁 Repository Structure

```text
Power-BI-Dashboard/
│
├── 📊 PowerBI/
│   └── Dashboard.pbix
│
├── 📂 Dataset/
│   └── dataset.csv
│
├── 🖼️ Screenshots/
│   ├── dashboard-overview.png
│   ├── dashboard-analysis.png
│   └── dashboard-details.png
│
├── 📄 Documentation/
│   └── Project-Documentation.pdf
│
└── README.md
```

> Replace the file and folder names above with the actual names in your repository.

---

# 📊 Dashboard Pages

## 🏠 1. Overview Dashboard

The Overview page provides a quick summary of the overall performance.

### Key Features

* Total Revenue
* Total Orders
* Total Customers
* Total Quantity
* Average Order Value
* Growth %
* Performance Summary
* Trend Analysis

### Visuals

* KPI Cards
* Revenue Trend
* Orders Trend
* Category Analysis
* Top Products
* Performance Charts

---

## 📈 2. Performance Analysis

This page provides detailed performance analysis.

### Analysis Includes

* Monthly performance
* Category-wise performance
* Product-wise performance
* Regional performance
* Sales trends
* Top-performing products
* Low-performing products

---

## 👥 3. Customer Analysis

The Customer Analysis page provides insights into customer behavior.

### Key Metrics

* Total Customers
* New Customers
* Repeat Customers
* Average Customer Value
* Customer Revenue Contribution

### Analysis

* Top Customers
* Customer Segmentation
* Customer Purchase Trends
* New vs Returning Customers

---

# 🎛️ Interactive Features

The dashboard includes interactive controls that allow users to dynamically analyze the data.

### Slicers

* 📅 Date
* 📆 Year
* 📅 Month
* 🏷️ Category
* 📦 Product
* 📍 Region
* 👤 Customer
* 💳 Payment Method

### Other Features

* Cross-filtering
* Drill-down
* Drill-through
* Tooltips
* Interactive charts
* Page navigation
* Dynamic KPI cards

---

# 📌 Key Performance Indicators

The dashboard tracks important business KPIs.

| KPI                        | Description                            |
| -------------------------- | -------------------------------------- |
| 💰 **Total Revenue**       | Total revenue generated                |
| 🛒 **Total Orders**        | Total number of unique orders          |
| 📦 **Total Quantity**      | Total quantity sold                    |
| 👥 **Total Customers**     | Total unique customers                 |
| 📊 **Average Order Value** | Average revenue generated per order    |
| 📈 **Growth %**            | Percentage growth over time            |
| ⭐ **On-Time %**            | Percentage of orders completed on time |
| ⚠️ **Delayed %**           | Percentage of delayed orders           |

---

# 🧮 DAX Measures

Example DAX measures used in the project:

### Total Revenue

```DAX
Total Revenue =
SUM(Sales[Revenue])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Sales[Order_ID])
```

### Total Quantity

```DAX
Total Quantity =
SUM(Sales[Quantity])
```

### Average Order Value

```DAX
Average Order Value =
DIVIDE(
    [Total Revenue],
    [Total Orders],
    0
)
```

### On-Time Delivery %

```DAX
On-Time % =
DIVIDE(
    [On-Time Orders],
    [Total Orders],
    0
)
```

> DAX formulas should be modified according to the actual table and column names in the dataset.

---

# 🔄 Data Preparation

The data was prepared using **Power Query**.

### Data Cleaning Steps

* Removed duplicate records
* Handled missing values
* Changed incorrect data types
* Renamed columns
* Removed unnecessary columns
* Standardized values
* Created calculated columns
* Merged datasets where required
* Created relationships between tables

---

# 🔗 Data Model

The dashboard uses relationships between different tables to enable efficient analysis.

A typical structure is:

```text
              ┌───────────────┐
              │     Date      │
              └───────┬───────┘
                      │
                      │
┌──────────────┐ ┌────▼─────┐ ┌──────────────┐
│   Customer   │─│   Fact   │─│   Product    │
└──────────────┘ │  Table   │ └──────────────┘
                 └────┬─────┘
                      │
                ┌─────▼──────┐
                │   Region   │
                └────────────┘
```

The model follows a **star-schema approach** wherever applicable.

---

# 🖼️ Dashboard Preview

## Dashboard Overview

![Dashboard Overview](Screenshots/dashboard-overview.png)

## Dashboard Analysis

![Dashboard Analysis](Screenshots/dashboard-analysis.png)

## Dashboard Details

![Dashboard Details](Screenshots/dashboard-details.png)

> Add your actual screenshots to the `Screenshots` folder using the same filenames, or update the paths above.

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Power-BI-Dashboard.git
```

## 2. Open the Project

Open the following file using **Microsoft Power BI Desktop**:

```text
PowerBI/Dashboard.pbix
```

## 3. Check the Data Source

If Power BI cannot find the dataset:

1. Open **Power BI Desktop**
2. Go to **Transform Data**
3. Select **Data Source Settings**
4. Update the dataset location
5. Apply the changes

## 4. Refresh the Dashboard

Click:

```text
Home → Refresh
```

The dashboard will update using the latest available data.

---

# 💡 Business Insights

The dashboard can be used to answer important business questions:

* Which products are performing best?
* Which categories generate the highest revenue?
* Which region performs best?
* What is the monthly performance trend?
* Which customers contribute the most revenue?
* Which products require improvement?
* What are the peak sales periods?
* How is performance changing over time?
* What percentage of orders are completed on time?

---

# 📈 Key Learnings

This project helped develop practical skills in:

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* Data Modeling
* KPI Development
* Data Visualization
* Business Intelligence
* Data Storytelling
* Interactive Dashboard Development

---

# 🔮 Future Enhancements

Future versions of the dashboard may include:

* 🤖 Machine Learning integration
* 🔮 Predictive analytics
* 📈 Sales forecasting
* 👥 Advanced customer segmentation
* 🚨 Automated alerts
* ☁️ Power BI Service deployment
* 🔄 Automated data refresh
* 📱 Mobile-friendly Power BI layout
* 📊 Advanced drill-through pages
* 📧 Scheduled report distribution

---

# 📜 Project Files

| File             | Description              |
| ---------------- | ------------------------ |
| `Dashboard.pbix` | Main Power BI dashboard  |
| `dataset.csv`    | Source dataset           |
| `Screenshots/`   | Dashboard screenshots    |
| `Documentation/` | Project documentation    |
| `README.md`      | Repository documentation |

---

# 👨‍💻 Author

**Kavya**

### Skills

`Power BI` • `DAX` • `Power Query` • `Excel` • `Python` • `Pandas` • `Data Analytics` • `Data Visualization`

---

# ⭐ If You Like This Project

If you find this Power BI dashboard useful or interesting:

⭐ **Star this repository**

🍴 **Fork the repository**

📢 **Share the project**

💬 **Feel free to provide feedback**

---

# 📄 License

This project is created for **educational, portfolio, and data analytics purposes**.

Please check the license and terms associated with the original dataset before redistributing the data.

---

## 🏆 Final Summary

This project demonstrates an end-to-end **Business Intelligence workflow using Microsoft Power BI**, from raw data preparation and transformation to data modeling, DAX calculations, interactive visualizations, KPI tracking, and business insights.

### 🚀

**Data → Power Query → Data Model → DAX → Visualization → Insights → Decision Making**

---

### 🔖 Topics

```text
power-bi
powerbi-dashboard
business-intelligence
data-analytics
data-visualization
dax
power-query
data-modeling
dashboard
kpi
interactive-dashboard
excel
data-analysis
business-analytics
```
