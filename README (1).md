# MIS 311 – Assignment #1: Supermarket Sales EDA

## Overview
This project performs **Exploratory Data Analysis (EDA)** on a Supermarket Sales dataset as part of MIS 311 – Introduction to Business Analytics.

## Dataset
- **Source:** Retail supermarket transaction records
- **Size:** 250 rows × 8 columns (after cleaning)
- **Branches:** Branch A (New York / Chicago), Branch B (Los Angeles)
- **Columns:** `sale_id`, `branch`, `city`, `customer_type`, `product_name`, `product_category`, `quantity`, `total_price`

## Project Structure
```
MIS-311/
├── Supermarket Sales EDA.pdf        # Main analysis report
├── Supermarket Sales Data.xlsx      # Dataset
├── chart1_overview.png              # Missing value analysis
├── chart2_category_revenue.png      # Revenue by category
├── chart3_branch_customer.png       # Branch & customer type analysis
├── chart4_desc_stats.png            # Descriptive statistics table
├── chart5_distributions.png         # Distribution plots
└── README.md
```

## Data Cleaning Summary

| Issue | Rows Affected | Action |
|---|---|---|
| Missing `customer_type` | 3 rows | Filled with "Unknown" |
| Missing `product_category` | 6 rows | Filled with "Unknown" |
| Missing `quantity` | 3 rows | Filled with median (11.0) |
| Duplicate rows | 3 rows | Removed |
| **Final clean dataset** | **250 rows** | ✅ Ready for analysis |

## Key Findings

### 🔍 Insight 1: Fruits and Beverages Are the Top Revenue-Generating Categories
Fruits generated the highest total revenue at **$7,505.08** (~23.8% of total), followed by Beverages at **$6,463.17** (~20.5%). Together they account for over **44%** of all sales, making them the most commercially important product lines.

### 🔍 Insight 2: Branch A Significantly Outperforms Branch B, and Members Spend More
Branch A recorded total revenue of **$22,097.47** — nearly **2.5× higher** than Branch B at **$8,948.81**. Member customers also spend on average **$136.30** per transaction vs **$112.99** for Normal customers, a difference of ~20.6%.

## Tools Used
- **Python** – pandas, matplotlib, seaborn

---
*EIU – Eastern International University | MIS 311 Introduction to Business Analytics*
