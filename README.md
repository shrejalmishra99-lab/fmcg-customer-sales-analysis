# FMCG Customer & Sales Analysis

Exploratory data analysis of customer data from an FMCG (Fast Moving Consumer Goods) company, done in Python. The goal is to clean the data and find patterns in customer spending.

## Business Questions

1. Which product category earns the most revenue?
2. Who are the main customers of the company?
3. Does income affect how much customers spend?

## Dataset

- Customer Personality Analysis dataset (`marketing_campaign.csv`), separated by semicolons (`;`)
- About 2,240 customers and 29 columns: customer background, income, and spending on Wine, Fruits, Meat, Fish, Sweets and Gold products
- Source: [Kaggle - Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
- The dataset is not included in this repository. Download it from the link above and place it in the same folder as the notebook.

## Data Cleaning

- Dropped 24 rows with missing `Income` values
- Removed an income outlier (666,666), keeping incomes below 200,000
- Removed junk values in `Marital_Status` (`Alone`, `Absurd`, `YOLO`)
- Created a new `Total_Spend` column by adding up all product categories

## Key Findings

- **Wine and Meat** are the top revenue-generating categories and together make up more than half of total spend.
- **Married and Together** customers form the largest customer group, so families are the core customer base.
- **Income has a strong positive effect on spending.** Higher-income customers spend more and show a much wider spread.

## Business Recommendations

- Prioritize stock, offers and marketing budget for Wine and Meat.
- Target family-pack offers at Married/Together customers.
- Use premium offers for high-income customers and budget combo packs for lower-income customers.

## Tools Used

- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook (VS Code)

## Files

| File | Description |
|------|-------------|
| `fmcg-customer-sales_analysis.ipynb` | Full analysis with code, charts and interpretations |
| `FMCG.pptx` | Presentation summarizing the project |

## How to Run

1. Clone or download this repository
2. Download `marketing_campaign.csv` from the Kaggle link and place it in the same folder
3. Install the libraries: `pip install pandas matplotlib seaborn`
4. Open the notebook and click **Run All**

## Author

**Shrejal Mishra** | [LinkedIn](https://www.linkedin.com/in/shrejal-mishra-6135212b7) | [GitHub](https://github.com/shrejalmishra99-lab)
