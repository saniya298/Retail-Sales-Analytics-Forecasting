# Retail-Sales-Analytics-Forecasting

## Project Overview

This project analyzes retail sales data from a Superstore dataset to identify sales trends, profitability drivers, regional performance, and the impact of discounts on profit. The project combines data cleaning, exploratory data analysis (EDA), visualization, and forecasting techniques to generate actionable business insights.

---

## Objectives

- Analyze retail sales performance across categories, regions, states, and products.
- Identify factors influencing profit.
- Study sales trends over time.
- Evaluate the impact of discounts on profitability.
- Generate business insights using data visualization.
- Perform basic sales forecasting.

---

## Dataset Information

- Dataset: Superstore Retail Dataset
- Records: 9,994
- Features: 21
- Data Period: 2014 – 2017

### Key Attributes

- Order Date
- Ship Date
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Discount
- Profit
- Region
- State

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Data Cleaning

The dataset was examined for data quality issues.

### Cleaning Performed

- Checked for missing values
- Checked for duplicate records
- Converted date columns to datetime format
- Verified data types

### Results

- Missing Values: 0
- Duplicate Records: 0

The dataset was already well-structured and required minimal cleaning.

---

## Exploratory Data Analysis (EDA)

### 1. Sales by Category

| Category        | Sales    |
|-----------------|---------:|
| Technology      | $836,154 |
| Furniture       | $741,999 |
| Office Supplies | $719,047 |

### Finding

Technology generated the highest sales among all categories.

---

### 2. Profit by Category

| Category        | Profit   |
|-----------------|---------:|
| Technology      | $145,455 |
| Office Supplies | $122,491 |
| Furniture       | $18,451  |

### Finding

Although Furniture generated strong sales, its profit contribution was significantly lower compared to Technology and Office Supplies.

---

### 3. Sales by Region

| Region  | Sales    |
|---------|---------:|
| West    | $725,458 |
| East    | $678,781 |
| Central | $501,240 |
| South   | $391,722 |

### Finding

The West region generated the highest revenue.

---

### 4. Profit by Region

| Region  | Profit   |
|---------|---------:|
| West    | $108,418 |
| East    | $91,523  |
| South   | $46,749  |
| Central | $39,706  |

### Finding

The West region was the most profitable region in the dataset.

---

### 5. Top States by Sales

| State        | Sales    |
|--------------|---------:|
| California   | $457,688 |
| New York     | $310,876 |
| Texas        | $170,188 |
| Washington   | $138,641 |
| Pennsylvania | $116,512 |

### Finding

California contributed the highest sales and significantly outperformed other states.

---

### 6. Top Selling Products

| Product                               | Sales   |
|---------------------------------------|--------:|
| Canon imageCLASS 2200 Advanced Copier | $61,599 |
| Fellowes PB500 Electric Punch Machine | $27,453 |
| Cisco TelePresence System EX90        | $22,638 |
| HON 5400 Series Task Chairs           | $21,870 |

### Finding

High-value office and technology products were among the top revenue generators.

---

### 7. Discount vs Profit Analysis

A scatter plot was used to study the relationship between discount levels and profit.

### Finding

- Orders with little or no discount generated the highest profits.
- Higher discount levels frequently resulted in reduced profits.
- Several heavily discounted orders produced significant losses.

### Business Insight

Aggressive discounting negatively impacts profitability and should be carefully managed.

---

### 8. Correlation Analysis

| Variables         | Correlation |
|-------------------|------------:|
| Sales ↔ Profit    | 0.48        |
| Sales ↔ Quantity  | 0.20        |
| Profit ↔ Discount | -0.22       |

### Findings

- Sales and Profit show a moderate positive relationship.
- Profit and Discount show a negative relationship.
- Increasing discounts generally reduces profit.

---

### 9. Monthly Sales Trend

Monthly sales were analyzed from 2014 to 2017.

### Findings

- Sales generally increased over time.
- Strong peaks occurred toward the end of each year.
- Highest monthly sales exceeded $115,000.

### Business Insight

The business exhibits seasonal sales patterns, with stronger performance during year-end periods.

---

## Forecasting

A Linear Regression model was used to forecast future sales based on historical monthly sales trends.

### Forecasting Workflow

- Aggregated monthly sales
- Created time-based features
- Trained Linear Regression model
- Predicted future sales values

### Outcome

The model provided a simple projection of future sales trends and demonstrated the application of forecasting techniques to retail business data.

---

## Visualizations Created

- Sales by Category
- Profit by Category
- Sales by Region
- Profit by Region
- Top States by Sales
- Top Products by Sales
- Monthly Sales Trend
- Discount vs Profit Scatter Plot
- Correlation Heatmap
- Sales Forecast Chart

---

## Key Business Insights

1. Technology is the highest-performing category in both sales and profit.
2. The West region contributes the highest revenue and profit.
3. California is the strongest-performing state.
4. High discount rates often lead to lower profits.
5. Sales demonstrate clear seasonal patterns.
6. Premium technology products generate substantial revenue.

---

## Conclusion

This project demonstrates the complete data analytics workflow, including data cleaning, exploratory data analysis, visualization, and forecasting. The analysis revealed important trends in sales performance, regional profitability, and discount strategies. The findings can help businesses make informed decisions regarding pricing, inventory management, and sales planning.

---

## Project Structure

```
Retail-Sales-Analytics-Forecasting/
│
├── data/
│   └── Superstore.csv
│
├── visualizations/
│   ├── sales_by_category.png
│   ├── profit_by_category.png
│   ├── sales_by_region.png
│   ├── profit_by_region.png
│   ├── monthly_sales_trend.png
│   ├── discount_vs_profit.png
│   └── correlation_heatmap.png
│
├── retail_sales_analysis.ipynb
├── README.md
└── requirements.txt
```
