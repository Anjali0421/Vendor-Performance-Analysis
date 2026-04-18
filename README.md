# 📊 Vendor Performance Analysis & Inventory Optimization

## 🚀 Project Overview
This project analyzes vendor performance, sales trends, and inventory efficiency to improve business profitability in a retail/wholesale environment.

It includes:
- Data ingestion from CSV files into a database
- Data transformation & cleaning
- Vendor-level KPI generation
- Exploratory Data Analysis (EDA)
- Business insights & recommendations

---

## 🎯 Business Problem
Efficient inventory and vendor management is critical for maximizing profitability.

Key objectives:
- Identify underperforming brands
- Determine top vendors contributing to revenue
- Analyze bulk purchasing benefits
- Improve inventory turnover
- Compare profitability across vendors

---

⚙️ Tech Stack
Python
Pandas
SQLite
SQLAlchemy
Jupyter Notebook
Power BI
🔄 Data Pipeline
1. Data Ingestion
Reads CSV files from the data/ folder
Stores them as tables in SQLite database
2. Data Transformation
Joins multiple tables:
purchases
sales
vendor_invoice
purchase_prices
Creates a vendor-level summary
3. Feature Engineering

New KPIs created:

Gross Profit
Profit Margin
Stock Turnover
Sales to Purchase Ratio
4. Data Cleaning
Handles missing values
Fixes data types
Removes inconsistencies
Cleans categorical columns
📈 Key Insights
Some products generate negative profit due to pricing issues
Several items have zero sales, leading to dead inventory
Top 10 vendors contribute ~65% of total purchases (dependency risk)
Bulk purchasing reduces unit cost significantly (~72%)
~$2.7M capital is tied in unsold inventory
Low-performing vendors have higher margins but lower sales volume
📊 Analysis & Visualizations
Correlation Heatmaps
Distribution Plots
Vendor Performance Analysis
Profit Margin Comparisons

(Available in Jupyter Notebooks)

💡 Business Recommendations
Optimize pricing for low-sales, high-margin products
Diversify vendor base to reduce dependency
Leverage bulk purchasing for cost efficiency
Reduce slow-moving inventory
Improve marketing strategies for low-performing vendors
▶️ How to Run
# Install dependencies
pip install pandas sqlalchemy

# Run data ingestion
python ingestion_db.py

# Generate vendor summary
python get_vendor_summary.py

📌 Future Improvements
Build automated pipeline (Airflow)
Create interactive dashboard (Streamlit)
Add demand forecasting model
Enable real-time data processing
