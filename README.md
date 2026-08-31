# sprint4-final-project

## Description
This project provides an end-to-end Exploratory Data Analysis (EDA) on real-world e-commerce data from Olist, the largest department store marketplace in Brazil. By merging, querying, and analyzing dataset relational structures spanning 2016 to 2018, this analysis evaluates business performance across four key dimensions: order fulfillment health, revenue drivers by product vertical, geographic concentration, and logistical impact on customer satisfaction.

## Data Source
Dataset Source: The dataset consists of 7 relational CSV files from the Olist Brazilian E-Commerce dataset hosted on the Practicum curriculum S3 bucket.

## Methods and Tools
- Python (`pandas`, `sqlite3`, `matplotlib`)
- SQL (In-memory `sqlite3` aggregation, multi-table `JOIN` operations, window-style percentages)
- Jupyter Notebook / Google Colab

## Key Findings
- **High Fulfillment Success:** 97.02% of all orders reach "delivered" status cleanly, with canceled and unavailable orders combining for under 1.3%.
- **Concentrated Top Revenue Drivers:** `health_beauty` ($1,446,622.08) and `watches_gifts` ($1,306,761.40) lead total revenue generation while maintaining strong customer review averages (>4.0 stars).
- **Geographic Clustering:** Customer demand is heavily concentrated in the Southeast region of Brazil, led by São Paulo (SP) with 41,746 customers, followed by Rio de Janeiro (RJ) and Minas Gerais (MG).
- **Delivery Speed Drives Ratings:** There is a strong negative correlation ($r = -0.3337$) between transit time and review scores—1-star reviews averaged 20.85 delivery days, whereas 5-star reviews averaged 10.22 days.

## How to Reproduce
1. Clone this repository: `git clone https://github.com/username/olist-ecommerce-eda.git`
2. Install dependencies: `pip install pandas matplotlib`
3. Run the analysis: `jupyter notebook eda_notebook.ipynb`
