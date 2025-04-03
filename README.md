# 📊 Order Data Analysis

## 📝 Project Overview
This project focuses on analyzing order data using **Python, SQL, Excel, and Google Data Studio**. The goal is to derive meaningful insights from sales trends, product performance, and customer behavior using various data analysis techniques.

## 🚀 Technologies Used
- **Python (Pandas, NumPy, Matplotlib, Seaborn, Plotly)** – Data cleaning, analysis, and visualization.
- **SQL (MySQL / PostgreSQL / SQLite)** – Querying, filtering, and aggregating data.
- **Excel** – Pivot tables and basic visualizations.
- **Google Data Studio** – Interactive dashboard for data visualization.

## 📂 Dataset Details
The dataset consists of **200+ orders** and contains the following columns:

| Column Name       | Description                                  |
|------------------|----------------------------------------------|
| Order ID         | Unique identifier for each order             |
| Order Date       | Date when the order was placed              |
| Ship Date        | Date when the order was shipped             |
| Customer Name    | Name of the customer                        |
| Product Category | Category of the product                     |
| Product Name     | Name of the product                         |
| Quantity         | Number of units ordered                     |
| Sales           | Revenue generated from the order            |
| Discount        | Discount applied to the order               |
| Profit         | Profit earned from the order                 |
| Region          | The geographical region of the order        |

## 📊 Key Analyses Performed
1️⃣ **Data Cleaning & Transformation** (Python & Pandas)  
2️⃣ **Exploratory Data Analysis (EDA)**  
   - Sales trends over time (Line Chart)
   - Most profitable products (Bar Chart)
   - Discount vs. Profit relationship (Scatter Plot)
   - Regional sales performance (Heatmap)
3️⃣ **SQL Queries for Business Insights**  
   - Total sales per region
   - Best-selling products
   - Customer segmentation based on purchase frequency
4️⃣ **Dashboard Creation in Google Data Studio**  
   - Sales by Region (Bar Chart)
   - Best-Selling Products (Pie Chart)
   - Monthly Sales Trend (Line Chart)

## 📦 Setup & Usage
### 🔹 Prerequisites
- Python (Install via [Python.org](https://www.python.org/))
- MySQL/PostgreSQL/SQLite (Database setup)
- Jupyter Notebook or Google Colab
- Google Data Studio Account

### 🔹 Installation Steps
1️⃣ Clone the repository:
```sh
  git clone https://github.com/akashhansda/Order-Data-Analysis.git
  cd Order-Data-Analysis
```
2️⃣ Install required Python packages:
```sh
  pip install pandas numpy matplotlib seaborn plotly mysql-connector-python
```
3️⃣ Load the dataset into SQL database:
```python
  import pandas as pd
  import sqlite3
  
  df = pd.read_csv("order_data.csv")
  conn = sqlite3.connect("orders.db")
  df.to_sql("sales_data", conn, index=False, if_exists="replace")
```
4️⃣ Run Python analysis scripts:
```sh
  python data_analysis.py
```
5️⃣ Connect SQL data to Google Data Studio for Dashboard Visualization.

## 📈 Results & Insights
- 📌 **Top-selling products**: Products that drive the highest revenue.
- 📌 **Seasonality in sales**: Identifying peak order months.
- 📌 **Discount vs. Profit Trends**: Determining optimal discount strategies.
- 📌 **Regional Performance**: Finding high and low-performing regions.

## 🤝 Contributions
Feel free to fork this repository and contribute. If you have any questions, raise an issue!

## 📜 License
This project is licensed under the MIT License.
