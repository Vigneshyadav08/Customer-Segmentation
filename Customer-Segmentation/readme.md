# Customer Segmentation using RFM Analysis & K-Means Clustering

## 1. Project Overview

This project implements an end-to-end **customer segmentation** solution using **RFM (Recency, Frequency, Monetary) analysis** combined with **K-Means clustering**. The goal is to identify meaningful customer groups based on purchasing behavior and present **actionable business insights** through an interactive **Power BI dashboard**.

The pipeline covers **web scraping, SQL analytics, Python data processing, machine learning, and visualization**—making it suitable for **Data Analyst / Data Science fresher roles**.

---

## 2. Business Problem

Organizations need to:

- Identify **high-value customers**
- Detect **inactive / at-risk customers**
- Optimize **marketing spend** and **retention strategies**

This project addresses these needs by segmenting customers using behavioral metrics and visualizing insights for decision-makers.

---

## 3. Tools & Technologies

| Layer            | Tools                            |
| ---------------- | -------------------------------- |
| Data Collection  | Python (Requests, BeautifulSoup) |
| Data Storage     | CSV                              |
| SQL Analytics    | SQLite                           |
| Data Processing  | Python (Pandas, NumPy)           |
| Machine Learning | Scikit-learn (K-Means)           |
| Visualization    | Power BI                         |
| Version Control  | GitHub                           |

---

## 4. Project Structure

```
Customer-Segmentation-RFM/
│
├── data/
│   ├── retail_transactions.csv
│   ├── rfm_sql_output.csv
│   └── final_customer_segments.csv
│
├── notebooks/
│   ├── web_scraping.ipynb
│   ├── rfm_analysis.ipynb
│   └── kmeans_clustering.ipynb
│
├── sql/
│   └── rfm_queries.sql
│
├── powerbi/
│   └── customer_segmentation_dashboard.pbix
│
└── README.md
```

---

## 5. End-to-End Workflow

1. **Web Scraping**

   - Scraped retail product data from a public website using Python.
   - Simulated customer transactions to generate realistic purchase behavior.

2. **Data Cleaning (Python)**

   - Removed invalid values and handled missing data.
   - Converted dates to SQL-compatible `YYYY-MM-DD` format.
   - Calculated total transaction value.

3. **SQL Analysis**

   - Imported cleaned data into SQLite.
   - Calculated RFM metrics using aggregation and date functions.

4. **RFM Scoring (Python)**

   - Assigned quantile-based RFM scores.
   - Created combined RFM score for customer ranking.

5. **Machine Learning (K-Means)**

   - Scaled RFM features using `StandardScaler`.
   - Determined optimal clusters using the **Elbow Method**.
   - Segmented customers using K-Means clustering.

6. **Visualization (Power BI)**

   - Built an interactive dashboard with KPIs, segment distribution, revenue contribution, and behavioral analysis.

---

## 6. RFM Metrics

- **Recency (R)**: Days since the customer’s last purchase
- **Frequency (F)**: Number of purchases made by the customer
- **Monetary (M)**: Total amount spent by the customer

These metrics quantify customer engagement and value.

---

## 7. Machine Learning Details

- **Algorithm**: K-Means Clustering
- **Type**: Unsupervised Learning
- **Features**: Recency, Frequency, Monetary
- **Why K-Means**:
  - Simple and interpretable
  - Widely used for customer segmentation
  - Easy to explain to business stakeholders

---

## 8. Power BI Dashboard Highlights

The dashboard includes:

- KPI cards (Total Customers, Avg Spend, Avg Recency)
- Customer count by segment (bar chart)
- Revenue contribution by segment (pie chart)
- Behavioral analysis (scatter plot: Recency vs Monetary)
- Interactive slicers for segment-level analysis

---

## 9. Key Insights

- A small customer segment contributes a large portion of revenue.
- Some customers are frequent buyers but low spenders.
- Customers with high recency values indicate churn risk.

---

## 10. Business Recommendations

- Provide loyalty rewards to high-value customers.
- Launch re-engagement campaigns for at-risk customers.
- Upsell frequent low-spending customers.
- Optimize marketing budgets based on segment contribution.

---

## 11. Learnings

- Practical SQL aggregation and date handling
- Hands-on RFM analysis for business problems
- Application of unsupervised learning in real scenarios
- Building an end-to-end analytics project
- Designing business-focused dashboards in Power BI

##

