# Amazon Products Analysis 🛒

## Project Overview
This project explores and cleans an **Amazon products sales dataset** (42k items) to prepare it for analysis. The focus is on **data cleaning, normalization, and parsing complex fields** such as price, reviews, delivery details, and sustainability badges.  

The goal is to demonstrate hands-on skills in **Python, Pandas, regex parsing, and Jupyter notebooks**, while extracting actionable insights relevant to business decision-making.

---

## Key Insights
- **Top Selling Products:** Batteries, calculators, and office supplies dominate → Consider targeted promotions or bundle deals for high-demand items.  
- **Price vs Units Bought:** Products priced $0–$20 have the highest sales → Potential to optimize marketing for low-priced items; reevaluate strategies for higher-priced items.  
- **Delivery Trends:** Mondays see the highest delivery volumes → Useful for inventory and logistics planning.  
- **Reviews vs Units Bought:** Moderate positive correlation (Pearson = 0.46) → Products with more reviews generally sell more; encourages review solicitation.  
- **Best Sellers:** Attract more reviews and higher engagement → Highlight top products in promotions.  
- **On Sale vs Full Price:** On-sale items have slightly higher median units sold (5,000 vs 3,000) → Strategic discounting increases engagement.  
- **Sustainability Badges:** Products with strong badges drive higher sales → Sustainability may influence purchase decisions.

---

## Skills Demonstrated
- Data Cleaning & Transformation with Pandas  
- Exploratory Data Analysis & Visualization  
- Handling Missing Data & Complex Fields  
- Communicating Business Insights  

---

## Dataset
- Original dataset: [Kaggle - Amazon Products Sales](https://www.kaggle.com/datasets/ikramshah512/amazon-products-sales-dataset-42k-items-2025)  
- Only a **sample dataset** is included in this repository for GitHub use.

---

## Project Structure
amazon_product_analysis/
├── data/ # Sample dataset
├── images/ # Charts & screenshots
├── notebooks/ # Jupyter notebooks
│ └── 01_data_cleaning_fixed.ipynb
│ └── 02_analysis_fixed.ipynb
├── requirements.txt # Python dependencies
└── README.md

---

## Steps Performed
1. **Download & load dataset** using KaggleHub.  
2. **Normalize numeric fields**: ratings, number of reviews, units sold, prices.  
3. **Convert categorical fields**: Best seller / Sponsored → Boolean.  
4. **Parse coupon values**.  
5. **Extract delivery information**: delivery cost, free delivery, estimated & fastest delivery dates, weekday.  
6. **Clean sustainability badges**.  
7. **Convert collected_at column to datetime**.  
8. **Save cleaned dataset**: full dataset (local) and sample dataset for GitHub.

---

## Example Visualizations
![Top 10 Sold Products](images/top_10_units_bought_annotated.png)  
![Units Bought vs Price Bin](images/units_bought_vs_price.png)  
![Delivery Weekday Trends](images/weekday_delivery_trends.png)  
![Best Seller vs Reviews](images/best_seller_vs_reviews_with_medians_corrected.png)  
![On Sale vs Units Bought](images/units_bought_last_month_sales.png)  
![Sustainability Badges vs Units Bought](images/sustainability_badges_vs_units_bought.png)

> **Tip:** Each visualization includes labels, titles, and annotations for clarity and business context.

---

## How to Run

```powershell
# 1. Clone this repository
git clone https://github.com/dahhyunseo/amazon_product_analysis.git
cd amazon_product_analysis

# 2. Create a virtual environment and activate it
python -m venv venv
# Windows
.\venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

# 3. Install required packages
pip install -r requirements.txt

# 4. Open Jupyter notebooks
jupyter notebook

# 5. Run the notebooks in order, starting with 01_data_cleaning.ipynb
```
