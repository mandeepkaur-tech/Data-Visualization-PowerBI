# 📊 Online Retail Sales Dashboard

> Power BI dashboard analyzing 500K+ UK online retail transactions to uncover revenue trends, top customers, and global expansion opportunities.

An interactive Power BI dashboard built on the **UCI Online Retail Dataset**, analyzing e-commerce transactions from a UK-based online gift retailer (Dec 2010 – Dec 2011). The dashboard uncovers revenue trends, top-performing customers and countries, and international expansion opportunities.

---

## 📑 Table of Contents

- [Dataset Overview](#-dataset-overview)
- [Dashboard Pages](#-dashboard-pages)
  - [1. Monthly Revenue Trend – 2011](#1-monthly-revenue-trend--2011)
  - [2. Top 10 Countries by Revenue (excl. UK)](#2-top-10-countries-by-revenue-excl-uk)
  - [3. Top 10 Customers by Revenue](#3-top-10-customers-by-revenue)
  - [4. Global Product Demand by Country – Expansion Opportunities](#4-global-product-demand-by-country--expansion-opportunities)
- [Key Insights](#-key-insights)
- [Tools Used](#️-tools-used)
- [Repository Structure](#-repository-structure)
- [How to Use](#-how-to-use)
- [Future Enhancements](#-future-enhancements)
- [Author & Contact](#-author--contact)

---

## 📁 Dataset Overview

| Metric | Value |
|---|---|
| Total Records | ~536,641 transactions |
| Date Range | Dec 1, 2010 – Dec 9, 2011 |
| Unique Invoices | ~25,900 |
| Unique Customers | ~4,373 |
| Countries Covered | 38 |
| Total Revenue | ~£9.7M |

**Columns in `Online_Retail_Dataset.csv`:**
- `InvoiceNo` – Unique invoice/transaction number
- `StockCode` – Product/item code
- `Description` – Product name
- `Quantity` – Units sold per line item
- `InvoiceDate` – Date & time of transaction
- `UnitPrice` – Price per unit (£)
- `CustomerID` – Unique customer identifier
- `Country` – Customer's country

---

## 📈 Dashboard Pages

### 1. Monthly Revenue Trend – 2011
- **Total Revenue 2011:** 1.18M
- **Peak Month Revenue:** 1.46M (October 2011)
- **Month-over-Month Growth:** 37.18%
- Revenue trended steadily upward through the year, spiking sharply in Q4 before a projected/forecasted decline into early 2012 (shown via the shaded forecast band).
- Includes an interactive **month slicer** for drilling into specific periods.

- **Dashboard**:(https://github.com/mandeepkaur-tech/Data-Visualization-PowerBI/blob/main/Dashboard%20Slide%201.png)

### 2. Top 10 Countries by Revenue (excl. UK)
- **Netherlands** leads international markets with **£285K** in revenue, followed by **EIRE (£263K)** and **Germany (£222K)**.
- The **top 4 countries** (Netherlands, EIRE, Germany, France) account for **75% of total international revenue**.
- Combo chart overlays revenue (bars) with order quantity (line) for a demand-vs-value comparison.

- **Dashboard**:(https://github.com/mandeepkaur-tech/Data-Visualization-PowerBI/blob/main/Dashboard%20Slide%202.png)

### 3. Top 10 Customers by Revenue
- Customer revenue is highly concentrated — the **top customer (ID ~14646/18102 range)** contributes as much as **£279K** and **£256K** individually.
- A small group of high-value customers (out of 4,373 total) drives a disproportionate share of revenue — signaling strong potential for a **VIP/loyalty retention strategy**.

- **Dashboard**:(https://github.com/mandeepkaur-tech/Data-Visualization-PowerBI/blob/main/Dashboard%20Slide%203.png)

### 4. Global Product Demand by Country – Expansion Opportunities
- A world map visualization highlighting demand concentration across Europe.
- **Netherlands, EIRE, and Germany** emerge as the top targets for expansion outside the UK, based on total quantity ordered (200K+, 142K+, and 117K+ units respectively).
- Total international quantity ordered: **912,621 units**.

- **Dashboard**:(https://github.com/mandeepkaur-tech/Data-Visualization-PowerBI/blob/main/Dashboard%20Slide%204.png)

---

## 🔑 Key Insights

- 📈 Revenue grew consistently across 2011, with an exceptional peak in October, likely tied to pre-holiday/seasonal bulk ordering.
- 🌍 International sales (outside the UK) are concentrated in Western Europe — Netherlands, Ireland, and Germany are prime candidates for deeper market investment.
- 👥 Revenue is customer-concentrated: a handful of large B2B/wholesale-style customers account for a major share of total sales, making customer retention a high-leverage growth lever.
- 🎯 Expansion opportunity: aligning inventory and marketing spend toward the top 4 international markets could capture the majority of untapped international demand.

---

## 🛠️ Tools Used

- **Power BI** – Dashboard design, DAX measures, interactive visuals & slicers
- **Dataset:** [UCI Machine Learning Repository – Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

---

## 📂 Repository Structure

```
├── Online_Retail_Dataset.csv     # Raw transactional dataset
├── Dashboard_Slide_1.png         # Monthly Revenue Trend
├── Dashboard_Slide_2.png         # Top 10 Countries by Revenue
├── Dashboard_Slide_3.png         # Top 10 Customers by Revenue
├── Dashboard_Slide_4.png         # Global Product Demand Map
└── README.md
```

---

## 🚀 How to Use

1. Clone this repository.
2. Open the `.pbix` Power BI file (if included) in Power BI Desktop.
3. Explore the interactive slicers on the Revenue Trend page to filter by month.
4. Refresh the data source to point to the local `Online_Retail_Dataset.csv` if needed.

---

## 📌 Future Enhancements

- Add RFM (Recency, Frequency, Monetary) customer segmentation
- Product-level profitability and returns analysis (negative quantity = returns)
- Cohort analysis for customer retention over time
- Automated data refresh via Power BI Service / cloud gateway

---

## 👤 Author & Contact

**Mandeep Kaur**

- 📧 Email: kaur.mandeeep.08@gmail.com
- 💼 LinkedIn: (https://www.linkedin.com/in/-mandeep-kaur-/)
- 🐙 GitHub: (https://github.com/mandeepkaur-tech)

Feel free to reach out for feedback, collaboration, or questions about this project!

---

*This project is for educational and portfolio purposes, analyzing publicly available retail transaction data.*
